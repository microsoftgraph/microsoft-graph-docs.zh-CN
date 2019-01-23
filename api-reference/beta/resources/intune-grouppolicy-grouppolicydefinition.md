---
title: groupPolicyDefinition 资源类型
description: 实体描述所有单个组策略的信息。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 502312f7a39dd5dc93fd8e39203f56d47a9ebf27
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429519"
---
# <a name="grouppolicydefinition-resource-type"></a>groupPolicyDefinition 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

实体描述所有单个组策略的信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 groupPolicyDefinition](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|读取属性和[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)对象的关系。|
|[更新 groupPolicyDefinition](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|更新[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|classType|[groupPolicyDefinitionClassType](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|标识的组策略可应用于的类型。 可取值为：`user`、`machine`、`both`。|
|displayName|String|本地化的策略名称。|
|explainText|String|本地化的说明或帮助文本与策略相关联。 默认值为空。|
|categoryPath|String|本地化的完整类别策略路径。|
|supportedOn|String|用于指定哪些操作系统或应用程序版本的本地化的字符串受策略。|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|指定的组策略的类型。 可取值为：`admxBacked`、`admxIngested`。|
|id|String|实体的键。|
|lastModifiedDateTime|DateTimeOffset|日期和实体上次修改的时间。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|definitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|组策略文件与定义关联。|
|演示文稿|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)集合|与定义关联组策略演示文稿。|

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
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




