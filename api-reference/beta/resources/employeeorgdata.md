---
title: employeeOrgData 资源类型
description: 表示与用户关联的组织数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: cmmdesai
ms.openlocfilehash: 841422920ccfe625bd03d8167c13f2a1eba83088
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50960430"
---
# <a name="employeeorgdata-resource-type"></a><span data-ttu-id="45e31-103">employeeOrgData 资源类型</span><span class="sxs-lookup"><span data-stu-id="45e31-103">employeeOrgData resource type</span></span>

<span data-ttu-id="45e31-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45e31-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45e31-105">表示与用户关联的组织数据。</span><span class="sxs-lookup"><span data-stu-id="45e31-105">Represents organization data associated with a user.</span></span> <span data-ttu-id="45e31-106">user 实体的 **employeeOrgData** 属性是组织属性的集合。 [](user.md)</span><span class="sxs-lookup"><span data-stu-id="45e31-106">The **employeeOrgData** property of the [user](user.md) entity is a collection of organization attributes.</span></span>

## <a name="properties"></a><span data-ttu-id="45e31-107">属性</span><span class="sxs-lookup"><span data-stu-id="45e31-107">Properties</span></span>
| <span data-ttu-id="45e31-108">属性</span><span class="sxs-lookup"><span data-stu-id="45e31-108">Property</span></span>       | <span data-ttu-id="45e31-109">类型</span><span class="sxs-lookup"><span data-stu-id="45e31-109">Type</span></span>    |<span data-ttu-id="45e31-110">说明</span><span class="sxs-lookup"><span data-stu-id="45e31-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="45e31-111">division</span><span class="sxs-lookup"><span data-stu-id="45e31-111">division</span></span> | <span data-ttu-id="45e31-112">String</span><span class="sxs-lookup"><span data-stu-id="45e31-112">String</span></span> | <span data-ttu-id="45e31-113">用户工作部门的名称。</span><span class="sxs-lookup"><span data-stu-id="45e31-113">The name of the division in which the user works.</span></span> <br><br><span data-ttu-id="45e31-114">仅在 `$select` 上返回。</span><span class="sxs-lookup"><span data-stu-id="45e31-114">Returned only on `$select`.</span></span> <span data-ttu-id="45e31-115">支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="45e31-115">Supports `$filter`.</span></span> |
| <span data-ttu-id="45e31-116">costCenter</span><span class="sxs-lookup"><span data-stu-id="45e31-116">costCenter</span></span> | <span data-ttu-id="45e31-117">String</span><span class="sxs-lookup"><span data-stu-id="45e31-117">String</span></span> | <span data-ttu-id="45e31-118">与用户关联的成本中心。</span><span class="sxs-lookup"><span data-stu-id="45e31-118">The cost center associated with the user.</span></span> <br><br><span data-ttu-id="45e31-119">仅在 `$select` 上返回。</span><span class="sxs-lookup"><span data-stu-id="45e31-119">Returned only on `$select`.</span></span> <span data-ttu-id="45e31-120">支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="45e31-120">Supports `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="45e31-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45e31-121">JSON representation</span></span>

<span data-ttu-id="45e31-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45e31-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [],
  "@odata.type": "microsoft.graph.employeeOrgData"
}-->

```json
{
  "costCenter": "string",
  "division": "string"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2020-10-24 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "employeeOrgData resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
