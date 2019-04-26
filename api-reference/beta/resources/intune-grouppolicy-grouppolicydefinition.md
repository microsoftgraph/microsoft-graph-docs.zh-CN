---
title: groupPolicyDefinition 资源类型
description: 实体描述有关单个组策略的所有信息。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a9e411c2672650e3e603bfa0e64fde1c4db53607
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32575770"
---
# <a name="grouppolicydefinition-resource-type"></a>groupPolicyDefinition 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

实体描述有关单个组策略的所有信息。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 groupPolicyDefinition](../api/intune-grouppolicy-grouppolicydefinition-get.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|读取[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)对象的属性和关系。|
|[更新 groupPolicyDefinition](../api/intune-grouppolicy-grouppolicydefinition-update.md)|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|更新[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|classType|[groupPolicyDefinitionClassType](../resources/intune-grouppolicy-grouppolicydefinitionclasstype.md)|标识策略可应用于的组的类型。 可取值为：`user`、`machine`。|
|displayName|String|本地化策略名称。|
|explainText|String|与策略关联的本地化说明或帮助文本。 默认值为空白。|
|categoryPath|String|策略的本地化完整类别路径。|
|supportedOn|String|用于指定受策略影响的操作系统或应用程序版本的本地化字符串。|
|policyType|[groupPolicyType](../resources/intune-grouppolicy-grouppolicytype.md)|指定组策略的类型。 可能的值是：`admxBacked`、`admxIngested`。|
|id|String|实体的键。|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|definitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|与定义关联的组策略文件。|
|文稿|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)集合|与定义关联的组策略演示文稿。|

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





