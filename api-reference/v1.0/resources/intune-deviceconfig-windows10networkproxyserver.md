---
title: windows10NetworkProxyServer 资源类型
description: 网络代理服务器策略。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a6f5562619b2e5ffa26a44cba2eb67a56c787a51
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59123081"
---
# <a name="windows10networkproxyserver-resource-type"></a>windows10NetworkProxyServer 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

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




