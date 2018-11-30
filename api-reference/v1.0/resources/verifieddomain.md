---
title: verifiedDomain 资源类型
description: 指定租户的域。组织 实体的 **verifiedDomains** 属性是一个 **VerifiedDomain** 集合。
ms.openlocfilehash: 21b6dd89dcc8b990046952d9ae7abcfe8ce02bca
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008981"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="05592-104">verifiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="05592-104">verifiedDomain resource type</span></span>

<span data-ttu-id="05592-p102">指定租户的域。[组织](organization.md) 实体的 **verifiedDomains** 属性是一个 **VerifiedDomain** 集合。</span><span class="sxs-lookup"><span data-stu-id="05592-p102">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="05592-107">属性</span><span class="sxs-lookup"><span data-stu-id="05592-107">Properties</span></span>
| <span data-ttu-id="05592-108">属性</span><span class="sxs-lookup"><span data-stu-id="05592-108">Property</span></span>     | <span data-ttu-id="05592-109">类型</span><span class="sxs-lookup"><span data-stu-id="05592-109">Type</span></span>   |<span data-ttu-id="05592-110">说明</span><span class="sxs-lookup"><span data-stu-id="05592-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="05592-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="05592-111">capabilities</span></span>|<span data-ttu-id="05592-112">String</span><span class="sxs-lookup"><span data-stu-id="05592-112">String</span></span>|<span data-ttu-id="05592-113">例如，“Email”、“OfficeCommunicationsOnline”。</span><span class="sxs-lookup"><span data-stu-id="05592-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="05592-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="05592-114">isDefault</span></span>|<span data-ttu-id="05592-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="05592-115">Boolean</span></span>|                <span data-ttu-id="05592-116">如果这是与租户关联的默认域，则为 **true**；否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="05592-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="05592-117">isInitial</span><span class="sxs-lookup"><span data-stu-id="05592-117">isInitial</span></span>|<span data-ttu-id="05592-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="05592-118">Boolean</span></span>|<span data-ttu-id="05592-119">如果这是与租户关联的初始域，则为 **true**；否则为 **false**</span><span class="sxs-lookup"><span data-stu-id="05592-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="05592-120">name</span><span class="sxs-lookup"><span data-stu-id="05592-120">name</span></span>|<span data-ttu-id="05592-121">String</span><span class="sxs-lookup"><span data-stu-id="05592-121">String</span></span>|<span data-ttu-id="05592-122">域名；例如，“contoso.onmicrosoft.com”</span><span class="sxs-lookup"><span data-stu-id="05592-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="05592-123">type</span><span class="sxs-lookup"><span data-stu-id="05592-123">type</span></span>|<span data-ttu-id="05592-124">String</span><span class="sxs-lookup"><span data-stu-id="05592-124">String</span></span>|<span data-ttu-id="05592-125">例如，“Managed”。</span><span class="sxs-lookup"><span data-stu-id="05592-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="05592-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="05592-126">JSON representation</span></span>

<span data-ttu-id="05592-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="05592-127">Here is a JSON representation of the resource</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "verifiedDomain resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
