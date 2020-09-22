---
title: educationCourse 资源类型
description: 表示类的课程信息。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 80128524160a5f01806d36f52531383d5ab469a5
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48095511"
---
# <a name="educationcourse-resource-type"></a><span data-ttu-id="0aafd-103">educationCourse 资源类型</span><span class="sxs-lookup"><span data-stu-id="0aafd-103">educationCourse resource type</span></span>

<span data-ttu-id="0aafd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0aafd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0aafd-105">表示类的课程信息。</span><span class="sxs-lookup"><span data-stu-id="0aafd-105">Represents the course information for a class.</span></span> <span data-ttu-id="0aafd-106">在 [educationClass](educationclass.md) 中使用。</span><span class="sxs-lookup"><span data-stu-id="0aafd-106">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="0aafd-107">属性</span><span class="sxs-lookup"><span data-stu-id="0aafd-107">Properties</span></span>

| <span data-ttu-id="0aafd-108">属性</span><span class="sxs-lookup"><span data-stu-id="0aafd-108">Property</span></span>     | <span data-ttu-id="0aafd-109">类型</span><span class="sxs-lookup"><span data-stu-id="0aafd-109">Type</span></span>   | <span data-ttu-id="0aafd-110">说明</span><span class="sxs-lookup"><span data-stu-id="0aafd-110">Description</span></span>                               |
| :----------- | :----- | :---------------------------------------- |
| <span data-ttu-id="0aafd-111">courseNumber</span><span class="sxs-lookup"><span data-stu-id="0aafd-111">courseNumber</span></span> | <span data-ttu-id="0aafd-112">字符串</span><span class="sxs-lookup"><span data-stu-id="0aafd-112">String</span></span> | <span data-ttu-id="0aafd-113">课程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="0aafd-113">Unique identifier for the course.</span></span>         |
| <span data-ttu-id="0aafd-114">说明</span><span class="sxs-lookup"><span data-stu-id="0aafd-114">description</span></span>  | <span data-ttu-id="0aafd-115">字符串</span><span class="sxs-lookup"><span data-stu-id="0aafd-115">String</span></span> | <span data-ttu-id="0aafd-116">课程的说明。</span><span class="sxs-lookup"><span data-stu-id="0aafd-116">Description of the course.</span></span>                |
| <span data-ttu-id="0aafd-117">displayName</span><span class="sxs-lookup"><span data-stu-id="0aafd-117">displayName</span></span>  | <span data-ttu-id="0aafd-118">字符串</span><span class="sxs-lookup"><span data-stu-id="0aafd-118">String</span></span> | <span data-ttu-id="0aafd-119">课程的名称。</span><span class="sxs-lookup"><span data-stu-id="0aafd-119">Name of the course.</span></span>                       |
| <span data-ttu-id="0aafd-120">externalId</span><span class="sxs-lookup"><span data-stu-id="0aafd-120">externalId</span></span>   | <span data-ttu-id="0aafd-121">String</span><span class="sxs-lookup"><span data-stu-id="0aafd-121">String</span></span> | <span data-ttu-id="0aafd-122">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="0aafd-122">ID of the course from the syncing system.</span></span> |
| <span data-ttu-id="0aafd-123">subject</span><span class="sxs-lookup"><span data-stu-id="0aafd-123">subject</span></span>      | <span data-ttu-id="0aafd-124">String</span><span class="sxs-lookup"><span data-stu-id="0aafd-124">String</span></span> | <span data-ttu-id="0aafd-125">课程的主题。</span><span class="sxs-lookup"><span data-stu-id="0aafd-125">Subject of the course.</span></span>                    |

## <a name="json-representation"></a><span data-ttu-id="0aafd-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0aafd-126">JSON representation</span></span>

<span data-ttu-id="0aafd-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0aafd-127">The following is a JSON representation of the resource.</span></span>

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


