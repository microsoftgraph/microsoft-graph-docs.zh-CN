---
title: windowsNetworkIsolationPolicy 资源类型
description: Windows 网络隔离策略
ms.openlocfilehash: 89c7db0453c76f6ec5016a4701bf357e27c579bc
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044947"
---
# <a name="windowsnetworkisolationpolicy-resource-type"></a>windowsNetworkIsolationPolicy 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

Windows 网络隔离策略
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|enterpriseNetworkDomainNames|String 集合|这是构成企业边界的域列表。 将被视为企业数据和保护数据从一个发送到的设备这些域。 这些位置将被视为企业数据到共享的安全目标。|
|enterpriseCloudResources|[proxiedDomain](../resources/intune-shared-proxieddomain.md) 集合|包含需要保护在云中承载的企业资源域的列表。 与这些资源的连接被视为企业数据。 如果代理与云资源配对，则到云资源的流量将通过表示的代理服务器（在端口 80 上）通过企业网络进行路由。 此外必须使用 EnterpriseInternalProxyServers 策略配置代理服务器使用实现此目的。 该集合最多可包含 500 个元素。|
|enterpriseIPRanges|[ipRange](../resources/intune-shared-iprange.md) 集合|设置可定义企业网络中计算机的企业 IP 范围。 来自这些计算机的数据将被视为企业的一部分并受保护。 这些位置将被视为企业数据到共享的安全目标。 该集合最多可包含 500 个元素。|
|enterpriseInternalProxyServers|String 集合|这是逗号分隔的内部代理服务器列表。 例如，“157.54.14.28, 157.54.11.118, 10.202.14.167, 157.53.14.163, 157.69.210.59”。 这些代理已由管理员配置为连接到 Internet 上的特定资源。 它们被视为企业版网络位置。 代理是仅利用中配置 EnterpriseCloudResources 策略以强制转换为通过这些代理的匹配的云资源通信。|
|enterpriseIPRangesAreAuthoritative|Boolean|用于通知客户端接受已配置的列表，并且不使用启发式方法来尝试查找其他子网的布尔值。 默认值为 false。|
|enterpriseProxyServers|String 集合|这是代理服务器的列表。 不在此列表的任何服务器被视为非企业。|
|enterpriseProxyServersAreAuthoritative|Boolean|用于通知客户端接受已配置的代理列表，并且不尝试检测其他工作代理的布尔值。 默认值为 false|
|neutralDomainResources|String 集合|可用于工作或个人资源的域名的列表。|

## <a name="relationships"></a>Relationships
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
      "@odata.type": "microsoft.graph.iPv6Range",
      "lowerAddress": "String",
      "upperAddress": "String"
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





