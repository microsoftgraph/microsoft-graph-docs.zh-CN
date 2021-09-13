---
title: groupPolicyCategory 资源类型
description: 类别实体存储组策略定义的类别
author: dougeby
ms.localizationpriority: medium
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: bd728c056576e31b37a4c105c62186f97e789fa1
ms.sourcegitcommit: 6c04234af08efce558e9bf926062b4686a84f1b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/12/2021
ms.locfileid: "59080959"
---
# <a name="grouppolicycategory-resource-type"></a>groupPolicyCategory 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

类别实体存储组策略定义的类别

## <a name="methods"></a>方法
|方法|返回类型|说明|
|:---|:---|:---|
|[获取 groupPolicyCategory](../api/intune-grouppolicy-grouppolicycategory-get.md)|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|读取 [groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) 对象的属性和关系。|
|[更新 groupPolicyCategory](../api/intune-grouppolicy-grouppolicycategory-update.md)|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|更新 [groupPolicyCategory 对象](../resources/intune-grouppolicy-grouppolicycategory.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|说明|
|:---|:---|:---|
|displayName|String|类别名称的字符串显示名称|
|isRoot|Boolean|定义类别是否属于根类别|
|id|String|实体的键。|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。|

## <a name="relationships"></a>关系
|关系|类型|描述|
|:---|:---|:---|
|父级|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md)|父类别|
|children|[groupPolicyCategory](../resources/intune-grouppolicy-grouppolicycategory.md) 集合|子类别|
|定义|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md) 集合|类别的直接 GroupPolicyDefinition 子级|
|definitionFile|[groupPolicyDefinitionFile](../resources/intune-grouppolicy-grouppolicydefinitionfile.md)|类别来自的定义文件的 ID|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyCategory"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyCategory",
  "displayName": "String",
  "isRoot": true,
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



