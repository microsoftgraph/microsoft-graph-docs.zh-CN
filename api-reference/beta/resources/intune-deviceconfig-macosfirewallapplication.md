---
title: macOSFirewallApplication 资源类型
description: 表示 macOS 防火墙应用程序列表中的应用程序
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 477911dba492bdda09eb815aba968bb7f63955bf
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30145400"
---
# <a name="macosfirewallapplication-resource-type"></a>macOSFirewallApplication 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 macOS 防火墙应用程序列表中的应用程序

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|bundleId|String|应用程序的 BundleId。|
|allowsIncomingConnections|布尔|是否允许传入连接。|

## <a name="relationships"></a>关系
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




