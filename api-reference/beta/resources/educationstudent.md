---
title: educationStudent 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。
author: mmast-msft
localization_priority: Normal
ms.prod: education
ms.openlocfilehash: 19ce3e28ccedc5f6165c8c333afb2ccd10343f14
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29406904"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="ecb5c-103">educationStudent 资源类型</span><span class="sxs-lookup"><span data-stu-id="ecb5c-103">educationStudent resource type</span></span>

> <span data-ttu-id="ecb5c-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ecb5c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ecb5c-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ecb5c-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ecb5c-106">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。</span><span class="sxs-lookup"><span data-stu-id="ecb5c-106">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="ecb5c-107">属性</span><span class="sxs-lookup"><span data-stu-id="ecb5c-107">Properties</span></span>
| <span data-ttu-id="ecb5c-108">属性</span><span class="sxs-lookup"><span data-stu-id="ecb5c-108">Property</span></span>     | <span data-ttu-id="ecb5c-109">类型</span><span class="sxs-lookup"><span data-stu-id="ecb5c-109">Type</span></span>   |<span data-ttu-id="ecb5c-110">说明</span><span class="sxs-lookup"><span data-stu-id="ecb5c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ecb5c-111">birthDate</span><span class="sxs-lookup"><span data-stu-id="ecb5c-111">birthDate</span></span>|<span data-ttu-id="ecb5c-112">Date</span><span class="sxs-lookup"><span data-stu-id="ecb5c-112">Date</span></span>| <span data-ttu-id="ecb5c-113">学生的出生日期。</span><span class="sxs-lookup"><span data-stu-id="ecb5c-113">Birth date of the student.</span></span>|
|<span data-ttu-id="ecb5c-114">externalId</span><span class="sxs-lookup"><span data-stu-id="ecb5c-114">externalId</span></span>|<span data-ttu-id="ecb5c-115">String</span><span class="sxs-lookup"><span data-stu-id="ecb5c-115">String</span></span>| <span data-ttu-id="ecb5c-116">源系统中学生的 ID。</span><span class="sxs-lookup"><span data-stu-id="ecb5c-116">ID of the student in the source system.</span></span>|
|<span data-ttu-id="ecb5c-117">gender</span><span class="sxs-lookup"><span data-stu-id="ecb5c-117">gender</span></span>|<span data-ttu-id="ecb5c-118">educationGender</span><span class="sxs-lookup"><span data-stu-id="ecb5c-118">educationGender</span></span>| <span data-ttu-id="ecb5c-119">可取值为：`female`、`male`、`other`、`unkownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="ecb5c-119">Possible values are: `female`, `male`, `other`, `unkownFutureValue`.</span></span>|
|<span data-ttu-id="ecb5c-120">grade</span><span class="sxs-lookup"><span data-stu-id="ecb5c-120">grade</span></span>|<span data-ttu-id="ecb5c-121">String</span><span class="sxs-lookup"><span data-stu-id="ecb5c-121">String</span></span>|<span data-ttu-id="ecb5c-122">学生的当前年级。</span><span class="sxs-lookup"><span data-stu-id="ecb5c-122">Current grade level of the student.</span></span>|
|<span data-ttu-id="ecb5c-123">graduationYear</span><span class="sxs-lookup"><span data-stu-id="ecb5c-123">graduationYear</span></span>|<span data-ttu-id="ecb5c-124">String</span><span class="sxs-lookup"><span data-stu-id="ecb5c-124">String</span></span>| <span data-ttu-id="ecb5c-125">学生从学校毕业的年份。</span><span class="sxs-lookup"><span data-stu-id="ecb5c-125">Year the student is graduating from the school.</span></span>|
|<span data-ttu-id="ecb5c-126">studentNumber</span><span class="sxs-lookup"><span data-stu-id="ecb5c-126">studentNumber</span></span>|<span data-ttu-id="ecb5c-127">String</span><span class="sxs-lookup"><span data-stu-id="ecb5c-127">String</span></span>| <span data-ttu-id="ecb5c-128">学生编号。</span><span class="sxs-lookup"><span data-stu-id="ecb5c-128">Student Number.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ecb5c-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ecb5c-129">JSON representation</span></span>

<span data-ttu-id="ecb5c-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ecb5c-130">The following is a JSON representation of the resource.</span></span>

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
