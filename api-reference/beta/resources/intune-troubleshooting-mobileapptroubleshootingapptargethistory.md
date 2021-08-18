---
title: mobileAppTroubleshootingAppTargetHistory 资源类型
description: 包含在移动应用疑难解答事件中的历史记录项。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 737114ea576344f268c1100a70afed2f27ef1f3e
ms.sourcegitcommit: 0116750a01323bc9bedd192d4a780edbe7ce0fdc
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2021
ms.locfileid: "58261129"
---
# <a name="mobileapptroubleshootingapptargethistory-resource-type"></a>mobileAppTroubleshootingAppTargetHistory 资源类型

命名空间：microsoft.graph

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

包含在移动应用疑难解答事件中的历史记录项。


继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|occurrenceDateTime|DateTimeOffset|历史记录项发生的时间。 继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)|
|troubleshootingErrorDetails|[deviceManagementTroubleshootingErrorDetails](../resources/intune-troubleshooting-devicemanagementtroubleshootingerrordetails.md)|包含有关错误及其修正的详细信息的对象。 继承自 [mobileAppTroubleshootingHistoryItem](../resources/intune-troubleshooting-mobileapptroubleshootinghistoryitem.md)|
|securityGroupId|String|面向它的 AAD 安全组 ID。|
|runState|[runState](../resources/intune-troubleshooting-runstate.md)|项目的状态。 可取值为：`unknown`、`success`、`fail`、`scriptError`、`pending`、`notApplicable`。|
|errorCode|String|失败的错误代码，如果没有失败，则为空。|

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
  "troubleshootingErrorDetails": {
    "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorDetails",
    "context": "String",
    "failure": "String",
    "failureDetails": "String",
    "remediation": "String",
    "resources": [
      {
        "@odata.type": "microsoft.graph.deviceManagementTroubleshootingErrorResource",
        "text": "String",
        "link": "String"
      }
    ]
  },
  "securityGroupId": "String",
  "runState": "String",
  "errorCode": "String"
}
```




