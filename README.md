# 2021 GIScience class at SU
This class aims to introduce the concept of GIScience, techniques of handling geospatial data, and geospatial modeling. Mainly we use R for hands-on. All materials are prepared to be reproducible.

## prerequisite
- [Github](https://github.com/) account
- [Google Earth Engine](http://signup.earthengine.google.com/)
- PC 

## required environments
We will use Docker. All materials and exercise will be run on Docker environment.

## Textbook
We follow two online textbooks. 
- [An Introduction to R](https://intro2r.com)
- [Geocomputation with R](https://geocompr.robinlovelace.net),  
licensed under a Creative Commons Attribution-NonCommercial-NoDerivatives 4.0 International License. 

## Reproducible works
The source code of [Geocomputation with R](https://geocompr.robinlovelace.net) is repreducible using docker.  

With the computer which the [docker](https://docs.docker.com/get-docker/) is installed, run:  

```

# download repo with Windows Powershell or a Unix terminal
git clone https://github.com/Robinlovelace/geocompr.git 
# or download manually from https://github.com/Robinlovelace/geocompr/archive/master.zip
cd geocompr # navigate into the repo
# on linux and mac with password:
docker run -d -p 8786:8787 -v $(pwd):/home/rstudio/data -e USERID=$UID -e PASSWORD=pw geocompr/geocompr
# on linux and mac without password:
docker run -d -p 8786:8787 -e DISABLE_AUTH=TRUE -v $(pwd):/home/rstudio/geocompr  geocompr/geocompr
# on windows without a password:
docker run -d -p 8786:8787 -v ${pwd}:/home/rstudio/data -e DISABLE_AUTH=TRUE robinlovelace/geocompr

```
  
Then, access to ``` http://localhost:8786 ``` to access Rstudio server.  

Another options are to use [binder](https://mybinder.org/v2/gh/robinlovelace/geocompr/master?urlpath=rstudio), or [Rstudio cloud](https://rstudio.cloud/project/1642300). 
It is noted that the cloud based resource often fail to keep connections, which may irritate you.  

<!---
If you want to run on your local machine, install [Rstudio](https://rstudio.com/products/rstudio/) with [R](https://www.r-project.org), then download the source-code and run at R console  

```
install.packages("remotes")
remotes::install_github("geocompr/geocompkg")
```
--->

## schedule
1. イントロダクション・環境構築
2. Rの導入（１）
3. Rの導入（２）
4. 空間データ処理（１）
5. 空間データ処理（２）
6. 地図化（１）
7. 地図化（２）
8. 演習（１）
9. 演習（２）
10. リモートセンシング概論
11. リモートセンシングデータ解析（１）
12. リモートセンシングデータ解析（２）
13. リモートセンシングデータ解析（３）
14. 演習（１）
15. 演習（２）
## References
All materials introduced below are freely available online.  

### GIScience 
- [geocomputation with R](https://geocompr.robinlovelace.net/)  
- [Spatial Data Science](https://keen-swartz-3146c4.netlify.app/)  
- [geospatial analysis](https://spatialanalysisonline.com/HTML/index.html)  
- [Spatio-Temporal Statistics with R](https://spacetimewithr.org/)   

### Basic R
- [R for data science](https://r4ds.had.co.nz/)  
- [GISオープン教材](https://gis-oer.github.io/gitbook/book/)
- [An Introduction to R](https://intro2r.com)

