---
title: groupPolicyPresentation 资源类型
description: 组策略定义中任何其他选项的显示演示文稿的基本实体。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1d6abbcde241059a15969236b3ab7bcb0825d67d
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166876"
---
# <a name="grouppolicypresentation-resource-type"></a>groupPolicyPresentation 资源类型

> **重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。

> **注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

组策略定义中任何其他选项的显示演示文稿的基本实体。

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 groupPolicyPresentation](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|读取[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)对象的属性和关系。|
|[更新 groupPolicyPresentation](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|更新[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)对象的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|标签|字符串|任何演示文稿实体的本地化文本标签。 默认值为空。|
|id|String|实体的键。|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|与演示文稿相关联的组策略定义。|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```




