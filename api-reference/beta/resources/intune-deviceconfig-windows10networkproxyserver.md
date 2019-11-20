---
title: windows10NetworkProxyServer 资源类型
description: 网络代理服务器策略。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 10f973747baa7137345cf73d249a81af4d9f3178
ms.sourcegitcommit: d40d2a9266bd376d713382925323aefab285ed69
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/20/2019
ms.locfileid: "38748039"
---
# <a name="windows10networkproxyserver-resource-type"></a>windows10NetworkProxyServer 资源类型

> **重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

网络代理服务器策略。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|address|String|代理服务器的地址。 在 "\>\[服务器：\<端口" \<格式中指定地址\>\]|
|exceptions|String 集合|不应使用代理服务器的地址。 系统无法将代理服务器用于以本节点中指定的内容开头的地址。|
|useForLocalAddresses|Boolean|指定是否应将代理服务器用于本地 (Intranet) 地址。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.windows10NetworkProxyServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.windows10NetworkProxyServer",
  "address": "String",
  "exceptions": [
    "String"
  ],
  "useForLocalAddresses": true
}
```



