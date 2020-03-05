---
title: assignedLicense 资源类型
description: 表示分配给用户的许可证。 User 实体的**assignedLicenses**属性是**assignedLicense**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: b7d529b62155493655ceccb4db594a6d560ccf84
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508210"
---
# <a name="assignedlicense-resource-type"></a><span data-ttu-id="70916-104">assignedLicense 资源类型</span><span class="sxs-lookup"><span data-stu-id="70916-104">assignedLicense resource type</span></span>

<span data-ttu-id="70916-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="70916-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70916-106">表示分配给用户的许可证。</span><span class="sxs-lookup"><span data-stu-id="70916-106">Represents a license assigned to a user.</span></span> <span data-ttu-id="70916-107">[User](user.md)实体的**AssignedLicenses**属性是**assignedLicense**的集合。</span><span class="sxs-lookup"><span data-stu-id="70916-107">The **assignedLicenses** property of the [user](user.md) entity is a collection of **assignedLicense**.</span></span>

## <a name="properties"></a><span data-ttu-id="70916-108">属性</span><span class="sxs-lookup"><span data-stu-id="70916-108">Properties</span></span>
| <span data-ttu-id="70916-109">属性</span><span class="sxs-lookup"><span data-stu-id="70916-109">Property</span></span>     | <span data-ttu-id="70916-110">类型</span><span class="sxs-lookup"><span data-stu-id="70916-110">Type</span></span>   |<span data-ttu-id="70916-111">说明</span><span class="sxs-lookup"><span data-stu-id="70916-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="70916-112">disabledPlans</span><span class="sxs-lookup"><span data-stu-id="70916-112">disabledPlans</span></span>|<span data-ttu-id="70916-113">Guid 集合</span><span class="sxs-lookup"><span data-stu-id="70916-113">Guid collection</span></span>|<span data-ttu-id="70916-114">已禁用的计划的唯一标识符的集合。</span><span class="sxs-lookup"><span data-stu-id="70916-114">A collection of the unique identifiers for plans that have been disabled.</span></span>|
|<span data-ttu-id="70916-115">skuId</span><span class="sxs-lookup"><span data-stu-id="70916-115">skuId</span></span>|<span data-ttu-id="70916-116">Guid</span><span class="sxs-lookup"><span data-stu-id="70916-116">Guid</span></span>|<span data-ttu-id="70916-117">此 SKU 的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="70916-117">The unique identifier for the SKU.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="70916-118">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="70916-118">JSON representation</span></span>

<span data-ttu-id="70916-119">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70916-119">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.assignedLicense"
}-->

```json
{
  "disabledPlans": ["guid"],
  "skuId": "guid"
}

```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "assignedLicense resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
