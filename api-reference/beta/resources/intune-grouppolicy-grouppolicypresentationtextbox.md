---
title: groupPolicyPresentationTextBox 资源类型
description: 表示 ADMX textBox 元素和 ADMX 文本元素。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: a3319960f8f15f06816eaa6a5ec2879352255c41
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58793307"
---
# <a name="grouppolicypresentationtextbox-resource-type"></a>groupPolicyPresentationTextBox 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 ADMX textBox 元素和 ADMX 文本元素。


继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 groupPolicyPresentationTextBoxes](../api/intune-grouppolicy-grouppolicypresentationtextbox-list.md)|[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) 集合|列出 [groupPolicyPresentationTextBox 对象的属性和](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) 关系。|
|[获取 groupPolicyPresentationTextBox](../api/intune-grouppolicy-grouppolicypresentationtextbox-get.md)|[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|读取 [groupPolicyPresentationTextBox 对象的属性和](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) 关系。|
|[创建 groupPolicyPresentationTextBox](../api/intune-grouppolicy-grouppolicypresentationtextbox-create.md)|[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|创建新的 [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) 对象。|
|[删除 groupPolicyPresentationTextBox](../api/intune-grouppolicy-grouppolicypresentationtextbox-delete.md)|无|删除 [groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)。|
|[更新 groupPolicyPresentationTextBox](../api/intune-grouppolicy-grouppolicypresentationtextbox-update.md)|[groupPolicyPresentationTextBox](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md)|更新 [groupPolicyPresentationTextBox 对象](../resources/intune-grouppolicy-grouppolicypresentationtextbox.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|标签|String|任何演示文稿实体的本地化文本标签。 默认值为空白。 继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|实体的键。 继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。 继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultValue|字符串|文本框中显示的本地化默认字符串。 默认值为空白。|
|必需|布尔值|要求在文本框中输入值。 默认值为 false。|
|maxLength|Int64|一个无符号整数，指定最大文本字符数。 默认值为 1023。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|与演示文稿关联的组策略定义。 继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationTextBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultValue": "String",
  "required": true,
  "maxLength": 1024
}
```



