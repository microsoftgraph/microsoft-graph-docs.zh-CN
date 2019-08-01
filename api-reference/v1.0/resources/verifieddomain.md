---
title: verifiedDomain 资源类型
description: 指定租户的域。 组织实体的**verifiedDomains**属性是**VerifiedDomain**的集合。
localization_priority: Normal
author: ''
ms.prod: ''
doc_type: resourcePageType
ms.openlocfilehash: 758d76bd5e1eb577223a41e4e0452179d8bdafc7
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36033458"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="4206c-104">verifiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="4206c-104">verifiedDomain resource type</span></span>

<span data-ttu-id="4206c-105">指定租户的域。</span><span class="sxs-lookup"><span data-stu-id="4206c-105">Specifies a domain for a tenant.</span></span> <span data-ttu-id="4206c-106">[组织](organization.md)实体的**VerifiedDomains**属性是**VerifiedDomain**的集合。</span><span class="sxs-lookup"><span data-stu-id="4206c-106">The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="4206c-107">属性</span><span class="sxs-lookup"><span data-stu-id="4206c-107">Properties</span></span>
| <span data-ttu-id="4206c-108">属性</span><span class="sxs-lookup"><span data-stu-id="4206c-108">Property</span></span>     | <span data-ttu-id="4206c-109">类型</span><span class="sxs-lookup"><span data-stu-id="4206c-109">Type</span></span>   |<span data-ttu-id="4206c-110">说明</span><span class="sxs-lookup"><span data-stu-id="4206c-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4206c-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="4206c-111">capabilities</span></span>|<span data-ttu-id="4206c-112">String</span><span class="sxs-lookup"><span data-stu-id="4206c-112">String</span></span>|<span data-ttu-id="4206c-113">例如，“Email”、“OfficeCommunicationsOnline”。</span><span class="sxs-lookup"><span data-stu-id="4206c-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="4206c-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="4206c-114">isDefault</span></span>|<span data-ttu-id="4206c-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="4206c-115">Boolean</span></span>|                <span data-ttu-id="4206c-116">如果这是与租户关联的默认域，则为 **true**；否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="4206c-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="4206c-117">isInitial</span><span class="sxs-lookup"><span data-stu-id="4206c-117">isInitial</span></span>|<span data-ttu-id="4206c-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="4206c-118">Boolean</span></span>|<span data-ttu-id="4206c-119">如果这是与租户关联的初始域，则为 **true**；否则为 **false**</span><span class="sxs-lookup"><span data-stu-id="4206c-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="4206c-120">name</span><span class="sxs-lookup"><span data-stu-id="4206c-120">name</span></span>|<span data-ttu-id="4206c-121">String</span><span class="sxs-lookup"><span data-stu-id="4206c-121">String</span></span>|<span data-ttu-id="4206c-122">域名；例如，“contoso.onmicrosoft.com”</span><span class="sxs-lookup"><span data-stu-id="4206c-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="4206c-123">type</span><span class="sxs-lookup"><span data-stu-id="4206c-123">type</span></span>|<span data-ttu-id="4206c-124">String</span><span class="sxs-lookup"><span data-stu-id="4206c-124">String</span></span>|<span data-ttu-id="4206c-125">例如，“Managed”。</span><span class="sxs-lookup"><span data-stu-id="4206c-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4206c-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="4206c-126">JSON representation</span></span>

<span data-ttu-id="4206c-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4206c-127">Here is a JSON representation of the resource</span></span>

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
