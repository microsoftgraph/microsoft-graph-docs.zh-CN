---
title: groupPolicyUploadedDefinition 资源类型
description: 实体描述有关单个组策略的所有信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: c37642443f7179f3fe215e7c5757634b0c9440c1
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298230"
---
# <a name="grouppolicyuploadeddefinition-resource-type"></a>groupPolicyUploadedDefinition 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

实体描述有关单个组策略的所有信息。


继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 groupPolicyUploadedDefinitions](../api/intune-grouppolicy-grouppolicyuploadeddefinition-list.md)|[groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 集合|列出 [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 对象的属性和关系。|
|[获取 groupPolicyUploadedDefinition](../api/intune-grouppolicy-grouppolicyuploadeddefinition-get.md)|[groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)|读取 [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 对象的属性和关系。|
|[创建 groupPolicyUploadedDefinition](../api/intune-grouppolicy-grouppolicyuploadeddefinition-create.md)|[groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)|创建新的 [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 对象。|
|[删除 groupPolicyUploadedDefinition](../api/intune-grouppolicy-grouppolicyuploadeddefinition-delete.md)|无|删除 [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)。|
|[更新 groupPolicyUploadedDefinition](../api/intune-grouppolicy-grouppolicyuploadeddefinition-update.md)|[groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)|更新 [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|classType|[groupPolicyDefinitionClassType](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|标识策略可应用于的组的类型。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)。 可取值为：`user`、`machine`。|
|displayName|字符串|本地化策略名称。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|explainText|字符串|与策略关联的本地化说明或帮助文本。 默认值为空白。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|categoryPath|字符串|策略的本地化完整类别路径。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|supportedOn|字符串|用于指定受策略影响的操作系统或应用程序版本的本地化字符串。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|指定组策略的类型。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)。 可取值为：`admxBacked`、`admxIngested`。|
|groupPolicyCategoryId|Guid|继承自[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)的父类别的类别 id|
|id|字符串|实体的键。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|definitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|与定义关联的组策略文件。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|“类别”|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|与定义关联的组策略类别。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|文稿|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) 集合|与定义关联的组策略演示文稿。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyUploadedDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyUploadedDefinition",
  "classType": "String",
  "displayName": "String",
  "explainText": "String",
  "categoryPath": "String",
  "supportedOn": "String",
  "policyType": "String",
  "groupPolicyCategoryId": "Guid",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




