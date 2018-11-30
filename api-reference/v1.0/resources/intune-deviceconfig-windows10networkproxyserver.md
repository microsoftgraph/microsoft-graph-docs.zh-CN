---
title: windows10NetworkProxyServer 资源类型
description: 网络代理服务器策略。
ms.openlocfilehash: 2cd9d4ddc84733e3985f718fd2d3ef86481d762e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008334"
---
# <a name="windows10networkproxyserver-resource-type"></a>windows10NetworkProxyServer 资源类型

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

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



