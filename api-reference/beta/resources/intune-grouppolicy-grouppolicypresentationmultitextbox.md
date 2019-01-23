---
title: groupPolicyPresentationMultiTextBox 资源类型
description: 代表 ADMX multiTextBox 元素和 ADMX multiText 元素。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 85253b6a1af70e75dcba3849fc06dc50935de306
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429392"
---
# <a name="grouppolicypresentationmultitextbox-resource-type"></a>groupPolicyPresentationMultiTextBox 资源类型

> **重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。 不支持在生产应用程序中使用这些 API。

> **注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

代表 ADMX multiTextBox 元素和 ADMX multiText 元素。


继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列表 groupPolicyPresentationMultiTextBoxes](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-list.md)|[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)集合|列出属性和[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)对象之间的关系。|
|[获取 groupPolicyPresentationMultiTextBox](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-get.md)|[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|读取属性和[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)对象的关系。|
|[创建 groupPolicyPresentationMultiTextBox](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-create.md)|[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|创建新的[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)对象。|
|[删除 groupPolicyPresentationMultiTextBox](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-delete.md)|无|删除[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)。|
|[更新 groupPolicyPresentationMultiTextBox](../api/intune-grouppolicy-grouppolicypresentationmultitextbox-update.md)|[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)|更新[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|标签|String|任何演示文稿实体的本地化的文本标签。 默认值为空。 继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|实体的键。 继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|日期和实体上次修改的时间。 继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|必需|Boolean|在文本框中输入值的要求。 默认值为 false。|
|maxLength|Int64|指定的文本字符的最大数量无符号的整数。 默认值为 1023年。|
|maxStrings|Int64|无符号的整数，指定字符串的最大数量。 默认值为 0。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|随演示文稿相关联的组策略定义。 继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationMultiTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "required": true,
  "maxLength": 1024,
  "maxStrings": 1024
}
```




