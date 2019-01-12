---
title: macOSFirewallApplication 资源类型
description: 代表 macOS 防火墙应用程序列表中的应用程序
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 8ad53f1a30c19a6ab1c3e32dc0871481fbac21f8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954125"
---
# <a name="macosfirewallapplication-resource-type"></a>macOSFirewallApplication 资源类型

> **重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。 在生产应用程序中不支持使用这些 API。

> **注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。

代表 macOS 防火墙应用程序列表中的应用程序
## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|bundleId|String|应用程序的 BundleId。|
|allowsIncomingConnections|布尔|是否允许传入连接。|

## <a name="relationships"></a>Relationships
无
## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.macOSFirewallApplication"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.macOSFirewallApplication",
  "bundleId": "String",
  "allowsIncomingConnections": true
}
```





