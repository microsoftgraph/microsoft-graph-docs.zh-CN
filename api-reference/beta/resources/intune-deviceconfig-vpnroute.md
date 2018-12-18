---
title: vpnRoute 资源类型
description: VPN 路由定义。
author: tfitzmac
ms.openlocfilehash: 64d755c4f21b47e928c64348a2f1d6dad1f7206a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27322020"
---
# <a name="vpnroute-resource-type"></a>vpnRoute 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

VPN 路由定义。
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|destinationPrefix|字符串|目标前缀 （IPv4/v6 地址）。|
|prefixSize|Int32|前缀大小。 (1-32)。 有效的值 1 到 32|

## <a name="relationships"></a>Relationships
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





