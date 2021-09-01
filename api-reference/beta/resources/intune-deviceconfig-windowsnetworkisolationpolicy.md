---
title: windowsNetworkIsolationPolicy 资源类型
description: Windows网络隔离策略
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c93d9292df647ccec7f6047cbb7a922329855f4e
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58790386"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a>windowsNetworkIsolationPolicy 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Windows网络隔离策略

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|enterpriseNetworkDomainNames|String collection|这是构成企业边界的域列表。 发送到设备的其中一个域的数据将被视为企业数据并受到保护。 这些位置将被视为要共享的企业数据的安全目标。|
|enterpriseCloudResources|[proxiedDomain](../resources/intune-shared-proxieddomain.md) 集合|包含托管在云中需要保护的企业资源域的列表。 与这些资源的连接被视为企业数据。 如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。 用于此目的的代理服务器也必须使用 EnterpriseInternalProxyServers 策略进行配置。 该集合最多可包含 500 个元素。|
|enterpriseIPRanges|[ipRange](../resources/intune-shared-iprange.md) 集合|设置定义企业网络中计算机的企业 IP 范围。 来自这些计算机的数据将被视为企业的一部分并受保护。 这些位置将被视为要共享的企业数据的安全目标。 该集合最多可包含 500 个元素。|
|enterpriseInternalProxyServers|String collection|这是逗号分隔的内部代理服务器列表。 例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。 这些代理已由管理员配置为连接到 Internet 上的特定资源。 它们被视为企业版网络位置。 仅在配置 EnterpriseCloudResources 策略以强制流量通过这些代理访问匹配的云资源时，才利用代理。|
|enterpriseIPRangesAreAuthoritative|Boolean|用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。 默认为 false。|
|enterpriseProxyServers|String collection|这是代理服务器的列表。 不在此列表中的任何服务器都被视为非企业服务器。|
|enterpriseProxyServersAreAuthoritative|Boolean|用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。 默认值为 false|
|neutralDomainResources|String collection|可用于工作或个人资源的域名列表。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windowsNetworkIsolationPolicy"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windowsNetworkIsolationPolicy",
  "enterpriseNetworkDomainNames": [
    "String"
  ],
  "enterpriseCloudResources": [
    {
      "@odata.type": "microsoft.graph.proxiedDomain",
      "ipAddressOrFQDN": "String",
      "proxy": "String"
    }
  ],
  "enterpriseIPRanges": [
    {
      "@odata.type": "microsoft.graph.ipRange"
    }
  ],
  "enterpriseInternalProxyServers": [
    "String"
  ],
  "enterpriseIPRangesAreAuthoritative": true,
  "enterpriseProxyServers": [
    "String"
  ],
  "enterpriseProxyServersAreAuthoritative": true,
  "neutralDomainResources": [
    "String"
  ]
}
```



