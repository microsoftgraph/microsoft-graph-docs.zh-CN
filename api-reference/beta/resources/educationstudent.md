---
title: educationStudent 资源类型
description: 添加到 educationUser 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。
author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: e64899cf56140246373c36428518ebd28bb136c7
ms.sourcegitcommit: 55e9497c8e003be389f8b5d641f80dae7bf6004b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2020
ms.locfileid: "44909721"
---
# <a name="educationstudent-resource-type"></a><span data-ttu-id="f41d3-103">educationStudent 资源类型</span><span class="sxs-lookup"><span data-stu-id="f41d3-103">educationStudent resource type</span></span>

<span data-ttu-id="f41d3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f41d3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f41d3-105">添加到 [educationUser](educationuser.md) 的其他信息，该属性将在用户的 primaryRole 为 `student` 时显示。</span><span class="sxs-lookup"><span data-stu-id="f41d3-105">Additional information added to an [educationUser](educationuser.md) that is present when the primaryRole of a user is `student`.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="f41d3-106">使用委派权限作用域时，Graph 将仅返回 `externalId` 属性。</span><span class="sxs-lookup"><span data-stu-id="f41d3-106">When using Delegated permission scopes, Graph will only return the `externalId` properties.</span></span> <span data-ttu-id="f41d3-107">所有其他属性都需要应用程序范围。</span><span class="sxs-lookup"><span data-stu-id="f41d3-107">All other properties require Application scopes.</span></span>

## <a name="properties"></a><span data-ttu-id="f41d3-108">属性</span><span class="sxs-lookup"><span data-stu-id="f41d3-108">Properties</span></span>

| <span data-ttu-id="f41d3-109">属性</span><span class="sxs-lookup"><span data-stu-id="f41d3-109">Property</span></span>       | <span data-ttu-id="f41d3-110">类型</span><span class="sxs-lookup"><span data-stu-id="f41d3-110">Type</span></span>            | <span data-ttu-id="f41d3-111">说明</span><span class="sxs-lookup"><span data-stu-id="f41d3-111">Description</span></span>                                     |
| :------------- | :-------------- | :---------------------------------------------- |
| <span data-ttu-id="f41d3-112">birthDate</span><span class="sxs-lookup"><span data-stu-id="f41d3-112">birthDate</span></span>      | <span data-ttu-id="f41d3-113">Date</span><span class="sxs-lookup"><span data-stu-id="f41d3-113">Date</span></span>            | <span data-ttu-id="f41d3-114">学生的出生日期。</span><span class="sxs-lookup"><span data-stu-id="f41d3-114">Birth date of the student.</span></span>                      |
| <span data-ttu-id="f41d3-115">externalId</span><span class="sxs-lookup"><span data-stu-id="f41d3-115">externalId</span></span>     | <span data-ttu-id="f41d3-116">String</span><span class="sxs-lookup"><span data-stu-id="f41d3-116">String</span></span>          | <span data-ttu-id="f41d3-117">源系统中学生的 ID。</span><span class="sxs-lookup"><span data-stu-id="f41d3-117">ID of the student in the source system.</span></span>         |
| <span data-ttu-id="f41d3-118">gender</span><span class="sxs-lookup"><span data-stu-id="f41d3-118">gender</span></span>         | <span data-ttu-id="f41d3-119">educationGender</span><span class="sxs-lookup"><span data-stu-id="f41d3-119">educationGender</span></span> | <span data-ttu-id="f41d3-120">可取值为：`female`、`male`、`other`。</span><span class="sxs-lookup"><span data-stu-id="f41d3-120">Possible values are: `female`, `male`, `other`.</span></span> |
| <span data-ttu-id="f41d3-121">grade</span><span class="sxs-lookup"><span data-stu-id="f41d3-121">grade</span></span>          | <span data-ttu-id="f41d3-122">String</span><span class="sxs-lookup"><span data-stu-id="f41d3-122">String</span></span>          | <span data-ttu-id="f41d3-123">学生的当前年级。</span><span class="sxs-lookup"><span data-stu-id="f41d3-123">Current grade level of the student.</span></span>             |
| <span data-ttu-id="f41d3-124">graduationYear</span><span class="sxs-lookup"><span data-stu-id="f41d3-124">graduationYear</span></span> | <span data-ttu-id="f41d3-125">String</span><span class="sxs-lookup"><span data-stu-id="f41d3-125">String</span></span>          | <span data-ttu-id="f41d3-126">学生从学校毕业的年份。</span><span class="sxs-lookup"><span data-stu-id="f41d3-126">Year the student is graduating from the school.</span></span> |
| <span data-ttu-id="f41d3-127">studentNumber</span><span class="sxs-lookup"><span data-stu-id="f41d3-127">studentNumber</span></span>  | <span data-ttu-id="f41d3-128">String</span><span class="sxs-lookup"><span data-stu-id="f41d3-128">String</span></span>          | <span data-ttu-id="f41d3-129">学生编号。</span><span class="sxs-lookup"><span data-stu-id="f41d3-129">Student Number.</span></span>                                 |

## <a name="json-representation"></a><span data-ttu-id="f41d3-130">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f41d3-130">JSON representation</span></span>

<span data-ttu-id="f41d3-131">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f41d3-131">The following is a JSON representation of the resource.</span></span>

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
