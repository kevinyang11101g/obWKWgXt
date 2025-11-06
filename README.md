# 前言

欢迎来到基于SSM的校园二手交易系统项目。本项目旨在为广大高校学生提供一个便捷、高效的二手交易平台，实现闲置物品的循环利用，降低资源浪费。

# 内容介绍

本项目主要包括以下几个模块：用户模块、商品模块、订单模块、消息模块等。用户模块负责用户的注册、登录、个人信息管理等功能；商品模块负责商品的发布、编辑、删除、搜索等功能；订单模块负责订单的创建、支付、取消、评价等功能；消息模块负责实时通知用户关注的信息。

# 技术介绍

## 语言：Java

## 使用框架：Spring Springmvc，Mybatis

## 前端技术：JS、Vue、CSS3

## 开发工具：IDEA/Eclipse

## 数据库：MySQL 5.7/8.0

## 数据库管理工具：phpstudy/Navicat

## JDK版本：jdk1.8

## Maven：apache-maven 3.8.1-bin

## 前端环境：Node.Js 12\14\16

# 核心代码

以下是一段商品查询的相关代码：

```java
// 商品Mapper接口
public interface CommodityMapper {
    // 根据关键词搜索商品
    List<Commodity> searchCommodity(@Param("keyword") String keyword);
}

// 商品Service层
@Service
public class CommodityService {
    @Autowired
    private CommodityMapper commodityMapper;

    public List<Commodity> searchCommodity(String keyword) {
        return commodityMapper.searchCommodity(keyword);
    }
}

// 商品Controller层
@RestController
@RequestMapping("/commodity")
public class CommodityController {
    @Autowired
    private CommodityService commodityService;

    @GetMapping("/search")
    public ResponseEntity<List<Commodity>> searchCommodity(@RequestParam("keyword") String keyword) {
        List<Commodity> commodities = commodityService.searchCommodity(keyword);
        return ResponseEntity.ok(commodities);
    }
}
```

# 免费源码获取

```
5000套系统成品在线演示视频，复制到流浪器： 
```
```
https://www.yuque.com/yuqueyonghux32e1j/kxdc9g/ad8oz3bamkxmay0e#Cxun
```
![下载](https://img12.360buyimg.com/ddimg/jfs/t1/339687/11/1349/28408/68ad865fF412d7877/adaa650483a100f2.jpg)

# 项目截图

![封面图片](https://img13.360buyimg.com/ddimg/jfs/t1/339678/14/8105/82515/68bdd2b6Ff057f610/c026db1619807dfb.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/329531/1/10435/17249/68bdd28eF60851b34/cf39729b25ec2ddb.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/324078/38/16836/85434/68bdd28fF99778462/229be44fe114f164.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/332274/24/10612/46163/68bdd28fFa12b805f/75db860741670d1c.jpg)

![介绍图片](https://img10.360buyimg.com/ddimg/jfs/t1/346533/7/722/29450/68bdd290F7e87f0f7/054e1eacfcd95c3b.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/333325/14/10428/26011/68bdd290Ff5f3202d/2c05fe02d784a8a4.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/334632/32/10592/25914/68bdd291F5b7b1622/9b88586fd86999ac.jpg)

![介绍图片](https://img14.360buyimg.com/ddimg/jfs/t1/336002/37/8124/21576/68bdd291Fcb1252e0/fd24fd6d3f2308cf.jpg)

![介绍图片](https://img13.360buyimg.com/ddimg/jfs/t1/346821/39/600/20946/68bdd292F4794a7e9/808dbc6524f39733.jpg)

![介绍图片](https://img12.360buyimg.com/ddimg/jfs/t1/346564/18/817/17108/68bdd292F86645e50/68db5556f31e931a.jpg)

