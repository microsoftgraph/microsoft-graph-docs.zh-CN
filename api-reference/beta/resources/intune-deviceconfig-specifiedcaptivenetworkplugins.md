---
title: specifiedCaptiveNetworkPlugins 资源类型
description: 指定在 IKEv2 AlwaysOn VPN 连接过程中允许的所有固定网络插件
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 7d205218aab1ef6fb5a59280ff25f5a22fde8c0b
ms.sourcegitcommit: b12904a27b6d0e197f562aca0dac5e74cd7bd3a1
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/31/2020
ms.locfileid: "41636091"
---
# <a name="specifiedcaptivenetworkplugins-resource-type"></a>specifiedCaptiveNetworkPlugins 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

指定在 IKEv2 AlwaysOn VPN 连接过程中允许的所有固定网络插件

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|allowedBundleIdentifiers|String 集合|IKEv2 服务器的地址。 必须是 FQDN、UserFQDN、网络地址或 ASN1DN|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.specifiedCaptiveNetworkPlugins"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.specifiedCaptiveNetworkPlugins",
  "allowedBundleIdentifiers": [
    "String"
  ]
}
```



