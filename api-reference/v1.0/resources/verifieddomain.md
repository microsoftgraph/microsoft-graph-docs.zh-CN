---
title: verifiedDomain 资源类型
description: 指定租户的域。 组织 **实体的 verifiedDomains** 属性是 **VerifiedDomain 的集合**。
localization_priority: Normal
author: davidmu1
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: e2d26cd5e74499b5f2a086dfaa0ca9e9cbf4a4d8
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135546"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="9e9c5-104">verifiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e9c5-104">verifiedDomain resource type</span></span>

<span data-ttu-id="9e9c5-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9e9c5-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9e9c5-106">指定租户的域。</span><span class="sxs-lookup"><span data-stu-id="9e9c5-106">Specifies a domain for a tenant.</span></span> <span data-ttu-id="9e9c5-107">组织 **实体的 verifiedDomains** 属性是 **VerifiedDomain 的集合**。 [](organization.md)</span><span class="sxs-lookup"><span data-stu-id="9e9c5-107">The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="9e9c5-108">属性</span><span class="sxs-lookup"><span data-stu-id="9e9c5-108">Properties</span></span>
| <span data-ttu-id="9e9c5-109">属性</span><span class="sxs-lookup"><span data-stu-id="9e9c5-109">Property</span></span>     | <span data-ttu-id="9e9c5-110">类型</span><span class="sxs-lookup"><span data-stu-id="9e9c5-110">Type</span></span>   |<span data-ttu-id="9e9c5-111">说明</span><span class="sxs-lookup"><span data-stu-id="9e9c5-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9e9c5-112">capabilities</span><span class="sxs-lookup"><span data-stu-id="9e9c5-112">capabilities</span></span>|<span data-ttu-id="9e9c5-113">String</span><span class="sxs-lookup"><span data-stu-id="9e9c5-113">String</span></span>|<span data-ttu-id="9e9c5-114">例如，“Email”、“OfficeCommunicationsOnline”。</span><span class="sxs-lookup"><span data-stu-id="9e9c5-114">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="9e9c5-115">isDefault</span><span class="sxs-lookup"><span data-stu-id="9e9c5-115">isDefault</span></span>|<span data-ttu-id="9e9c5-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e9c5-116">Boolean</span></span>|                <span data-ttu-id="9e9c5-117">如果这是与租户关联的默认域，则为 **true**；否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="9e9c5-117">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="9e9c5-118">isInitial</span><span class="sxs-lookup"><span data-stu-id="9e9c5-118">isInitial</span></span>|<span data-ttu-id="9e9c5-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="9e9c5-119">Boolean</span></span>|<span data-ttu-id="9e9c5-120">如果这是与租户关联的初始域，则为 **true**；否则为 **false**</span><span class="sxs-lookup"><span data-stu-id="9e9c5-120">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="9e9c5-121">name</span><span class="sxs-lookup"><span data-stu-id="9e9c5-121">name</span></span>|<span data-ttu-id="9e9c5-122">String</span><span class="sxs-lookup"><span data-stu-id="9e9c5-122">String</span></span>|<span data-ttu-id="9e9c5-123">域名；例如，“contoso.onmicrosoft.com”</span><span class="sxs-lookup"><span data-stu-id="9e9c5-123">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="9e9c5-124">type</span><span class="sxs-lookup"><span data-stu-id="9e9c5-124">type</span></span>|<span data-ttu-id="9e9c5-125">String</span><span class="sxs-lookup"><span data-stu-id="9e9c5-125">String</span></span>|<span data-ttu-id="9e9c5-126">例如，“Managed”。</span><span class="sxs-lookup"><span data-stu-id="9e9c5-126">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="9e9c5-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e9c5-127">JSON representation</span></span>

<span data-ttu-id="9e9c5-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e9c5-128">Here is a JSON representation of the resource</span></span>

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

