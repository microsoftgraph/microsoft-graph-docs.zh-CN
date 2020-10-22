---
title: employeeOrgData 资源类型
description: 表示与用户相关联的组织数据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: cmmdesai
ms.openlocfilehash: 841d3c7965309721d662475f2cba553c378c49ee
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635606"
---
# <a name="employeeorgdata-resource-type"></a><span data-ttu-id="7ab52-103">employeeOrgData 资源类型</span><span class="sxs-lookup"><span data-stu-id="7ab52-103">employeeOrgData resource type</span></span>

<span data-ttu-id="7ab52-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7ab52-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="7ab52-105">表示与用户相关联的组织数据。</span><span class="sxs-lookup"><span data-stu-id="7ab52-105">Represents organization data associated with a user.</span></span> <span data-ttu-id="7ab52-106">[User](user.md)实体的**employeeOrgData**属性是一个组织属性的集合。</span><span class="sxs-lookup"><span data-stu-id="7ab52-106">The **employeeOrgData** property of the [user](user.md) entity is a collection of organization attributes.</span></span>

## <a name="properties"></a><span data-ttu-id="7ab52-107">属性</span><span class="sxs-lookup"><span data-stu-id="7ab52-107">Properties</span></span>
| <span data-ttu-id="7ab52-108">属性</span><span class="sxs-lookup"><span data-stu-id="7ab52-108">Property</span></span>       | <span data-ttu-id="7ab52-109">类型</span><span class="sxs-lookup"><span data-stu-id="7ab52-109">Type</span></span>    |<span data-ttu-id="7ab52-110">Description</span><span class="sxs-lookup"><span data-stu-id="7ab52-110">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="7ab52-111">division</span><span class="sxs-lookup"><span data-stu-id="7ab52-111">division</span></span> | <span data-ttu-id="7ab52-112">String</span><span class="sxs-lookup"><span data-stu-id="7ab52-112">String</span></span> | <span data-ttu-id="7ab52-113">用户工作的部门的名称。</span><span class="sxs-lookup"><span data-stu-id="7ab52-113">The name of the division in which the user works.</span></span> <br><br><span data-ttu-id="7ab52-114">仅在 `$select` 上返回。</span><span class="sxs-lookup"><span data-stu-id="7ab52-114">Returned only on `$select`.</span></span> <span data-ttu-id="7ab52-115">支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="7ab52-115">Supports `$filter`.</span></span> |
| <span data-ttu-id="7ab52-116">costCenter</span><span class="sxs-lookup"><span data-stu-id="7ab52-116">costCenter</span></span> | <span data-ttu-id="7ab52-117">String</span><span class="sxs-lookup"><span data-stu-id="7ab52-117">String</span></span> | <span data-ttu-id="7ab52-118">与用户关联的成本中心。</span><span class="sxs-lookup"><span data-stu-id="7ab52-118">The cost center associated with the user.</span></span> <br><br><span data-ttu-id="7ab52-119">仅在 `$select` 上返回。</span><span class="sxs-lookup"><span data-stu-id="7ab52-119">Returned only on `$select`.</span></span> <span data-ttu-id="7ab52-120">支持 `$filter`。</span><span class="sxs-lookup"><span data-stu-id="7ab52-120">Supports `$filter`.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="7ab52-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7ab52-121">JSON representation</span></span>

<span data-ttu-id="7ab52-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ab52-122">The following is a JSON representation of the resource.</span></span>

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
