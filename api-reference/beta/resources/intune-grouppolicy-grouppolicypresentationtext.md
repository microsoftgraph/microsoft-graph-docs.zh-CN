---
title: groupPolicyPresentationText 资源类型
description: 表示 ADMX 文本元素。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2021108ef033e1529911de57be24612935896d22
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30142859"
---
# <a name="grouppolicypresentationtext-resource-type"></a>groupPolicyPresentationText 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 ADMX 文本元素。


继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[列出 groupPolicyPresentationTexts](../api/intune-grouppolicy-grouppolicypresentationtext-list.md)|[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)集合|列出[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)对象的属性和关系。|
|[获取 groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-get.md)|[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|读取[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)对象的属性和关系。|
|[创建 groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-create.md)|[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|创建新的[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)对象。|
|[删除 groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-delete.md)|无|删除[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)。|
|[更新 groupPolicyPresentationText](../api/intune-grouppolicy-grouppolicypresentationtext-update.md)|[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)|更新[groupPolicyPresentationText](../resources/intune-grouppolicy-grouppolicypresentationtext.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|标签|字符串|任何演示文稿实体的本地化文本标签。 默认值为空。 继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|实体的键。 继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。 继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|与演示文稿相关联的组策略定义。 继承自[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationText"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationText",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




