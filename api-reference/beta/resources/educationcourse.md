---
title: educationCourse 资源类型
description: 表示类的课程信息。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 9ba29e98150db6ffa9938585540d9b77f8a755cc
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42502268"
---
# <a name="educationcourse-resource-type"></a><span data-ttu-id="d0448-103">educationCourse 资源类型</span><span class="sxs-lookup"><span data-stu-id="d0448-103">educationCourse resource type</span></span>

<span data-ttu-id="d0448-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="d0448-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d0448-105">表示类的课程信息。</span><span class="sxs-lookup"><span data-stu-id="d0448-105">Represents the course information for a class.</span></span> <span data-ttu-id="d0448-106">在 [educationClass](educationclass.md) 中使用。</span><span class="sxs-lookup"><span data-stu-id="d0448-106">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="d0448-107">属性</span><span class="sxs-lookup"><span data-stu-id="d0448-107">Properties</span></span>

| <span data-ttu-id="d0448-108">属性</span><span class="sxs-lookup"><span data-stu-id="d0448-108">Property</span></span>     | <span data-ttu-id="d0448-109">类型</span><span class="sxs-lookup"><span data-stu-id="d0448-109">Type</span></span>   | <span data-ttu-id="d0448-110">说明</span><span class="sxs-lookup"><span data-stu-id="d0448-110">Description</span></span>                               |
| :----------- | :----- | :---------------------------------------- |
| <span data-ttu-id="d0448-111">courseNumber</span><span class="sxs-lookup"><span data-stu-id="d0448-111">courseNumber</span></span> | <span data-ttu-id="d0448-112">String</span><span class="sxs-lookup"><span data-stu-id="d0448-112">String</span></span> | <span data-ttu-id="d0448-113">课程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d0448-113">Unique identifier for the course.</span></span>         |
| <span data-ttu-id="d0448-114">说明</span><span class="sxs-lookup"><span data-stu-id="d0448-114">description</span></span>  | <span data-ttu-id="d0448-115">字符串</span><span class="sxs-lookup"><span data-stu-id="d0448-115">String</span></span> | <span data-ttu-id="d0448-116">课程的说明。</span><span class="sxs-lookup"><span data-stu-id="d0448-116">Description of the course.</span></span>                |
| <span data-ttu-id="d0448-117">displayName</span><span class="sxs-lookup"><span data-stu-id="d0448-117">displayName</span></span>  | <span data-ttu-id="d0448-118">字符串</span><span class="sxs-lookup"><span data-stu-id="d0448-118">String</span></span> | <span data-ttu-id="d0448-119">课程的名称。</span><span class="sxs-lookup"><span data-stu-id="d0448-119">Name of the course.</span></span>                       |
| <span data-ttu-id="d0448-120">externalId</span><span class="sxs-lookup"><span data-stu-id="d0448-120">externalId</span></span>   | <span data-ttu-id="d0448-121">String</span><span class="sxs-lookup"><span data-stu-id="d0448-121">String</span></span> | <span data-ttu-id="d0448-122">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="d0448-122">ID of the course from the syncing system.</span></span> |
| <span data-ttu-id="d0448-123">subject</span><span class="sxs-lookup"><span data-stu-id="d0448-123">subject</span></span>      | <span data-ttu-id="d0448-124">String</span><span class="sxs-lookup"><span data-stu-id="d0448-124">String</span></span> | <span data-ttu-id="d0448-125">课程的主题。</span><span class="sxs-lookup"><span data-stu-id="d0448-125">Subject of the course.</span></span>                    |

## <a name="json-representation"></a><span data-ttu-id="d0448-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d0448-126">JSON representation</span></span>

<span data-ttu-id="d0448-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d0448-127">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationCourse"
}-->

```json
{
  "courseNumber": "String",
  "description": "String",
  "displayName": "String",
  "externalId": "String",
  "subject": "String"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "educationCourse resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
