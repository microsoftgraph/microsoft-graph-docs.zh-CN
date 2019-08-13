---
title: vpnRoute 资源类型
description: VPN 路由定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 00f5d1eb3f05d11833e687d002e1d698a366fd61
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36367608"
---
# <a name="vpnroute-resource-type"></a>vpnRoute 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN 路由定义。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|destinationPrefix|String|目标前缀 (IPv4/v6 地址)。|
|prefixSize|Int32|前缀大小。 (1-32)。 有效值为1至32|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnRoute"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnRoute",
  "destinationPrefix": "String",
  "prefixSize": 1024
}
```



