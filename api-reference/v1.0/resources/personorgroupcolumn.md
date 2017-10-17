---
author: rgregg
ms.author: rgregg
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.openlocfilehash: 715c6ca22957cbd951784e6cf32edf2bf47f1098
ms.sourcegitcommit: 7aea7a97e36e6d146214de3a90fdbc71628aadba
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/28/2017
---
# <a name="personorgroupcolumn-resource-type"></a>PersonOrGroupColumn 资源类型

[columnDefinition](columnDefinition.md) 资源上的 **personOrGroupColumn** 指示列值表示从目录中选择的个人或组。

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
| **chooseFromType**         | string  | 是否允许仅选择人员，或人员和组。 必须是 `peopleAndGroups` 或 `peopleOnly` 的其中一个。

## <a name="displayas-values"></a>DisplayAs 值

| DisplayAs 值               | 说明
|:------------------------------|:-----------------------
| **account**                   | 个人或组的原始 SharePoint 编码的声明字符串（如 i:0#.f|membership|jane@contoso.com）。
| **department**                | 个人或组所在的部门。
| **firstName**                 | 个人的名字。
| **id**                        | 目录中个人或组的 ID。
| **lastName**                  | 个人的姓氏。
| **mobilePhone**               | 个人的移动电话号码。
| **name**                      | 个人的名称。
| **nameWithPictureAndDetails** | 个人的姓名及其照片和其他详细信息。
| **nameWithPresence**          | 默认值。 带有状态指示器图标（空闲/忙碌等）的个人名称
| **office**                    | 个人的办公室号码。
| **pictureOnly36x36**          | 个人的照片，采用 36x36 像素的正方形边框。
| **pictureOnly48x48**          | 个人的照片，采用 48x48 像素的正方形边框。
| **pictureOnly72x72**          | 个人的照片，采用 72x72 像素的正方形边框。
| **sipAddress**                | 个人的 SIP 地址。
| **title**                     | 组织中的个人头衔。
| **userName**                  | 个人或组的用户名。
| **workEmail**                 | 个人或组的电子邮件地址。
| **workPhone**                 | 个人的工作电话号码。

注意：可能返回其他 DisplayAs 类型。

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn"
} -->
