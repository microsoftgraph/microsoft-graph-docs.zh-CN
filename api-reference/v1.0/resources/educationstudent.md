---
title: educationStudent 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 5b0e154beb5b8133c69392af8fa9611263c68945
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52231848"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="cd90b-103">educationStudent 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd90b-103">educationStudent resource type</span></span>

<span data-ttu-id="cd90b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd90b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd90b-105">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。</span><span class="sxs-lookup"><span data-stu-id="cd90b-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

## <a name="properties"></a><span data-ttu-id="cd90b-106">属性</span><span class="sxs-lookup"><span data-stu-id="cd90b-106">Properties</span></span>

| <span data-ttu-id="cd90b-107">属性</span><span class="sxs-lookup"><span data-stu-id="cd90b-107">Property</span></span>       | <span data-ttu-id="cd90b-108">类型</span><span class="sxs-lookup"><span data-stu-id="cd90b-108">Type</span></span>            | <span data-ttu-id="cd90b-109">说明</span><span class="sxs-lookup"><span data-stu-id="cd90b-109">Description</span></span>                                                               |
| :------------- | :-------------- | :------------------------------------------------------------------------ |
| <span data-ttu-id="cd90b-110">birthDate</span><span class="sxs-lookup"><span data-stu-id="cd90b-110">birthDate</span></span>      | <span data-ttu-id="cd90b-111">Date</span><span class="sxs-lookup"><span data-stu-id="cd90b-111">Date</span></span>            | <span data-ttu-id="cd90b-112">学生的出生日期。</span><span class="sxs-lookup"><span data-stu-id="cd90b-112">Birth date of the student.</span></span>                                                |
| <span data-ttu-id="cd90b-113">externalId</span><span class="sxs-lookup"><span data-stu-id="cd90b-113">externalId</span></span>     | <span data-ttu-id="cd90b-114">String</span><span class="sxs-lookup"><span data-stu-id="cd90b-114">String</span></span>          | <span data-ttu-id="cd90b-115">源系统中学生的 ID。</span><span class="sxs-lookup"><span data-stu-id="cd90b-115">ID of the student in the source system.</span></span>                                   |
| <span data-ttu-id="cd90b-116">gender</span><span class="sxs-lookup"><span data-stu-id="cd90b-116">gender</span></span>         | <span data-ttu-id="cd90b-117">educationGender</span><span class="sxs-lookup"><span data-stu-id="cd90b-117">educationGender</span></span> | <span data-ttu-id="cd90b-118">可能的值包括 `female`、`male`、`other`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="cd90b-118">The possible values are: `female`, `male`, `other`, `unknownFutureValue`.</span></span> |
| <span data-ttu-id="cd90b-119">grade</span><span class="sxs-lookup"><span data-stu-id="cd90b-119">grade</span></span>          | <span data-ttu-id="cd90b-120">String</span><span class="sxs-lookup"><span data-stu-id="cd90b-120">String</span></span>          | <span data-ttu-id="cd90b-121">学生的当前年级。</span><span class="sxs-lookup"><span data-stu-id="cd90b-121">Current grade level of the student.</span></span>                                       |
| <span data-ttu-id="cd90b-122">graduationYear</span><span class="sxs-lookup"><span data-stu-id="cd90b-122">graduationYear</span></span> | <span data-ttu-id="cd90b-123">String</span><span class="sxs-lookup"><span data-stu-id="cd90b-123">String</span></span>          | <span data-ttu-id="cd90b-124">学生从学校毕业的年份。</span><span class="sxs-lookup"><span data-stu-id="cd90b-124">Year the student is graduating from the school.</span></span>                           |
| <span data-ttu-id="cd90b-125">studentNumber</span><span class="sxs-lookup"><span data-stu-id="cd90b-125">studentNumber</span></span>  | <span data-ttu-id="cd90b-126">String</span><span class="sxs-lookup"><span data-stu-id="cd90b-126">String</span></span>          | <span data-ttu-id="cd90b-127">学生编号。</span><span class="sxs-lookup"><span data-stu-id="cd90b-127">Student Number.</span></span>                                                           |

## <a name="relationships"></a><span data-ttu-id="cd90b-128">关系</span><span class="sxs-lookup"><span data-stu-id="cd90b-128">Relationships</span></span>

<span data-ttu-id="cd90b-129">无。</span><span class="sxs-lookup"><span data-stu-id="cd90b-129">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="cd90b-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd90b-130">JSON representation</span></span>

<span data-ttu-id="cd90b-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd90b-131">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationStudent"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationStudent",
  "graduationYear": "String",
  "grade": "String",
  "birthDate": "DateTimeOffset",
  "gender": "String",
  "studentNumber": "String",
  "externalId": "String"
}
```
