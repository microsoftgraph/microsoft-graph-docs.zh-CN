# <a name="securitynetworkprotocol-enum-type"></a>securityNetworkProtocol 枚举类型

网络协议的可能值。

## <a name="members"></a>成员

|成员|值|说明|
|:---|:---|:---|
|unknown|-1|未知协议。|
|ip|0|Internet 协议。|
|icmp|1| Internet 控制消息协议。|
|igmp|2| Internet 组管理协议。|
|ggp|3| 网关至网关协议。|
|ipv4|4| Internet 协议第四版。|
|tcp|6| 传输控制协议。|
|pup|12| PARC 通用数据包协议。|
|udp|17| 用户数据报协议。|
|idp|22| Internet 数据报协议。|
|ipv6|41| Internet 协议第 6 版 (IPv6)。|
|ipv6RoutingHeader|43| ipv6 路由标头。|
|ipv6FragmentHeader|44| ipv6 片段标头。|
|ipSecEncapsulatingSecurityPayload|50| ipv6 封装安全有效负载标头。|
|ipSecAuthenticationHeader|51| ipv6 身份验证标头。|
|icmpV6|58| ipv6 的 Internet 控制消息协议。|
|ipv6NoNextHeader|59| ipv6 无下一标头。|
|ipv6DestinationOptions|60| ipv6 目标选项标头。|
|nd|77| 网络磁盘协议（非正式）。|
|raw|255| 原始 IP 数据包协议。|
|ipx|1000| Internet 数据包交换协议。|
|spx|1256| 顺排包交换协议。|
|spxII|1257|  顺序包交换第 2 版协议。|