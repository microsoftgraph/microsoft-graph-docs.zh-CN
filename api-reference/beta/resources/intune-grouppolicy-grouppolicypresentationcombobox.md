---
title: groupPolicyPresentationComboBox 资源类型
description: 代表 ADMX comboBox 元素和 ADMX 文本元素。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 2225cda293bd2966dd39347dfe1ed03b2a4137c4
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29431347"
---
# <a name="grouppolicypresentationcombobox-resource-type"></a>groupPolicyPresentationComboBox 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

代表 ADMX comboBox 元素和 ADMX 文本元素。


继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 groupPolicyPresentationComboBoxes](../api/intune-grouppolicy-grouppolicypresentationcombobox-list.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)集合|列出属性和[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象之间的关系。|
|[获取 groupPolicyPresentationComboBox](../api/intune-grouppolicy-grouppolicypresentationcombobox-get.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|读取属性和[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象的关系。|
|[创建 groupPolicyPresentationComboBox](../api/intune-grouppolicy-grouppolicypresentationcombobox-create.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|创建新的[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象。|
|[删除 groupPolicyPresentationComboBox](../api/intune-grouppolicy-grouppolicypresentationcombobox-delete.md)|无|删除[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)。|
|[更新 groupPolicyPresentationComboBox](../api/intune-grouppolicy-grouppolicypresentationcombobox-update.md)|[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)|更新[groupPolicyPresentationComboBox](../resources/intune-grouppolicy-grouppolicypresentationcombobox.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|标签|String|任何演示文稿实体的本地化的文本标签。 默认值为空。 继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|实体的键。 继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|日期和实体上次修改的时间。 继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultValue|字符串|本地化的组合框中显示的默认字符串。 默认值为空。|
|建议|String 集合|组合框下拉列表中列出的本地化的字符串。 默认值为空。|
|必需|Boolean|指定是否必须参数指定一个值。 默认值为 false。|
|maxLength|Int64|指定的参数的文本字符的最大数量无符号的整数。 默认值是 1023年。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|随演示文稿相关联的组策略定义。 继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationComboBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationComboBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultValue": "String",
  "suggestions": [
    "String"
  ],
  "required": true,
  "maxLength": 1024
}
```




