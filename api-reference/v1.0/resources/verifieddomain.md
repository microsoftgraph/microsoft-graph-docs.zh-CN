---
title: verifiedDomain 资源类型
description: 指定租户的域。 组织实体的**verifiedDomains**属性是**VerifiedDomain**的集合。
localization_priority: Normal
ms.openlocfilehash: 6eb6490ce8dac29f2617b7873230fad7c7b5c536
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32456904"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="a86b8-104">verifiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="a86b8-104">verifiedDomain resource type</span></span>

<span data-ttu-id="a86b8-105">指定租户的域。</span><span class="sxs-lookup"><span data-stu-id="a86b8-105">Specifies a domain for a tenant.</span></span> <span data-ttu-id="a86b8-106">[组织](organization.md)实体的**verifiedDomains**属性是**VerifiedDomain**的集合。</span><span class="sxs-lookup"><span data-stu-id="a86b8-106">The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="a86b8-107">属性</span><span class="sxs-lookup"><span data-stu-id="a86b8-107">Properties</span></span>
| <span data-ttu-id="a86b8-108">属性</span><span class="sxs-lookup"><span data-stu-id="a86b8-108">Property</span></span>     | <span data-ttu-id="a86b8-109">类型</span><span class="sxs-lookup"><span data-stu-id="a86b8-109">Type</span></span>   |<span data-ttu-id="a86b8-110">说明</span><span class="sxs-lookup"><span data-stu-id="a86b8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="a86b8-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="a86b8-111">capabilities</span></span>|<span data-ttu-id="a86b8-112">String</span><span class="sxs-lookup"><span data-stu-id="a86b8-112">String</span></span>|<span data-ttu-id="a86b8-113">例如，“Email”、“OfficeCommunicationsOnline”。</span><span class="sxs-lookup"><span data-stu-id="a86b8-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="a86b8-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="a86b8-114">isDefault</span></span>|<span data-ttu-id="a86b8-115">布尔</span><span class="sxs-lookup"><span data-stu-id="a86b8-115">Boolean</span></span>|                <span data-ttu-id="a86b8-116">如果这是与租户关联的默认域，则为 **true**；否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="a86b8-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="a86b8-117">isInitial</span><span class="sxs-lookup"><span data-stu-id="a86b8-117">isInitial</span></span>|<span data-ttu-id="a86b8-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="a86b8-118">Boolean</span></span>|<span data-ttu-id="a86b8-119">如果这是与租户关联的初始域，则为 **true**；否则为 **false**</span><span class="sxs-lookup"><span data-stu-id="a86b8-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="a86b8-120">name</span><span class="sxs-lookup"><span data-stu-id="a86b8-120">name</span></span>|<span data-ttu-id="a86b8-121">String</span><span class="sxs-lookup"><span data-stu-id="a86b8-121">String</span></span>|<span data-ttu-id="a86b8-122">域名；例如，“contoso.onmicrosoft.com”</span><span class="sxs-lookup"><span data-stu-id="a86b8-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="a86b8-123">type</span><span class="sxs-lookup"><span data-stu-id="a86b8-123">type</span></span>|<span data-ttu-id="a86b8-124">String</span><span class="sxs-lookup"><span data-stu-id="a86b8-124">String</span></span>|<span data-ttu-id="a86b8-125">例如，“Managed”。</span><span class="sxs-lookup"><span data-stu-id="a86b8-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="a86b8-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a86b8-126">JSON representation</span></span>

<span data-ttu-id="a86b8-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a86b8-127">Here is a JSON representation of the resource</span></span>

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
