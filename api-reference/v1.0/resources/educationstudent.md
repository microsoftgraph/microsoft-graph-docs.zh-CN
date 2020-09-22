---
title: educationStudent 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c8cc053900a774f6a79bcabb5350a840959aeeb1
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48032614"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="73d8a-103">educationStudent 资源类型</span><span class="sxs-lookup"><span data-stu-id="73d8a-103">educationStudent resource type</span></span>

<span data-ttu-id="73d8a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="73d8a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="73d8a-105">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。</span><span class="sxs-lookup"><span data-stu-id="73d8a-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="73d8a-106">属性</span><span class="sxs-lookup"><span data-stu-id="73d8a-106">Properties</span></span>
| <span data-ttu-id="73d8a-107">属性</span><span class="sxs-lookup"><span data-stu-id="73d8a-107">Property</span></span>     | <span data-ttu-id="73d8a-108">类型</span><span class="sxs-lookup"><span data-stu-id="73d8a-108">Type</span></span>   |<span data-ttu-id="73d8a-109">说明</span><span class="sxs-lookup"><span data-stu-id="73d8a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73d8a-110">birthDate</span><span class="sxs-lookup"><span data-stu-id="73d8a-110">birthDate</span></span>|<span data-ttu-id="73d8a-111">Date</span><span class="sxs-lookup"><span data-stu-id="73d8a-111">Date</span></span>| <span data-ttu-id="73d8a-112">学生的出生日期。</span><span class="sxs-lookup"><span data-stu-id="73d8a-112">Birth date of the student.</span></span>|
|<span data-ttu-id="73d8a-113">externalId</span><span class="sxs-lookup"><span data-stu-id="73d8a-113">externalId</span></span>|<span data-ttu-id="73d8a-114">String</span><span class="sxs-lookup"><span data-stu-id="73d8a-114">String</span></span>| <span data-ttu-id="73d8a-115">源系统中学生的 ID。</span><span class="sxs-lookup"><span data-stu-id="73d8a-115">ID of the student in the source system.</span></span>|
|<span data-ttu-id="73d8a-116">gender</span><span class="sxs-lookup"><span data-stu-id="73d8a-116">gender</span></span>|<span data-ttu-id="73d8a-117">educationGender</span><span class="sxs-lookup"><span data-stu-id="73d8a-117">educationGender</span></span>| <span data-ttu-id="73d8a-118">可能的值包括 `female`、`male`、`other`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="73d8a-118">The possible values are: `female`, `male`, `other`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="73d8a-119">grade</span><span class="sxs-lookup"><span data-stu-id="73d8a-119">grade</span></span>|<span data-ttu-id="73d8a-120">String</span><span class="sxs-lookup"><span data-stu-id="73d8a-120">String</span></span>|<span data-ttu-id="73d8a-121">学生的当前年级。</span><span class="sxs-lookup"><span data-stu-id="73d8a-121">Current grade level of the student.</span></span>|
|<span data-ttu-id="73d8a-122">graduationYear</span><span class="sxs-lookup"><span data-stu-id="73d8a-122">graduationYear</span></span>|<span data-ttu-id="73d8a-123">String</span><span class="sxs-lookup"><span data-stu-id="73d8a-123">String</span></span>| <span data-ttu-id="73d8a-124">学生从学校毕业的年份。</span><span class="sxs-lookup"><span data-stu-id="73d8a-124">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="73d8a-125">studentNumber</span><span class="sxs-lookup"><span data-stu-id="73d8a-125">studentNumber</span></span>|<span data-ttu-id="73d8a-126">String</span><span class="sxs-lookup"><span data-stu-id="73d8a-126">String</span></span>| <span data-ttu-id="73d8a-127">学生编号。</span><span class="sxs-lookup"><span data-stu-id="73d8a-127">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="73d8a-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73d8a-128">JSON representation</span></span>

<span data-ttu-id="73d8a-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73d8a-129">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationStudent resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

