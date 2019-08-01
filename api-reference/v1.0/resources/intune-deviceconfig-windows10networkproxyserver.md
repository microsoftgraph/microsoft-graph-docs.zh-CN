---
title: windows10NetworkProxyServer 资源类型
description: 网络代理服务器策略。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: b68f13ab80544d591b22fc77ab35110302dc48ea
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36031008"
---
# <a name="windows10networkproxyserver-resource-type"></a>windows10NetworkProxyServer 资源类型

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

网络代理服务器策略。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|address|String|代理服务器的地址。 按照以下格式指定地址：<server>\[“:”<port>\]|
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



