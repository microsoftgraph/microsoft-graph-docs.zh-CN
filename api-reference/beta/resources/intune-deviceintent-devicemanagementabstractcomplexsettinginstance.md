---
title: deviceManagementAbstractComplexSettingInstance 资源类型
description: 一个代表抽象设置的复杂值的设置实例
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bb835db6d1d97cb4a72e8b68e0a45e6bf33728aa
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2019
ms.locfileid: "31524111"
---
# <a name="devicemanagementabstractcomplexsettinginstance-resource-type"></a>deviceManagementAbstractComplexSettingInstance 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

一个代表抽象设置的复杂值的设置实例


继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 deviceManagementAbstractComplexSettingInstances](../api/intune-deviceintent-devicemanagementabstractcomplexsettinginstance-list.md)|[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)集合|列出[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)对象的属性和关系。|
|[获取 deviceManagementAbstractComplexSettingInstance](../api/intune-deviceintent-devicemanagementabstractcomplexsettinginstance-get.md)|[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)|读取[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)对象的属性和关系。|
|[创建 deviceManagementAbstractComplexSettingInstance](../api/intune-deviceintent-devicemanagementabstractcomplexsettinginstance-create.md)|[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)|创建新的[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)对象。|
|[删除 deviceManagementAbstractComplexSettingInstance](../api/intune-deviceintent-devicemanagementabstractcomplexsettinginstance-delete.md)|无|删除[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)。|
|[更新 deviceManagementAbstractComplexSettingInstance](../api/intune-deviceintent-devicemanagementabstractcomplexsettinginstance-update.md)|[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)|更新[deviceManagementAbstractComplexSettingInstance](../resources/intune-deviceintent-devicemanagementabstractcomplexsettinginstance.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|id|String|从[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)继承的设置实例 ID|
|definitionId|String|继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的此实例的设置定义 ID|
|valueJson|String|继承自[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)的值的 JSON 表示形式|
|implementationId|String|此复杂设置的所选实现的定义 ID|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|value|[deviceManagementSettingInstance](../resources/intune-deviceintent-devicemanagementsettinginstance.md)集合|构成复杂设置的值|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.deviceManagementAbstractComplexSettingInstance"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceManagementAbstractComplexSettingInstance",
  "id": "String (identifier)",
  "definitionId": "String",
  "valueJson": "String",
  "implementationId": "String"
}
```







