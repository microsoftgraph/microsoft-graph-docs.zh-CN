---
title: deviceConfigurationUserStateSummary 资源类型
description: 尚未记录
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 170b84d58d17bfbf8eea7d402c26b78019be3958
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30163019"
---
# <a name="deviceconfigurationuserstatesummary-resource-type"></a>deviceConfigurationUserStateSummary 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

尚未记录

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceConfigurationUserStateSummary](../api/intune-deviceconfig-deviceconfigurationuserstatesummary-get.md)|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|读取[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)对象的属性和关系。|
|[更新 deviceConfigurationUserStateSummary](../api/intune-deviceconfig-deviceconfigurationuserstatesummary-update.md)|[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)|更新[deviceConfigurationUserStateSummary](../resources/intune-deviceconfig-deviceconfigurationuserstatesummary.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的键。|
|unknownUserCount|Int32|未知用户的数量|
|notApplicableUserCount|Int32|不适用的用户数|
|compliantUserCount|Int32|合规用户数|
|remediatedUserCount|Int32|已修正用户的数量|
|nonCompliantUserCount|Int32|不符合的用户数|
|errorUserCount|Int32|错误用户数|
|conflictUserCount|Int32|冲突用户数|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceConfigurationUserStateSummary"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceConfigurationUserStateSummary",
  "id": "String (identifier)",
  "unknownUserCount": 1024,
  "notApplicableUserCount": 1024,
  "compliantUserCount": 1024,
  "remediatedUserCount": 1024,
  "nonCompliantUserCount": 1024,
  "errorUserCount": 1024,
  "conflictUserCount": 1024
}
```




