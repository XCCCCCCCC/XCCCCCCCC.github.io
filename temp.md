# 网络分层模型和应用协议

## 五层网络模型（TCP/IP协议族核心：分层模型）
* 应用层，HTTP/FTP/DNS/SMTP/POP3协议，封装为http请求报文，由首部和实体组成。
* 传输层，TCP/UDP协议，将请求分为多个数据包，并为数据包打上序号。（三次握手，四次挥手）
* 网络层，IP协议，用ip地址找到目标mac协议。
* 数据链路层，MAC协议，执行发送
* 物理层。

## 数据的传输
## 四层、五层、七层

# 应用层协议

## URL（uniform resource locator），统一资源定位符
### 示例：http（schema）://a.com（domain）:80（port）/news/detail（path）?id=1（query）#t1（hash）
* 当协议是http端口为80时，端口可以省略。
* 当协议是http端口为443时，端口可以省略。
* schema、domain、path是必填的。

## HTTP（Hyper Text Transfer Protocol）

### 传递消息的模式
HTTP使用了一种极为简单的消息传递模式，[请求-响应]模式。
发起请求的称之为**客户端**，接受请求并完成响应的称之为**服务器**。
[请求-响应]完成后，一次交互结束。

### 传递消息的格式

* 请求（request）：
  1. 请求行
  2. 请求头
  3. 请求体
* 响应（response）：
  1. 响应行
  2. 响应头
  3. 响应体