---
author: simonhult
ms.date: 09/11/2017
title: PersonOrGroupColumn
localization_priority: Normal
ms.prod: insights
description: columnDefinition 资源上的 personOrGroupColumn 指示列值，该值表示从目录中选择的个人或组。
doc_type: resourcePageType
ms.openlocfilehash: 728d9244a08d893eacc53f01106d07a952f536f5ea978a03584ed41d3151c3c1
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54196920"
---
# <a name="personorgroupcolumn-resource-type"></a>PersonOrGroupColumn 资源类型

命名空间：microsoft.graph

[columnDefinition](columndefinition.md) 资源上的 **personOrGroupColumn** 指示列值，该值表示从目录中选择的个人或组。

## <a name="json-representation"></a>JSON 表示形式

下面是 **personOrGroupColumn** 资源的 JSON 表示形式。
<!-- { "blockType": "resource", "@type": "microsoft.graph.personOrGroupColumn", "@property.aka": "chooseFromType=format" } -->

```json
{
  "allowMultipleSelection": true,
  "displayAs": "account | contentType | created | department | ...",
  "chooseFromType": "peopleAndGroups | peopleOnly"
}
```

## <a name="properties"></a>属性

| 属性名称              | 类型    | 说明
|:---------------------------|:--------|:--------------------------------------
| **allowMultipleSelection** | boolean | 指示是否可以从源中选择多个值。
| **displayAs**              | string  | 如何显示有关所选个人或组的信息。 请参阅下文。
| **chooseFromType**         | string  | 是否允许仅选择人员，或同时选择人员和组。 必须为 `peopleAndGroups` 或 `peopleOnly` 的其中一个。

## <a name="displayas-options"></a>DisplayAs 选项

| DisplayAs 值               | 说明
|:------------------------------|:-----------------------
| **帐户**                   | 采用原始 SharePoint 编码的人员或组声明字符串（如 `i:0#.f|membership|jane@contoso.com`).
| **department**                | 人员或组的所在部门。
| **firstName**                 | 人员的名字。
| **id**                        | 目录中个人或组的 id。
| **lastName**                  | 人员的姓氏。
| **mobilePhone**               | 人员的移动电话号码。
| **name**                      | 人员姓名。
| **nameWithPictureAndDetails** | 人员姓名，以及他们的照片和其他详细信息。
| **nameWithPresence**          | 默认值。 人员姓名和状态指示器图标（空闲/忙碌/等）
| **office**                    | 人员的办公室电话。
| **pictureOnly36x36**          | 人员的照片，采用 36x36 像素的正方形框。
| **pictureOnly48x48**          | 人员的照片，采用 48x48 像素的正方形框。
| **pictureOnly72x72**          | 人员的照片，采用 72x72 像素的正方形框。
| **sipAddress**                | 人员的 sip 地址。
| **title**                     | 人员在组织中的职务。
| **userName**                  | 人员或组的用户名。
| **workEmail**                 | 人员或组的电子邮件地址。
| **workPhone**                 | 人员的工作电话号码。

注意：可能返回其他 DisplayAs 类型。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "suppressions": [
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(peopleAndGroups,peopleOnly) are in resource, but () are in table",
    "Warning: /api-reference/v1.0/resources/personorgroupcolumn.md:
      Found potential enums in resource example that weren't defined in a table:(account,contentType,created,department,...) are in resource, but () are in table"
  ],
  "tocPath": "Resources/PersonOrGroupColumn"
} -->

