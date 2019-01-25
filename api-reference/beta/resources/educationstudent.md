---
title: educationStudent 资源类型
description: 添加到 `student` 的其他信息，该属性将在用户的 primaryRole 为  时显示。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 554763d41c4ce48a09334394330e05fcd6dd4152
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29522033"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="b7c98-103">educationStudent 资源类型</span><span class="sxs-lookup"><span data-stu-id="b7c98-103">educationStudent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b7c98-104">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。</span><span class="sxs-lookup"><span data-stu-id="b7c98-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="b7c98-105">属性</span><span class="sxs-lookup"><span data-stu-id="b7c98-105">Properties</span></span>
| <span data-ttu-id="b7c98-106">属性</span><span class="sxs-lookup"><span data-stu-id="b7c98-106">Property</span></span>     | <span data-ttu-id="b7c98-107">类型</span><span class="sxs-lookup"><span data-stu-id="b7c98-107">Type</span></span>   |<span data-ttu-id="b7c98-108">说明</span><span class="sxs-lookup"><span data-stu-id="b7c98-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b7c98-109">birthDate</span><span class="sxs-lookup"><span data-stu-id="b7c98-109">birthDate</span></span>|<span data-ttu-id="b7c98-110">Date</span><span class="sxs-lookup"><span data-stu-id="b7c98-110">Date</span></span>| <span data-ttu-id="b7c98-111">学生的出生日期。</span><span class="sxs-lookup"><span data-stu-id="b7c98-111">Birth date of the student.</span></span>|
|<span data-ttu-id="b7c98-112">externalId</span><span class="sxs-lookup"><span data-stu-id="b7c98-112">externalId</span></span>|<span data-ttu-id="b7c98-113">String</span><span class="sxs-lookup"><span data-stu-id="b7c98-113">String</span></span>| <span data-ttu-id="b7c98-114">源系统中学生的 ID。</span><span class="sxs-lookup"><span data-stu-id="b7c98-114">ID of the student in the source system.</span></span>|
|<span data-ttu-id="b7c98-115">gender</span><span class="sxs-lookup"><span data-stu-id="b7c98-115">gender</span></span>|<span data-ttu-id="b7c98-116">educationGender</span><span class="sxs-lookup"><span data-stu-id="b7c98-116">educationGender</span></span>| <span data-ttu-id="b7c98-117">可取值为：`female`、`male`、`other`、`unkownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="b7c98-117">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="b7c98-118">grade</span><span class="sxs-lookup"><span data-stu-id="b7c98-118">grade</span></span>|<span data-ttu-id="b7c98-119">String</span><span class="sxs-lookup"><span data-stu-id="b7c98-119">String</span></span>|<span data-ttu-id="b7c98-120">学生的当前年级。</span><span class="sxs-lookup"><span data-stu-id="b7c98-120">Current grade level of the student.</span></span>|
|<span data-ttu-id="b7c98-121">graduationYear</span><span class="sxs-lookup"><span data-stu-id="b7c98-121">graduationYear</span></span>|<span data-ttu-id="b7c98-122">String</span><span class="sxs-lookup"><span data-stu-id="b7c98-122">String</span></span>| <span data-ttu-id="b7c98-123">学生从学校毕业的年份。</span><span class="sxs-lookup"><span data-stu-id="b7c98-123">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="b7c98-124">studentNumber</span><span class="sxs-lookup"><span data-stu-id="b7c98-124">studentNumber</span></span>|<span data-ttu-id="b7c98-125">String</span><span class="sxs-lookup"><span data-stu-id="b7c98-125">String</span></span>| <span data-ttu-id="b7c98-126">学生编号。</span><span class="sxs-lookup"><span data-stu-id="b7c98-126">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="b7c98-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b7c98-127">JSON representation</span></span>

<span data-ttu-id="b7c98-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b7c98-128">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationStudent"
}-->

```json
{
  "birthDate": "String (timestamp)",
  "externalId": "String",
  "gender": "educationGender",
  "grade": "String",
  "graduationYear": "String",
  "studentNumber": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/educationstudent.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
