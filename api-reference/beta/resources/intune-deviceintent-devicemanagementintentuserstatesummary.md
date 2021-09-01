---
title: deviceManagementIntentUserStateSummary 资源类型
description: 表示意图的用户状态摘要的实体
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: ae189dbf5d5287e3123696c66cc433c41be174cc
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58790379"
---
# <a name="devicemanagementintentuserstatesummary-resource-type"></a>deviceManagementIntentUserStateSummary 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示意图的用户状态摘要的实体

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 deviceManagementIntentUserStateSummary](../api/intune-deviceintent-devicemanagementintentuserstatesummary-get.md)|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|读取 [deviceManagementIntentUserStateSummary 对象的属性和](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) 关系。|
|[更新 deviceManagementIntentUserStateSummary](../api/intune-deviceintent-devicemanagementintentuserstatesummary-update.md)|[deviceManagementIntentUserStateSummary](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md)|更新 [deviceManagementIntentUserStateSummary 对象](../resources/intune-deviceintent-devicemanagementintentuserstatesummary.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|The ID|
|conflictCount|Int32|发生冲突的用户数|
|errorCount|Int32|错误用户数|
|failedCount|Int32|失败用户数|
|notApplicableCount|Int32|不适用用户的数量|
|successCount|Int32|成功用户数|

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



