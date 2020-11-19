---
title: groupPolicyDefinition 资源类型
description: 实体描述有关单个组策略的所有信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 2b7a2317927e9c486d105df01cd78001de7a0c66
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49298552"
---
# <a name="grouppolicydefinition-resource-type"></a>groupPolicyDefinition 资源类型

命名空间：microsoft.graph

> **重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

实体描述有关单个组策略的所有信息。

## <a name="methods"></a>Methods
|方法|返回类型|Description|
|:---|:---|:---|
|[获取 groupPolicyDefinition](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|读取 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) 对象的属性和关系。|
|[更新 groupPolicyDefinition](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|更新 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) 对象的属性。|

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|classType|[groupPolicyDefinitionClassType](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|标识策略可应用于的组的类型。 可取值为：`user`、`machine`。|
|displayName|字符串|本地化策略名称。|
|explainText|字符串|与策略关联的本地化说明或帮助文本。 默认值为空白。|
|categoryPath|字符串|策略的本地化完整类别路径。|
|supportedOn|字符串|用于指定受策略影响的操作系统或应用程序版本的本地化字符串。|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|指定组策略的类型。 可取值为：`admxBacked`、`admxIngested`。|
|groupPolicyCategoryId|Guid|父类别的类别 id|
|id|字符串|实体的键。|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|definitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|与定义关联的组策略文件。|
|“类别”|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|与定义关联的组策略类别。|
|文稿|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) 集合|与定义关联的组策略演示文稿。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyDefinition"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyDefinition",
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




