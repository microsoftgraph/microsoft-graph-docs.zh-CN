---
title: educationStudent 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。
ms.openlocfilehash: cd5435514b44ffe6baa071a547f3e17ef0239b02
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27048785"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="f0ad4-103">educationStudent 资源类型</span><span class="sxs-lookup"><span data-stu-id="f0ad4-103">educationStudent resource type</span></span>

> <span data-ttu-id="f0ad4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f0ad4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f0ad4-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f0ad4-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f0ad4-106">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。</span><span class="sxs-lookup"><span data-stu-id="f0ad4-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="f0ad4-107">属性</span><span class="sxs-lookup"><span data-stu-id="f0ad4-107">Properties</span></span>
| <span data-ttu-id="f0ad4-108">属性</span><span class="sxs-lookup"><span data-stu-id="f0ad4-108">Property</span></span>     | <span data-ttu-id="f0ad4-109">类型</span><span class="sxs-lookup"><span data-stu-id="f0ad4-109">Type</span></span>   |<span data-ttu-id="f0ad4-110">说明</span><span class="sxs-lookup"><span data-stu-id="f0ad4-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f0ad4-111">birthDate</span><span class="sxs-lookup"><span data-stu-id="f0ad4-111">birthDate</span></span>|<span data-ttu-id="f0ad4-112">Date</span><span class="sxs-lookup"><span data-stu-id="f0ad4-112">Date</span></span>| <span data-ttu-id="f0ad4-113">学生的出生日期。</span><span class="sxs-lookup"><span data-stu-id="f0ad4-113">Birth date of the student.</span></span>|
|<span data-ttu-id="f0ad4-114">externalId</span><span class="sxs-lookup"><span data-stu-id="f0ad4-114">externalId</span></span>|<span data-ttu-id="f0ad4-115">String</span><span class="sxs-lookup"><span data-stu-id="f0ad4-115">String</span></span>| <span data-ttu-id="f0ad4-116">源系统中学生的 ID。</span><span class="sxs-lookup"><span data-stu-id="f0ad4-116">ID of the student in the source system.</span></span>|
|<span data-ttu-id="f0ad4-117">gender</span><span class="sxs-lookup"><span data-stu-id="f0ad4-117">gender</span></span>|`educationGender enumeration`| <span data-ttu-id="f0ad4-118">可取值为：`female`、`male`、`other`、`unkownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="f0ad4-118">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="f0ad4-119">grade</span><span class="sxs-lookup"><span data-stu-id="f0ad4-119">grade</span></span>|<span data-ttu-id="f0ad4-120">String</span><span class="sxs-lookup"><span data-stu-id="f0ad4-120">String</span></span>|<span data-ttu-id="f0ad4-121">学生的当前年级。</span><span class="sxs-lookup"><span data-stu-id="f0ad4-121">Current grade level of the student.</span></span>|
|<span data-ttu-id="f0ad4-122">graduationYear</span><span class="sxs-lookup"><span data-stu-id="f0ad4-122">graduationYear</span></span>|<span data-ttu-id="f0ad4-123">String</span><span class="sxs-lookup"><span data-stu-id="f0ad4-123">String</span></span>| <span data-ttu-id="f0ad4-124">学生从学校毕业的年份。</span><span class="sxs-lookup"><span data-stu-id="f0ad4-124">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="f0ad4-125">studentNumber</span><span class="sxs-lookup"><span data-stu-id="f0ad4-125">studentNumber</span></span>|<span data-ttu-id="f0ad4-126">String</span><span class="sxs-lookup"><span data-stu-id="f0ad4-126">String</span></span>| <span data-ttu-id="f0ad4-127">学生编号。</span><span class="sxs-lookup"><span data-stu-id="f0ad4-127">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f0ad4-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f0ad4-128">JSON representation</span></span>

<span data-ttu-id="f0ad4-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f0ad4-129">The following is a JSON representation of the resource.</span></span>

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