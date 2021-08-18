---
title: groupPolicyPresentation 资源类型
description: 用于显示组策略定义中任何其他选项的显示的基本实体。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 281b3ad7d33c0dafbefa810744ac775eaecf05d59b2e673670bab80787f82991
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54253518"
---
# <a name="grouppolicypresentation-resource-type"></a>groupPolicyPresentation 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

用于显示组策略定义中任何其他选项的显示的基本实体。

## <a name="methods"></a>Methods
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 groupPolicyPresentation](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|读取 [groupPolicyPresentation 对象的属性和](../resources/intune-grouppolicy-grouppolicypresentation.md) 关系。|
|[更新 groupPolicyPresentation](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|更新 [groupPolicyPresentation 对象](../resources/intune-grouppolicy-grouppolicypresentation.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|标签|String|任何演示文稿实体的本地化文本标签。 默认值为空白。|
|id|String|实体的键。|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。|

## <a name="relationships"></a>关系
|关系|类型|说明|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|与演示文稿关联的组策略定义。|

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




