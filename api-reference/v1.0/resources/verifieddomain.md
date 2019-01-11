---
title: verifiedDomain 资源类型
description: 指定租户的域。组织 实体的 **verifiedDomains** 属性是一个 **VerifiedDomain** 集合。
localization_priority: Normal
ms.openlocfilehash: 6eb6490ce8dac29f2617b7873230fad7c7b5c536
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876494"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="d650a-104">verifiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="d650a-104">verifiedDomain resource type</span></span>

<span data-ttu-id="d650a-p102">指定租户的域。[组织](organization.md) 实体的 **verifiedDomains** 属性是一个 **VerifiedDomain** 集合。</span><span class="sxs-lookup"><span data-stu-id="d650a-p102">Specifies a domain for a tenant. The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="d650a-107">属性</span><span class="sxs-lookup"><span data-stu-id="d650a-107">Properties</span></span>
| <span data-ttu-id="d650a-108">属性</span><span class="sxs-lookup"><span data-stu-id="d650a-108">Property</span></span>     | <span data-ttu-id="d650a-109">类型</span><span class="sxs-lookup"><span data-stu-id="d650a-109">Type</span></span>   |<span data-ttu-id="d650a-110">说明</span><span class="sxs-lookup"><span data-stu-id="d650a-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d650a-111">capabilities</span><span class="sxs-lookup"><span data-stu-id="d650a-111">capabilities</span></span>|<span data-ttu-id="d650a-112">String</span><span class="sxs-lookup"><span data-stu-id="d650a-112">String</span></span>|<span data-ttu-id="d650a-113">例如，“Email”、“OfficeCommunicationsOnline”。</span><span class="sxs-lookup"><span data-stu-id="d650a-113">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="d650a-114">isDefault</span><span class="sxs-lookup"><span data-stu-id="d650a-114">isDefault</span></span>|<span data-ttu-id="d650a-115">Boolean</span><span class="sxs-lookup"><span data-stu-id="d650a-115">Boolean</span></span>|                <span data-ttu-id="d650a-116">如果这是与租户关联的默认域，则为 **true**；否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="d650a-116">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="d650a-117">isInitial</span><span class="sxs-lookup"><span data-stu-id="d650a-117">isInitial</span></span>|<span data-ttu-id="d650a-118">Boolean</span><span class="sxs-lookup"><span data-stu-id="d650a-118">Boolean</span></span>|<span data-ttu-id="d650a-119">如果这是与租户关联的初始域，则为 **true**；否则为 **false**</span><span class="sxs-lookup"><span data-stu-id="d650a-119">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="d650a-120">name</span><span class="sxs-lookup"><span data-stu-id="d650a-120">name</span></span>|<span data-ttu-id="d650a-121">String</span><span class="sxs-lookup"><span data-stu-id="d650a-121">String</span></span>|<span data-ttu-id="d650a-122">域名；例如，“contoso.onmicrosoft.com”</span><span class="sxs-lookup"><span data-stu-id="d650a-122">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="d650a-123">type</span><span class="sxs-lookup"><span data-stu-id="d650a-123">type</span></span>|<span data-ttu-id="d650a-124">String</span><span class="sxs-lookup"><span data-stu-id="d650a-124">String</span></span>|<span data-ttu-id="d650a-125">例如，“Managed”。</span><span class="sxs-lookup"><span data-stu-id="d650a-125">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="d650a-126">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d650a-126">JSON representation</span></span>

<span data-ttu-id="d650a-127">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d650a-127">Here is a JSON representation of the resource</span></span>

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
