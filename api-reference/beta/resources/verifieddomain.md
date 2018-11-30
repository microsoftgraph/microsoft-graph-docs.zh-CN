---
title: verifiedDomain 资源类型
description: 指定租户的域。组织 实体的 **verifiedDomains** 属性是一个 **VerifiedDomain** 集合。
ms.openlocfilehash: 810b5fea0fbaf82eeb452c0f5c6032679590ff49
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046763"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="2bd3b-104">verifiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="2bd3b-104">verifiedDomain resource type</span></span>

> <span data-ttu-id="2bd3b-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2bd3b-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2bd3b-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2bd3b-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2bd3b-p103">指定租户的域。[组织](organization.md) 实体的 **verifiedDomains** 属性是一个 **VerifiedDomain** 集合。</span><span class="sxs-lookup"><span data-stu-id="2bd3b-p103">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="2bd3b-109">属性</span><span class="sxs-lookup"><span data-stu-id="2bd3b-109">Properties</span></span>
| <span data-ttu-id="2bd3b-110">属性</span><span class="sxs-lookup"><span data-stu-id="2bd3b-110">Property</span></span>     | <span data-ttu-id="2bd3b-111">类型</span><span class="sxs-lookup"><span data-stu-id="2bd3b-111">Type</span></span>   |<span data-ttu-id="2bd3b-112">说明</span><span class="sxs-lookup"><span data-stu-id="2bd3b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2bd3b-113">capabilities</span><span class="sxs-lookup"><span data-stu-id="2bd3b-113">capabilities</span></span>|<span data-ttu-id="2bd3b-114">String</span><span class="sxs-lookup"><span data-stu-id="2bd3b-114">String</span></span>|<span data-ttu-id="2bd3b-115">例如，“Email”、“OfficeCommunicationsOnline”。</span><span class="sxs-lookup"><span data-stu-id="2bd3b-115">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="2bd3b-116">isDefault</span><span class="sxs-lookup"><span data-stu-id="2bd3b-116">isDefault</span></span>|<span data-ttu-id="2bd3b-117">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bd3b-117">Boolean</span></span>|                <span data-ttu-id="2bd3b-118">如果这是与租户关联的默认域，则为 **true**；否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="2bd3b-118">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="2bd3b-119">isInitial</span><span class="sxs-lookup"><span data-stu-id="2bd3b-119">isInitial</span></span>|<span data-ttu-id="2bd3b-120">Boolean</span><span class="sxs-lookup"><span data-stu-id="2bd3b-120">Boolean</span></span>|<span data-ttu-id="2bd3b-121">如果这是与租户关联的初始域，则为 **true**；否则为 **false**</span><span class="sxs-lookup"><span data-stu-id="2bd3b-121">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="2bd3b-122">name</span><span class="sxs-lookup"><span data-stu-id="2bd3b-122">name</span></span>|<span data-ttu-id="2bd3b-123">String</span><span class="sxs-lookup"><span data-stu-id="2bd3b-123">String</span></span>|<span data-ttu-id="2bd3b-124">域名；例如，“contoso.onmicrosoft.com”</span><span class="sxs-lookup"><span data-stu-id="2bd3b-124">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="2bd3b-125">type</span><span class="sxs-lookup"><span data-stu-id="2bd3b-125">type</span></span>|<span data-ttu-id="2bd3b-126">String</span><span class="sxs-lookup"><span data-stu-id="2bd3b-126">String</span></span>|<span data-ttu-id="2bd3b-127">例如，“Managed”。</span><span class="sxs-lookup"><span data-stu-id="2bd3b-127">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2bd3b-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2bd3b-128">JSON representation</span></span>

<span data-ttu-id="2bd3b-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2bd3b-129">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.verifieddomain"
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
