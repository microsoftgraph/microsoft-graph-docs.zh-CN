---
title: educationAssignmentIndividualRecipient 资源类型
description: '在 assignTo 属性中使用。 当设置为 "单个收件人列表" 时, 课程中的 "选定学生" 将 '
localization_priority: Normal
author: dipakboyed
ms.prod: education
ms.openlocfilehash: 736345901faeeb4d3fab4d417752b684f1e19307
ms.sourcegitcommit: 3410e1b8dcf62a7b0e4d6b11920912479f21feb2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/26/2019
ms.locfileid: "30799989"
---
# <a name="educationassignmentindividualrecipient-resource-type"></a><span data-ttu-id="577db-104">educationAssignmentIndividualRecipient 资源类型</span><span class="sxs-lookup"><span data-stu-id="577db-104">educationAssignmentIndividualRecipient resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="577db-105">在[assignTo](educationassignment.md)属性中使用。</span><span class="sxs-lookup"><span data-stu-id="577db-105">Used inside the [assignment.assignTo](educationassignment.md) property.</span></span> <span data-ttu-id="577db-106">如果设置为 "单个收件人列表", 则在发布工作分配时, 类中的所选学生将收到提交对象。</span><span class="sxs-lookup"><span data-stu-id="577db-106">When set to individual recipient list, selected students in the class will receive a submission object when the assignment is published.</span></span>

<span data-ttu-id="577db-107">此资源是[educationAssignmentRecipient](educationassignmentrecipient.md)的子类。</span><span class="sxs-lookup"><span data-stu-id="577db-107">This resource is a subclass of [educationAssignmentRecipient](educationassignmentrecipient.md).</span></span>

## <a name="properties"></a><span data-ttu-id="577db-108">属性</span><span class="sxs-lookup"><span data-stu-id="577db-108">Properties</span></span>
| <span data-ttu-id="577db-109">属性</span><span class="sxs-lookup"><span data-stu-id="577db-109">Property</span></span>     | <span data-ttu-id="577db-110">类型</span><span class="sxs-lookup"><span data-stu-id="577db-110">Type</span></span>   |<span data-ttu-id="577db-111">说明</span><span class="sxs-lookup"><span data-stu-id="577db-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="577db-112">recipients</span><span class="sxs-lookup"><span data-stu-id="577db-112">recipients</span></span>|<span data-ttu-id="577db-113">String collection</span><span class="sxs-lookup"><span data-stu-id="577db-113">String collection</span></span>|<span data-ttu-id="577db-114">收件人的 id 的集合。</span><span class="sxs-lookup"><span data-stu-id="577db-114">A collection of ids of the recipients.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="577db-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="577db-115">JSON representation</span></span>

<span data-ttu-id="577db-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="577db-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationAssignmentIndividualRecipient"
}-->

```json
{
  "recipients": ["String"]
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationAssignmentIndividualRecipient resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationassignmentindividualrecipient.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
