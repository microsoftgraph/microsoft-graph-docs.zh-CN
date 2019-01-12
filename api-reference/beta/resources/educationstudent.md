---
title: educationStudent 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: b6f6cf8e8a79c427403c2f2157228c8ce130b313
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27913308"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="6b702-103">educationStudent 资源类型</span><span class="sxs-lookup"><span data-stu-id="6b702-103">educationStudent resource type</span></span>

> <span data-ttu-id="6b702-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6b702-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6b702-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6b702-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6b702-106">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。</span><span class="sxs-lookup"><span data-stu-id="6b702-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="6b702-107">属性</span><span class="sxs-lookup"><span data-stu-id="6b702-107">Properties</span></span>
| <span data-ttu-id="6b702-108">属性</span><span class="sxs-lookup"><span data-stu-id="6b702-108">Property</span></span>     | <span data-ttu-id="6b702-109">类型</span><span class="sxs-lookup"><span data-stu-id="6b702-109">Type</span></span>   |<span data-ttu-id="6b702-110">说明</span><span class="sxs-lookup"><span data-stu-id="6b702-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6b702-111">birthDate</span><span class="sxs-lookup"><span data-stu-id="6b702-111">birthDate</span></span>|<span data-ttu-id="6b702-112">Date</span><span class="sxs-lookup"><span data-stu-id="6b702-112">Date</span></span>| <span data-ttu-id="6b702-113">学生的出生日期。</span><span class="sxs-lookup"><span data-stu-id="6b702-113">Birth date of the student.</span></span>|
|<span data-ttu-id="6b702-114">externalId</span><span class="sxs-lookup"><span data-stu-id="6b702-114">externalId</span></span>|<span data-ttu-id="6b702-115">String</span><span class="sxs-lookup"><span data-stu-id="6b702-115">String</span></span>| <span data-ttu-id="6b702-116">源系统中学生的 ID。</span><span class="sxs-lookup"><span data-stu-id="6b702-116">ID of the student in the source system.</span></span>|
|<span data-ttu-id="6b702-117">gender</span><span class="sxs-lookup"><span data-stu-id="6b702-117">gender</span></span>|`educationGender enumeration`| <span data-ttu-id="6b702-118">可取值为：`female`、`male`、`other`、`unkownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="6b702-118">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="6b702-119">grade</span><span class="sxs-lookup"><span data-stu-id="6b702-119">grade</span></span>|<span data-ttu-id="6b702-120">String</span><span class="sxs-lookup"><span data-stu-id="6b702-120">String</span></span>|<span data-ttu-id="6b702-121">学生的当前年级。</span><span class="sxs-lookup"><span data-stu-id="6b702-121">Current grade level of the student.</span></span>|
|<span data-ttu-id="6b702-122">graduationYear</span><span class="sxs-lookup"><span data-stu-id="6b702-122">graduationYear</span></span>|<span data-ttu-id="6b702-123">String</span><span class="sxs-lookup"><span data-stu-id="6b702-123">String</span></span>| <span data-ttu-id="6b702-124">学生从学校毕业的年份。</span><span class="sxs-lookup"><span data-stu-id="6b702-124">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="6b702-125">studentNumber</span><span class="sxs-lookup"><span data-stu-id="6b702-125">studentNumber</span></span>|<span data-ttu-id="6b702-126">String</span><span class="sxs-lookup"><span data-stu-id="6b702-126">String</span></span>| <span data-ttu-id="6b702-127">学生编号。</span><span class="sxs-lookup"><span data-stu-id="6b702-127">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="6b702-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6b702-128">JSON representation</span></span>

<span data-ttu-id="6b702-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b702-129">The following is a JSON representation of the resource.</span></span>

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
