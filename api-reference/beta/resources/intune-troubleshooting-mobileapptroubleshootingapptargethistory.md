---
title: mobileAppTroubleshootingAppTargetHistory 资源类型
description: 移动应用程序疑难解答事件中包含的历史记录项。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c0a1d37f86ebb43b7d697a9407ce0e3a479b2350
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402963"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a>mobileAppTroubleshootingAppTargetHistory 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

移动应用程序疑难解答事件中包含的历史记录项。


继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|occurrenceDateTime|DateTimeOffset|历史记录项所发生的时间。 继承自[mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)|
|securityGroupId|String|它已向其目标 AAD 安全组 id。|
|runState|[runState](../resources/intune-shared-runstate.md)|项目的状态。 可取值为：`unknown`、`success`、`fail`。|
|errorCode|String|故障，如果没有出现故障空的错误代码。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.mobileAppTroubleshootingAppTargetHistory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.mobileAppTroubleshootingAppTargetHistory",
  "occurrenceDateTime": "String (timestamp)",
  "securityGroupId": "String",
  "runState": "String",
  "errorCode": "String"
}
```




