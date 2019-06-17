---
title: vpnServer 资源类型
description: VPN 服务器定义。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 540741a6b3df349e5a096070e7973e3dadc2533e
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34987514"
---
# <a name="vpnserver-resource-type"></a>vpnServer 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

VPN 服务器定义。

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|说明|String|说明。|
|address|String|地址 (IP 地址、FQDN 或 URL)|
|isDefaultServer|Boolean|默认服务器。|

## <a name="relationships"></a>关系
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





