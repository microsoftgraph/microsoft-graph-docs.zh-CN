---
title: employeeOrgData 资源类型
description: 表示与用户关联的组织数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: users
author: cmmdesai
ms.openlocfilehash: 5e3ea0401730ffc8b15cae8c371d9352995c6f28
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50961991"
---
# <a name="employeeorgdata-resource-type"></a><span data-ttu-id="9219c-103">employeeOrgData 资源类型</span><span class="sxs-lookup"><span data-stu-id="9219c-103">employeeOrgData resource type</span></span>

<span data-ttu-id="9219c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9219c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9219c-105">表示与用户关联的组织数据。</span><span class="sxs-lookup"><span data-stu-id="9219c-105">Represents organization data associated with a user.</span></span> <span data-ttu-id="9219c-106">user 实体的 **employeeOrgData** 属性是组织属性的集合。 [](user.md)</span><span class="sxs-lookup"><span data-stu-id="9219c-106">The **employeeOrgData** property of the [user](user.md) entity is a collection of organization attributes.</span></span>

## <a name="properties"></a><span data-ttu-id="9219c-107">属性</span><span class="sxs-lookup"><span data-stu-id="9219c-107">Properties</span></span>
| <span data-ttu-id="9219c-108">属性</span><span class="sxs-lookup"><span data-stu-id="9219c-108">Property</span></span>       | <span data-ttu-id="9219c-109">类型</span><span class="sxs-lookup"><span data-stu-id="9219c-109">Type</span></span>    |<span data-ttu-id="9219c-110">说明</span><span class="sxs-lookup"><span data-stu-id="9219c-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="9219c-111">division</span><span class="sxs-lookup"><span data-stu-id="9219c-111">division</span></span> | <span data-ttu-id="9219c-112">String</span><span class="sxs-lookup"><span data-stu-id="9219c-112">String</span></span> | <span data-ttu-id="9219c-113">用户工作部门的名称。</span><span class="sxs-lookup"><span data-stu-id="9219c-113">The name of the division in which the user works.</span></span> <br><br><span data-ttu-id="9219c-114">仅在 `$select` 上返回。</span><span class="sxs-lookup"><span data-stu-id="9219c-114">Returned only on `$select`.</span></span> <span data-ttu-id="9219c-115">支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="9219c-115">Supports `$filter`.</span></span> |
| <span data-ttu-id="9219c-116">costCenter</span><span class="sxs-lookup"><span data-stu-id="9219c-116">costCenter</span></span> | <span data-ttu-id="9219c-117">String</span><span class="sxs-lookup"><span data-stu-id="9219c-117">String</span></span> | <span data-ttu-id="9219c-118">与用户关联的成本中心。</span><span class="sxs-lookup"><span data-stu-id="9219c-118">The cost center associated with the user.</span></span> <br><br><span data-ttu-id="9219c-119">仅在 `$select` 上返回。</span><span class="sxs-lookup"><span data-stu-id="9219c-119">Returned only on `$select`.</span></span> <span data-ttu-id="9219c-120">支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="9219c-120">Supports `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9219c-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9219c-121">JSON representation</span></span>

<span data-ttu-id="9219c-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9219c-122">The following is a JSON representation of the resource.</span></span>

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
