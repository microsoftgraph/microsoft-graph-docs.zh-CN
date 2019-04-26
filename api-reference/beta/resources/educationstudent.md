---
title: educationStudent 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 9927c2fbb34dea97258c4c1ef407d60f14e2fe50
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334107"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="2f05e-103">educationStudent 资源类型</span><span class="sxs-lookup"><span data-stu-id="2f05e-103">educationStudent resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2f05e-104">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。</span><span class="sxs-lookup"><span data-stu-id="2f05e-104">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="2f05e-105">属性</span><span class="sxs-lookup"><span data-stu-id="2f05e-105">Properties</span></span>
| <span data-ttu-id="2f05e-106">属性</span><span class="sxs-lookup"><span data-stu-id="2f05e-106">Property</span></span>     | <span data-ttu-id="2f05e-107">类型</span><span class="sxs-lookup"><span data-stu-id="2f05e-107">Type</span></span>   |<span data-ttu-id="2f05e-108">说明</span><span class="sxs-lookup"><span data-stu-id="2f05e-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2f05e-109">birthDate</span><span class="sxs-lookup"><span data-stu-id="2f05e-109">birthDate</span></span>|<span data-ttu-id="2f05e-110">Date</span><span class="sxs-lookup"><span data-stu-id="2f05e-110">Date</span></span>| <span data-ttu-id="2f05e-111">学生的出生日期。</span><span class="sxs-lookup"><span data-stu-id="2f05e-111">Birth date of the student.</span></span>|
|<span data-ttu-id="2f05e-112">externalId</span><span class="sxs-lookup"><span data-stu-id="2f05e-112">externalId</span></span>|<span data-ttu-id="2f05e-113">String</span><span class="sxs-lookup"><span data-stu-id="2f05e-113">String</span></span>| <span data-ttu-id="2f05e-114">源系统中学生的 ID。</span><span class="sxs-lookup"><span data-stu-id="2f05e-114">ID of the student in the source system.</span></span>|
|<span data-ttu-id="2f05e-115">gender</span><span class="sxs-lookup"><span data-stu-id="2f05e-115">gender</span></span>|<span data-ttu-id="2f05e-116">educationGender</span><span class="sxs-lookup"><span data-stu-id="2f05e-116">educationGender</span></span>| <span data-ttu-id="2f05e-117">可取值为：`female`、`male`、`other`、`unkownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="2f05e-117">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="2f05e-118">grade</span><span class="sxs-lookup"><span data-stu-id="2f05e-118">grade</span></span>|<span data-ttu-id="2f05e-119">String</span><span class="sxs-lookup"><span data-stu-id="2f05e-119">String</span></span>|<span data-ttu-id="2f05e-120">学生的当前年级。</span><span class="sxs-lookup"><span data-stu-id="2f05e-120">Current grade level of the student.</span></span>|
|<span data-ttu-id="2f05e-121">graduationYear</span><span class="sxs-lookup"><span data-stu-id="2f05e-121">graduationYear</span></span>|<span data-ttu-id="2f05e-122">String</span><span class="sxs-lookup"><span data-stu-id="2f05e-122">String</span></span>| <span data-ttu-id="2f05e-123">学生从学校毕业的年份。</span><span class="sxs-lookup"><span data-stu-id="2f05e-123">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="2f05e-124">studentNumber</span><span class="sxs-lookup"><span data-stu-id="2f05e-124">studentNumber</span></span>|<span data-ttu-id="2f05e-125">String</span><span class="sxs-lookup"><span data-stu-id="2f05e-125">String</span></span>| <span data-ttu-id="2f05e-126">学生编号。</span><span class="sxs-lookup"><span data-stu-id="2f05e-126">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2f05e-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2f05e-127">JSON representation</span></span>

<span data-ttu-id="2f05e-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2f05e-128">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
