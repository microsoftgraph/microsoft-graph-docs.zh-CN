---
title: verifiedDomain 资源类型
description: 指定租户的域。组织 实体的 **verifiedDomains** 属性是一个 **VerifiedDomain** 集合。
localization_priority: Normal
ms.openlocfilehash: 01e2d174f47d08bea4de9d582ffd6126002e8f1f
ms.sourcegitcommit: 66066b71d353fd7c2481d43b1dba2c33390eee61
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2019
ms.locfileid: "29576869"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="182ae-104">verifiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="182ae-104">verifiedDomain resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="182ae-p102">指定租户的域。[组织](organization.md) 实体的 **verifiedDomains** 属性是一个 **VerifiedDomain** 集合。</span><span class="sxs-lookup"><span data-stu-id="182ae-p102">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="182ae-107">属性</span><span class="sxs-lookup"><span data-stu-id="182ae-107">Properties</span></span>
| <span data-ttu-id="182ae-108">属性</span><span class="sxs-lookup"><span data-stu-id="182ae-108">Property</span></span>     | <span data-ttu-id="182ae-109">类型</span><span class="sxs-lookup"><span data-stu-id="182ae-109">Type</span></span>   |<span data-ttu-id="182ae-110">说明</span><span class="sxs-lookup"><span data-stu-id="182ae-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="182ae-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="182ae-111">capabilities</span></span>|<span data-ttu-id="182ae-112">String</span><span class="sxs-lookup"><span data-stu-id="182ae-112">String</span></span>|<span data-ttu-id="182ae-113">例如，“Email”、“OfficeCommunicationsOnline”。</span><span class="sxs-lookup"><span data-stu-id="182ae-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="182ae-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="182ae-114">isDefault</span></span>|<span data-ttu-id="182ae-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="182ae-115">Boolean</span></span>|                <span data-ttu-id="182ae-116">如果这是与租户关联的默认域，则为 **true**；否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="182ae-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="182ae-117">isInitial</span><span class="sxs-lookup"><span data-stu-id="182ae-117">isInitial</span></span>|<span data-ttu-id="182ae-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="182ae-118">Boolean</span></span>|<span data-ttu-id="182ae-119">如果这是与租户关联的初始域，则为 **true**；否则为 **false**</span><span class="sxs-lookup"><span data-stu-id="182ae-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="182ae-120">name</span><span class="sxs-lookup"><span data-stu-id="182ae-120">name</span></span>|<span data-ttu-id="182ae-121">String</span><span class="sxs-lookup"><span data-stu-id="182ae-121">String</span></span>|<span data-ttu-id="182ae-122">域名；例如，“contoso.onmicrosoft.com”</span><span class="sxs-lookup"><span data-stu-id="182ae-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="182ae-123">type</span><span class="sxs-lookup"><span data-stu-id="182ae-123">type</span></span>|<span data-ttu-id="182ae-124">String</span><span class="sxs-lookup"><span data-stu-id="182ae-124">String</span></span>|<span data-ttu-id="182ae-125">例如，“Managed”。</span><span class="sxs-lookup"><span data-stu-id="182ae-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="182ae-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="182ae-126">JSON representation</span></span>

<span data-ttu-id="182ae-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="182ae-127">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifiedDomain"
}-->

```json
{
  "capabilities": "string",
  "isDefault": true,
  "isInitial": true,
  "name": "string",
  "type": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/verifieddomain.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
