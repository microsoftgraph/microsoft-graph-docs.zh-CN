---
title: groupPolicyPresentationDropdownList 资源类型
description: 表示 ADMX dropdownList 元素和 ADMX 枚举元素。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: resourcePageType
ms.openlocfilehash: 9fe4410f0f6d433b62874a5d8ddc6d8ef4e13712
ms.sourcegitcommit: dcf237b515e70302aec0d0c490feb1de7a60613e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/31/2021
ms.locfileid: "58817052"
---
# <a name="grouppolicypresentationdropdownlist-resource-type"></a>groupPolicyPresentationDropdownList 资源类型

命名空间：microsoft.graph

> **重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。

> **注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。

表示 ADMX dropdownList 元素和 ADMX 枚举元素。


继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)

## <a name="methods"></a>方法
|方法|返回类型|Description|
|:---|:---|:---|
|[列出 groupPolicyPresentationDropdownLists](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-list.md)|[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) 集合|列出 [groupPolicyPresentationDropdownList 对象的属性和](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) 关系。|
|[获取 groupPolicyPresentationDropdownList](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-get.md)|[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|读取 [groupPolicyPresentationDropdownList 对象的属性和](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) 关系。|
|[创建 groupPolicyPresentationDropdownList](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-create.md)|[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|创建新的 [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) 对象。|
|[删除 groupPolicyPresentationDropdownList](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-delete.md)|无|删除 [groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)。|
|[更新 groupPolicyPresentationDropdownList](../api/intune-grouppolicy-grouppolicypresentationdropdownlist-update.md)|[groupPolicyPresentationDropdownList](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md)|更新 [groupPolicyPresentationDropdownList 对象](../resources/intune-grouppolicy-grouppolicypresentationdropdownlist.md) 的属性。|

## <a name="properties"></a>属性
|属性|类型|Description|
|:---|:---|:---|
|标签|String|任何演示文稿实体的本地化文本标签。 默认值为空白。 继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|id|String|实体的键。 继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|lastModifiedDateTime|DateTimeOffset|上次修改实体的日期和时间。 继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|
|defaultItem|[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md)|用于标识项目列表默认选项的本地化字符串值。|
|items|[groupPolicyPresentationDropdownListItem](../resources/intune-grouppolicy-grouppolicypresentationdropdownlistitem.md) 集合|表示一组本地化的显示名称及其关联值。|
|必需|Boolean|要求在参数框中输入值。 默认值为 false。|

## <a name="relationships"></a>关系
|关系|类型|Description|
|:---|:---|:---|
|definition|[groupPolicyDefinition](../resources/intune-grouppolicy-grouppolicydefinition.md)|与演示文稿关联的组策略定义。 继承自 [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)|

## <a name="json-representation"></a>JSON 表示形式
下面是资源的 JSON 表示形式。
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownList"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationDropdownList",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)",
  "defaultItem": {
    "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
    "displayName": "String",
    "value": "String"
  },
  "items": [
    {
      "@odata.type": "microsoft.graph.groupPolicyPresentationDropdownListItem",
      "displayName": "String",
      "value": "String"
    }
  ],
  "required": true
}
```



