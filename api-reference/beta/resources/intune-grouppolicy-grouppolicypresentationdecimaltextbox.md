---
title: groupPolicyPresentationDecimalTextBox 资源类型
description: 表示 ADMX decimalTextBox 元素和 ADMX 十进制元素。
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 4125cb9a3ad81504271a02f2336c274e0a550e57
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59086008"
---
# <a name="grouppolicypresentationdecimaltextbox-resource-type"></a>groupPolicyPresentationDecimalTextBox 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 ADMX decimalTextBox 元素和 ADMX 十进制元素。


继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 groupPolicyPresentationDecimalTextBoxes](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-list.md)|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) 集合|列出 [groupPolicyPresentationDecimalTextBox 对象的属性和](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) 关系。|
|[获取 groupPolicyPresentationDecimalTextBox](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-get.md)|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|读取 [groupPolicyPresentationDecimalTextBox 对象的属性和](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) 关系。|
|[创建 groupPolicyPresentationDecimalTextBox](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-create.md)|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|创建新的 [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) 对象。|
|[删除 groupPolicyPresentationDecimalTextBox](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-delete.md)|无|删除 [groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)。|
|[更新 groupPolicyPresentationDecimalTextBox](../api/intune-grouppolicy-grouppolicypresentationdecimaltextbox-update.md)|[groupPolicyPresentationDecimalTextBox](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md)|更新 [groupPolicyPresentationDecimalTextBox 对象](../resources/intune-grouppolicy-grouppolicypresentationdecimaltextbox.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|标签|String|任何演示文稿实体的本地化文本标签。 默认值为空白。 继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|实体的键。 继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。 继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultValue|Int64|一个无符号整数，指定小数文本框的初始值。 默认值为 1。|
|spin|Boolean|如果为 true，则创建旋转控件;否则，为数字输入创建一个文本框。 默认值为 true。|
|spinStep|Int64|一个无符号整数，指定旋转控件更改的增量。 默认值为 1。|
|必需|Boolean|要求在参数框中输入值。 默认值为 false。|
|minValue|Int64|一个无符号整数，指定允许的最小值。 默认值为 0。|
|maxValue|Int64|一个无符号整数，指定允许的最大值。 默认值为 9999。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|与演示文稿关联的组策略定义。 继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationDecimalTextBox"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDecimalTextBox",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultValue": 1024,
  "spin": true,
  "spinStep": 1024,
  "required": true,
  "minValue": 1024,
  "maxValue": 1024
}
```



