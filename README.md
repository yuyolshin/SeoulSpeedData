# Seoul Speed Data

> Dataset for spatial temporal traffic forecasting problem in highly urbanized areas 

This is an average taxi speed datasets of Seoul, South Korea. The original data is retrieved from !TOPIS(https://topis.seoul.go.kr). TOPIS aggregates the raw GPS tracking data collected from DTG (Digital Tacho Graph) on Seoul taxis into 5 min resolution. 
To use the dataset for evaluation of traffic forecasting models, we processed the dataset and defined two study areas - (1) urban-core, and (2) urban-mix Urban-core, located in Gangnam-gu, Seoul, is populated with rather homogeneous 304 links. Urban-mix is an expansion of Urban-core, and it is populated with heterogeneous 1,007 links. The data ranges from 2018.04.01 ~ 2018.04.30 (1 month)

> ![image](https://user-images.githubusercontent.com/31876093/141141076-7d44ed1e-7868-4cf4-9e93-3597b1d97f9f.png)
> (a) _Urban-Core_, and (b) _Urban-mix_

--------------------
## [Link](https://drive.google.com/drive/folders/14i4stoWQcQr6mVXtXKGx2lLw12Cn8kg0?usp=sharing) For the Data
###### The dataset is composed of:
- **urban-core.csv**: speed matrix including the road segments in _urban-core_
  - column 1: Link ID
  - column 2: Link ID (last 5 digits)
  - columns 3 & 4: center point of each road segment
  - column 5: speed limit
  - column 6: road segment length
  - column 7: direction (upward or downward)
  - columns 8~8647: average speeds in 5-min frequency (2018/04/01 00:00 ~ 2018/04/30 11:55)
- **urban-mix.csv**: speed matrix including the road segments in _urban-mix_
  - column 1: Link ID
  - columns 2 & 3: start point of each road segment
  - columns 4 & 5: end point of each road segment
  - column 6: speed limit
  - column 7: -
  - columns 8~8647: average speeds in 5-min frequency (2018/04/01 00:00 ~ 2018/04/30 11:55)
- **Adj(urban-core).csv**: adjacency matrix for _urban-core_. The order of nodes are the same in speed matrix file and adjacency matrix file.
- **Adj(urban-mix).csv**: adjacency matrix for _urban-mix_. The order of nodes are the same in speed matrix file and adjacency matrix file.

-------------------
##### If you are using this dataset for your work, please cite the following reference. 
- Shin, Y., & Yoon, Y. (2020). Incorporating dynamicity of transportation network with multi-weight traffic graph convolutional network for traffic forecasting. IEEE Transactions on Intelligent Transportation Systems.

'''
### This dataset should only be used for research purposes 
'''
