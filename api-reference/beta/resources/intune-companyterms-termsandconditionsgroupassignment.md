---
title: termsAndConditionsGroupAssignment 资源类型
description: TermsAndConditionsGroupAssignment 实体表示分配给给定组的给定条款和条件 (T&C) 策略。 组中的用户需要接受这些条款，才能将设备注册到 Intune。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 417871f610e9c278e902b41c020c1d8fd904eb6a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33949135"
---
# <a name="termsandconditionsgroupassignment-resource-type"></a>termsAndConditionsGroupAssignment 资源类型

> **重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

TermsAndConditionsGroupAssignment 实体表示分配给给定组的给定条款和条件 (T&C) 策略。 组中的用户需要接受这些条款，才能将设备注册到 Intune。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 termsAndConditionsGroupAssignments](../api/intune-companyterms-termsandconditionsgroupassignment-list.md)|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)集合|列出[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的属性和关系。|
|[获取 termsAndConditionsGroupAssignment](../api/intune-companyterms-termsandconditionsgroupassignment-get.md)|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|读取[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的属性和关系。|
|[创建 termsAndConditionsGroupAssignment](../api/intune-companyterms-termsandconditionsgroupassignment-create.md)|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|创建新的[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象。|
|[删除 termsAndConditionsGroupAssignment](../api/intune-companyterms-termsandconditionsgroupassignment-delete.md)|无|删除[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)。|
|[更新 termsAndConditionsGroupAssignment](../api/intune-companyterms-termsandconditionsgroupassignment-update.md)|[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)|更新[termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|实体的唯一标识符。|
|targetGroupId|String|向其分配 T&C 策略的组的唯一标识符。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|termsAndConditions|[termsAndConditions](../resources/intune-companyterms-termsandconditions.md)|所分配的条款和条件的导航链接。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.termsAndConditionsGroupAssignment"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "String (identifier)",
  "targetGroupId": "String"
}
```




