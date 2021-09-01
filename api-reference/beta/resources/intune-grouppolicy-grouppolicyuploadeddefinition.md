---
title: groupPolicyUploadedDefinition 资源类型
description: 实体描述有关单个组策略的所有信息。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 268259e11f71396fc89321f3bb09d18b71475276
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58806024"
---
# <a name="grouppolicyuploadeddefinition-resource-type"></a>groupPolicyUploadedDefinition 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

实体描述有关单个组策略的所有信息。


继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 groupPolicyUploadedDefinitions](../api/intune-grouppolicy-grouppolicyuploadeddefinition-list.md)|[groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 集合|列出 [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 对象的属性和关系。|
|[获取 groupPolicyUploadedDefinition](../api/intune-grouppolicy-grouppolicyuploadeddefinition-get.md)|[groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)|读取 [groupPolicyUploadedDefinition 对象的属性和](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 关系。|
|[创建 groupPolicyUploadedDefinition](../api/intune-grouppolicy-grouppolicyuploadeddefinition-create.md)|[groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)|创建新的 [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 对象。|
|[删除 groupPolicyUploadedDefinition](../api/intune-grouppolicy-grouppolicyuploadeddefinition-delete.md)|无|删除 [groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)。|
|[更新 groupPolicyUploadedDefinition](../api/intune-grouppolicy-grouppolicyuploadeddefinition-update.md)|[groupPolicyUploadedDefinition](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md)|更新 [groupPolicyUploadedDefinition 对象](../resources/intune-grouppolicy-grouppolicyuploadeddefinition.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|classType|[groupPolicyDefinitionClassType](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|标识策略可应用于的组类型。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)。 可取值为：`user`、`machine`。|
|displayName|String|本地化的策略名称。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|explainText|String|与策略关联的本地化说明或帮助文本。 默认值为空白。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|categoryPath|String|策略的本地化完整类别路径。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|supportedOn|String|用于指定受策略影响的操作系统或应用程序版本的本地化字符串。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|指定组策略的类型。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)。 可取值为：`admxBacked`、`admxIngested`。|
|hasRelatedDefinitions|布尔值|表示此定义是否有相关定义 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|groupPolicyCategoryId|Guid|父类别的类别 ID 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|minDeviceCspVersion|字符串|此定义中设备配置所需的最低 CSP 版本 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|minUserCspVersion|字符串|此定义中用户配置所需的最低 CSP 版本 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|version|String|设置定义版本 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|id|String|实体的键。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|definitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|与定义关联的组策略文件。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|“类别”|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|与定义关联的组策略类别。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|演示文稿|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) 集合|与定义关联的组策略演示文稿。 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|previousVersionDefinition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|此定义的早期版本的定义 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|
|nextVersionDefinition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|此定义的下一版本的定义 继承自 [groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|

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
  "hasRelatedDefinitions": true,
  "groupPolicyCategoryId": "Guid",
  "minDeviceCspVersion": "String",
  "minUserCspVersion": "String",
  "version": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



