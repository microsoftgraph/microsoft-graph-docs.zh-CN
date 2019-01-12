---
title: vpnServer 资源类型
description: VPN 服务器定义。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 61eaedb7ecca3f4a7074d079f2b10164dfe2ad76
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27969546"
---
# <a name="vpnserver-resource-type"></a>vpnServer 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

VPN 服务器定义。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|说明。|
|address|String|地址 （IP 地址、 FQDN 或 URL）|
|isDefaultServer|Boolean|默认服务器。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.vpnServer"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.vpnServer",
  "description": "String",
  "address": "String",
  "isDefaultServer": true
}
```





