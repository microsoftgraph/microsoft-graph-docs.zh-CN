---
title: deviceManagementIntentUserState 资源类型
description: 表示意向的用户状态的实体
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 1ad8fe7e61f883bae43522a0aaafecacaf090be0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36371360"
---
# <a name="devicemanagementintentuserstate-resource-type"></a>deviceManagementIntentUserState 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示意向的用户状态的实体

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementIntentUserStates](../api/intune-deviceintent-devicemanagementintentuserstate-list.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)集合|列出[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)对象的属性和关系。|
|[获取 deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-get.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|读取[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)对象的属性和关系。|
|[创建 deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-create.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|创建新的[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)对象。|
|[删除 deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-delete.md)|无|删除[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)。|
|[更新 deviceManagementIntentUserState](../api/intune-deviceintent-devicemanagementintentuserstate-update.md)|[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)|更新[deviceManagementIntentUserState](../resources/intune-deviceintent-devicemanagementintentuserstate.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|ID|
|userPrincipalName|String|在设备上报告的用户主体名称|
|userName|String|在设备上报告的用户名|
|deviceCount|Int32|属于某个意图的用户的设备计数|
|lastReportedDateTime|DateTimeOffset|意向报表的上次修改日期时间|
|state|[complianceStatus](../resources/intune-shared-compliancestatus.md)|意图的用户状态。 可取值为：`unknown`、`notApplicable`、`compliant`、`remediated`、`nonCompliant`、`error`、`conflict`、`notAssigned`。|

## <a name="relationships"></a>关系
无

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementIntentUserState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementIntentUserState",
  "id": "String (identifier)",
  "userPrincipalName": "String",
  "userName": "String",
  "deviceCount": 1024,
  "lastReportedDateTime": "String (timestamp)",
  "state": "String"
}
```



