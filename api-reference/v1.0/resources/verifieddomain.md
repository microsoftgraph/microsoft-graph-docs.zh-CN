---
title: verifiedDomain 资源类型
description: 指定租户的域。 **organization 实体的 verifiedDomains** 属性是 **VerifiedDomain 的集合**。
localization_priority: Normal
author: Jumaodhiss
ms.prod: directory-management
doc_type: resourcePageType
ms.openlocfilehash: 8636552fa99b3389f35f22e2edccc5d13cb06482
ms.sourcegitcommit: 8ca598ac70647bf4f897361ee90d3aa31d2ecca5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51468980"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="df339-104">verifiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="df339-104">verifiedDomain resource type</span></span>

<span data-ttu-id="df339-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df339-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="df339-106">指定租户的域。</span><span class="sxs-lookup"><span data-stu-id="df339-106">Specifies a domain for a tenant.</span></span> <span data-ttu-id="df339-107">**organization 实体的 verifiedDomains** 属性是 **VerifiedDomain 的集合**。 [](organization.md)</span><span class="sxs-lookup"><span data-stu-id="df339-107">The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="df339-108">属性</span><span class="sxs-lookup"><span data-stu-id="df339-108">Properties</span></span>
| <span data-ttu-id="df339-109">属性</span><span class="sxs-lookup"><span data-stu-id="df339-109">Property</span></span>     | <span data-ttu-id="df339-110">类型</span><span class="sxs-lookup"><span data-stu-id="df339-110">Type</span></span>   |<span data-ttu-id="df339-111">说明</span><span class="sxs-lookup"><span data-stu-id="df339-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="df339-112">capabilities</span><span class="sxs-lookup"><span data-stu-id="df339-112">capabilities</span></span>|<span data-ttu-id="df339-113">String</span><span class="sxs-lookup"><span data-stu-id="df339-113">String</span></span>|<span data-ttu-id="df339-114">例如，“Email”、“OfficeCommunicationsOnline”。</span><span class="sxs-lookup"><span data-stu-id="df339-114">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="df339-115">isDefault</span><span class="sxs-lookup"><span data-stu-id="df339-115">isDefault</span></span>|<span data-ttu-id="df339-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="df339-116">Boolean</span></span>|                <span data-ttu-id="df339-117">如果这是与租户关联的默认域，则为 **true**；否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="df339-117">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="df339-118">isInitial</span><span class="sxs-lookup"><span data-stu-id="df339-118">isInitial</span></span>|<span data-ttu-id="df339-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="df339-119">Boolean</span></span>|<span data-ttu-id="df339-120">如果这是与租户关联的初始域，则为 **true**；否则为 **false**</span><span class="sxs-lookup"><span data-stu-id="df339-120">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="df339-121">name</span><span class="sxs-lookup"><span data-stu-id="df339-121">name</span></span>|<span data-ttu-id="df339-122">String</span><span class="sxs-lookup"><span data-stu-id="df339-122">String</span></span>|<span data-ttu-id="df339-123">域名；例如，“contoso.onmicrosoft.com”</span><span class="sxs-lookup"><span data-stu-id="df339-123">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="df339-124">type</span><span class="sxs-lookup"><span data-stu-id="df339-124">type</span></span>|<span data-ttu-id="df339-125">String</span><span class="sxs-lookup"><span data-stu-id="df339-125">String</span></span>|<span data-ttu-id="df339-126">例如，“Managed”。</span><span class="sxs-lookup"><span data-stu-id="df339-126">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="df339-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="df339-127">JSON representation</span></span>

<span data-ttu-id="df339-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="df339-128">Here is a JSON representation of the resource</span></span>

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

