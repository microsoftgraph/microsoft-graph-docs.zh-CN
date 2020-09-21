---
title: groupPolicyUploadedCategory 资源类型
description: Category 实体存储组策略定义的类别
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 51d9abab7ae3a6e85a1e13e3fb52854f4702ca31
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48030680"
---
# <a name="grouppolicyuploadedcategory-resource-type"></a>groupPolicyUploadedCategory 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

Category 实体存储组策略定义的类别


继承自 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 groupPolicyUploadedCategories](../api/intune-grouppolicy-grouppolicyuploadedcategory-list.md)|[groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) 集合|列出 [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) 对象的属性和关系。|
|[获取 groupPolicyUploadedCategory](../api/intune-grouppolicy-grouppolicyuploadedcategory-get.md)|[groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|读取 [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) 对象的属性和关系。|
|[创建 groupPolicyUploadedCategory](../api/intune-grouppolicy-grouppolicyuploadedcategory-create.md)|[groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|创建新的 [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) 对象。|
|[删除 groupPolicyUploadedCategory](../api/intune-grouppolicy-grouppolicyuploadedcategory-delete.md)|无|删除 [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)。|
|[更新 groupPolicyUploadedCategory](../api/intune-grouppolicy-grouppolicyuploadedcategory-update.md)|[groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md)|更新 [groupPolicyUploadedCategory](../resources/intune-grouppolicy-grouppolicyuploadedcategory.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|从[GroupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)继承的类别的显示名称的字符串 id|
|isRoot|Boolean|定义类别是否是从[GroupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)继承的根类别|
|id|String|实体的键。 继承自 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。 继承自 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|父级|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|继承自[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)的父类别|
|children|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) 集合|继承自[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)的子类别|
|限定|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) 集合|继承自[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)的类别的直接 GroupPolicyDefinition 子级|
|definitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|类别来自[GroupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)继承的定义文件的 id|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyUploadedCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedCategory",
  "displayName": "String",
  "isRoot": true,
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```






