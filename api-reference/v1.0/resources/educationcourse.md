---
title: educationCourse 资源类型
description: 表示课程的课程信息。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 347eb92cd0b36789cc7ecce1dea72af6985ea330
ms.sourcegitcommit: 34891a1c601976166958be1aa04bab5936592b44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/06/2021
ms.locfileid: "52232135"
---
# <a name="educationcourse-resource-type"></a><span data-ttu-id="e491b-103">educationCourse 资源类型</span><span class="sxs-lookup"><span data-stu-id="e491b-103">educationCourse resource type</span></span>

<span data-ttu-id="e491b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e491b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e491b-105">表示课程的课程信息。</span><span class="sxs-lookup"><span data-stu-id="e491b-105">Represents the course information for a class.</span></span> <span data-ttu-id="e491b-106">在 [educationClass](educationclass.md) 中使用。</span><span class="sxs-lookup"><span data-stu-id="e491b-106">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="e491b-107">属性</span><span class="sxs-lookup"><span data-stu-id="e491b-107">Properties</span></span>

| <span data-ttu-id="e491b-108">属性</span><span class="sxs-lookup"><span data-stu-id="e491b-108">Property</span></span>     | <span data-ttu-id="e491b-109">类型</span><span class="sxs-lookup"><span data-stu-id="e491b-109">Type</span></span>   | <span data-ttu-id="e491b-110">说明</span><span class="sxs-lookup"><span data-stu-id="e491b-110">Description</span></span>                               |
| :----------- | :----- | :---------------------------------------- |
| <span data-ttu-id="e491b-111">courseNumber</span><span class="sxs-lookup"><span data-stu-id="e491b-111">courseNumber</span></span> | <span data-ttu-id="e491b-112">String</span><span class="sxs-lookup"><span data-stu-id="e491b-112">String</span></span> | <span data-ttu-id="e491b-113">课程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e491b-113">Unique identifier for the course.</span></span>         |
| <span data-ttu-id="e491b-114">说明</span><span class="sxs-lookup"><span data-stu-id="e491b-114">description</span></span>  | <span data-ttu-id="e491b-115">String</span><span class="sxs-lookup"><span data-stu-id="e491b-115">String</span></span> | <span data-ttu-id="e491b-116">课程说明。</span><span class="sxs-lookup"><span data-stu-id="e491b-116">Description of the course.</span></span>                |
| <span data-ttu-id="e491b-117">displayName</span><span class="sxs-lookup"><span data-stu-id="e491b-117">displayName</span></span>  | <span data-ttu-id="e491b-118">String</span><span class="sxs-lookup"><span data-stu-id="e491b-118">String</span></span> | <span data-ttu-id="e491b-119">课程名称。</span><span class="sxs-lookup"><span data-stu-id="e491b-119">Name of the course.</span></span>                       |
| <span data-ttu-id="e491b-120">externalId</span><span class="sxs-lookup"><span data-stu-id="e491b-120">externalId</span></span>   | <span data-ttu-id="e491b-121">String</span><span class="sxs-lookup"><span data-stu-id="e491b-121">String</span></span> | <span data-ttu-id="e491b-122">同步系统中课程的 ID。</span><span class="sxs-lookup"><span data-stu-id="e491b-122">ID of the course from the syncing system.</span></span> |
| <span data-ttu-id="e491b-123">subject</span><span class="sxs-lookup"><span data-stu-id="e491b-123">subject</span></span>      | <span data-ttu-id="e491b-124">String</span><span class="sxs-lookup"><span data-stu-id="e491b-124">String</span></span> | <span data-ttu-id="e491b-125">课程主题。</span><span class="sxs-lookup"><span data-stu-id="e491b-125">Subject of the course.</span></span>                    |

## <a name="relationships"></a><span data-ttu-id="e491b-126">关系</span><span class="sxs-lookup"><span data-stu-id="e491b-126">Relationships</span></span>

<span data-ttu-id="e491b-127">无。</span><span class="sxs-lookup"><span data-stu-id="e491b-127">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="e491b-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e491b-128">JSON representation</span></span>

<span data-ttu-id="e491b-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e491b-129">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.educationCourse"
}
-->

```json
{
  "@odata.type": "#microsoft.graph.educationCourse",
  "subject": "String",
  "courseNumber": "String",
  "description": "String",
  "displayName": "String",
  "externalId": "String"
}
```
