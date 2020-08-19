---
title: verifiedDomain 资源类型
description: 指定租户的域。 组织实体的 **verifiedDomains** 属性是 **VerifiedDomain**的集合。
localization_priority: Normal
author: davidmu1
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 656e4a4c8fc40c86eea3b3e167adae22a9580081
ms.sourcegitcommit: a6d284b3726139f11194aa3d23b8bb79165cc09e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/19/2020
ms.locfileid: "46807694"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="cd5bf-104">verifiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="cd5bf-104">verifiedDomain resource type</span></span>

<span data-ttu-id="cd5bf-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cd5bf-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cd5bf-106">指定租户的域。</span><span class="sxs-lookup"><span data-stu-id="cd5bf-106">Specifies a domain for a tenant.</span></span> <span data-ttu-id="cd5bf-107">[组织](organization.md)实体的**VerifiedDomains**属性是**VerifiedDomain**的集合。</span><span class="sxs-lookup"><span data-stu-id="cd5bf-107">The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="cd5bf-108">属性</span><span class="sxs-lookup"><span data-stu-id="cd5bf-108">Properties</span></span>
| <span data-ttu-id="cd5bf-109">属性</span><span class="sxs-lookup"><span data-stu-id="cd5bf-109">Property</span></span>     | <span data-ttu-id="cd5bf-110">类型</span><span class="sxs-lookup"><span data-stu-id="cd5bf-110">Type</span></span>   |<span data-ttu-id="cd5bf-111">说明</span><span class="sxs-lookup"><span data-stu-id="cd5bf-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="cd5bf-112">capabilities</span><span class="sxs-lookup"><span data-stu-id="cd5bf-112">capabilities</span></span>|<span data-ttu-id="cd5bf-113">String</span><span class="sxs-lookup"><span data-stu-id="cd5bf-113">String</span></span>|<span data-ttu-id="cd5bf-114">例如，“Email”、“OfficeCommunicationsOnline”。</span><span class="sxs-lookup"><span data-stu-id="cd5bf-114">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="cd5bf-115">isDefault</span><span class="sxs-lookup"><span data-stu-id="cd5bf-115">isDefault</span></span>|<span data-ttu-id="cd5bf-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd5bf-116">Boolean</span></span>|                <span data-ttu-id="cd5bf-117">如果这是与租户关联的默认域，则为 **true**；否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="cd5bf-117">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="cd5bf-118">isInitial</span><span class="sxs-lookup"><span data-stu-id="cd5bf-118">isInitial</span></span>|<span data-ttu-id="cd5bf-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="cd5bf-119">Boolean</span></span>|<span data-ttu-id="cd5bf-120">如果这是与租户关联的初始域，则为 **true**；否则为 **false**</span><span class="sxs-lookup"><span data-stu-id="cd5bf-120">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="cd5bf-121">name</span><span class="sxs-lookup"><span data-stu-id="cd5bf-121">name</span></span>|<span data-ttu-id="cd5bf-122">String</span><span class="sxs-lookup"><span data-stu-id="cd5bf-122">String</span></span>|<span data-ttu-id="cd5bf-123">域名；例如，“contoso.onmicrosoft.com”</span><span class="sxs-lookup"><span data-stu-id="cd5bf-123">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="cd5bf-124">type</span><span class="sxs-lookup"><span data-stu-id="cd5bf-124">type</span></span>|<span data-ttu-id="cd5bf-125">String</span><span class="sxs-lookup"><span data-stu-id="cd5bf-125">String</span></span>|<span data-ttu-id="cd5bf-126">例如，“Managed”。</span><span class="sxs-lookup"><span data-stu-id="cd5bf-126">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="cd5bf-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="cd5bf-127">JSON representation</span></span>

<span data-ttu-id="cd5bf-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cd5bf-128">Here is a JSON representation of the resource</span></span>

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
