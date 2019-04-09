---
title: deviceManagementIntentUserStateSummary 资源类型
description: 表示意向的用户状态摘要的实体
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c930b19e604aaf3867260e359a2b7fcb12153762
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31523992"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a>deviceManagementIntentUserStateSummary 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示意向的用户状态摘要的实体

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceManagementIntentUserStateSummary](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|读取[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象的属性和关系。|
|[更新 deviceManagementIntentUserStateSummary](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|更新[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|ID|
|conflictCount|Int32|发生冲突的用户数|
|errorCount|Int32|错误用户数|
|failedCount|Int32|失败的用户数|
|notApplicableCount|Int32|不适用的用户数|
|successCount|Int32|成功的用户数|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentUserStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserStateSummary",
  "id": "String (identifier)",
  "conflictCount": 1024,
  "errorCount": 1024,
  "failedCount": 1024,
  "notApplicableCount": 1024,
  "successCount": 1024
}
```







