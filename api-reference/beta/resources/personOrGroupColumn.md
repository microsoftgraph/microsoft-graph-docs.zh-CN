---
author: simonhult
description: columnDefinition 资源上的 personOrGroupColumn 指示列值，该值表示从目录中选择的个人或组。
ms.date: 09/11/2017
title: PersonOrGroupColumn
ms.localizationpriority: medium
ms.prod: insights
doc_type: resourcePageType
ms.openlocfilehash: 2e35c461dcec7cac70af8b6591a4fcb251ccc8e2
ms.sourcegitcommit: e5d5095e26dca6f434354a0970e789e94ee6afb0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/22/2022
ms.locfileid: "63720802"
---
# <a name="personorgroupcolumn-resource-type"></a>PersonOrGroupColumn 资源类型

命名空间：microsoft.graph

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

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

| 属性                   | 类型    | 说明                                                                                                        |
| :------------------------- | :------ | :----------------------------------------------------------------------------------------------------------------- |
| **allowMultipleSelection** | boolean | 指示是否可以从源中选择多个值。                                                 |
| **displayAs**              | string  | 如何显示有关所选个人或组的信息。 请参阅下文。                                        |
| **chooseFromType**         | string  | 是否允许仅选择人员，或同时选择人员和组。 必须为 `peopleAndGroups` 或 `peopleOnly` 的其中一个。 |

## <a name="displayas-values"></a>displayAs 值

| 值                         | 说明                                                                                                 |
| :---------------------------- | :---------------------------------------------------------------------------------------------------------- |
| **帐户**                   | 采用原始 SharePoint 编码的人员或组声明字符串（如 `i:0#.f|membership|jane@contoso.com`). |
| **department**                | 人员或组的所在部门。                                                                           |
| **firstName**                 | 人员的名字。                                                                                    |
| **id**                        | 目录中个人或组的 id。                                                             |
| **lastName**                  | 人员的姓氏。                                                                                     |
| **mobilePhone**               | 人员的移动电话号码。                                                                           |
| **name**                      | 人员姓名。                                                                                          |
| **nameWithPictureAndDetails** | 人员姓名，以及他们的照片和其他详细信息。                                          |
| **nameWithPresence**          | 默认值。 人员姓名和状态指示器图标（空闲/忙碌/等）                             |
| **office**                    | 人员的办公室电话。                                                                                 |
| **pictureOnly36x36**          | 人员的照片，采用 36x36 像素的正方形框。                                                         |
| **pictureOnly48x48**          | 人员的照片，采用 48x48 像素的正方形框。                                                         |
| **pictureOnly72x72**          | 人员的照片，采用 72x72 像素的正方形框。                                                         |
| **sipAddress**                | 人员的 sip 地址。                                                                                   |
| **title**                     | 人员在组织中的职务。                                                                     |
| **userName**                  | 人员或组的用户名。                                                                            |
| **workEmail**                 | 人员或组的电子邮件地址。                                                                        |
| **workPhone**                 | 人员的工作电话号码。                                                                             |

注意：可能返回其他 DisplayAs 类型。

<!--
{
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Resources/PersonOrGroupColumn",
  "suppressions": []
}
-->
