---
title: educationCourse 资源类型
description: 表示类的课程信息。
author: mlafleur
localization_priority: Normal
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: c160f9bd20f7dfccfa19dbf4d466dd967fde9c2c
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972759"
---
# <a name="educationcourse-resource-type"></a><span data-ttu-id="ec12a-103">educationCourse 资源类型</span><span class="sxs-lookup"><span data-stu-id="ec12a-103">educationCourse resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ec12a-104">表示类的课程信息。</span><span class="sxs-lookup"><span data-stu-id="ec12a-104">Represents the course information for a class.</span></span> <span data-ttu-id="ec12a-105">在 [educationClass](educationclass.md) 中使用。</span><span class="sxs-lookup"><span data-stu-id="ec12a-105">It is used within [educationClass](educationclass.md).</span></span>

## <a name="properties"></a><span data-ttu-id="ec12a-106">属性</span><span class="sxs-lookup"><span data-stu-id="ec12a-106">Properties</span></span>

| <span data-ttu-id="ec12a-107">属性</span><span class="sxs-lookup"><span data-stu-id="ec12a-107">Property</span></span>     | <span data-ttu-id="ec12a-108">类型</span><span class="sxs-lookup"><span data-stu-id="ec12a-108">Type</span></span>   | <span data-ttu-id="ec12a-109">说明</span><span class="sxs-lookup"><span data-stu-id="ec12a-109">Description</span></span>                               |
| :----------- | :----- | :---------------------------------------- |
| <span data-ttu-id="ec12a-110">courseNumber</span><span class="sxs-lookup"><span data-stu-id="ec12a-110">courseNumber</span></span> | <span data-ttu-id="ec12a-111">String</span><span class="sxs-lookup"><span data-stu-id="ec12a-111">String</span></span> | <span data-ttu-id="ec12a-112">课程的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="ec12a-112">Unique identifier for the course.</span></span>         |
| <span data-ttu-id="ec12a-113">说明</span><span class="sxs-lookup"><span data-stu-id="ec12a-113">description</span></span>  | <span data-ttu-id="ec12a-114">字符串</span><span class="sxs-lookup"><span data-stu-id="ec12a-114">String</span></span> | <span data-ttu-id="ec12a-115">课程的说明。</span><span class="sxs-lookup"><span data-stu-id="ec12a-115">Description of the course.</span></span>                |
| <span data-ttu-id="ec12a-116">displayName</span><span class="sxs-lookup"><span data-stu-id="ec12a-116">displayName</span></span>  | <span data-ttu-id="ec12a-117">字符串</span><span class="sxs-lookup"><span data-stu-id="ec12a-117">String</span></span> | <span data-ttu-id="ec12a-118">课程的名称。</span><span class="sxs-lookup"><span data-stu-id="ec12a-118">Name of the course.</span></span>                       |
| <span data-ttu-id="ec12a-119">externalId</span><span class="sxs-lookup"><span data-stu-id="ec12a-119">externalId</span></span>   | <span data-ttu-id="ec12a-120">String</span><span class="sxs-lookup"><span data-stu-id="ec12a-120">String</span></span> | <span data-ttu-id="ec12a-121">来自同步系统的课程 ID。</span><span class="sxs-lookup"><span data-stu-id="ec12a-121">ID of the course from the syncing system.</span></span> |
| <span data-ttu-id="ec12a-122">subject</span><span class="sxs-lookup"><span data-stu-id="ec12a-122">subject</span></span>      | <span data-ttu-id="ec12a-123">String</span><span class="sxs-lookup"><span data-stu-id="ec12a-123">String</span></span> | <span data-ttu-id="ec12a-124">课程的主题。</span><span class="sxs-lookup"><span data-stu-id="ec12a-124">Subject of the course.</span></span>                    |

## <a name="json-representation"></a><span data-ttu-id="ec12a-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ec12a-125">JSON representation</span></span>

<span data-ttu-id="ec12a-126">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec12a-126">The following is a JSON representation of the resource.</span></span>

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
