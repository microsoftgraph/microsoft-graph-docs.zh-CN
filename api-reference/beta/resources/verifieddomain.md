---
title: verifiedDomain 资源类型
description: 指定租户的域。 组织 **实体的 verifiedDomains** 属性是 **VerifiedDomain 的集合**。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: directory-management
author: davidmu1
ms.openlocfilehash: 2c4e833042a7bca3f3b85d3c9eb15bd7eb12925d
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135847"
---
# <a name="verifieddomain-resource-type"></a><span data-ttu-id="de850-104">verifiedDomain 资源类型</span><span class="sxs-lookup"><span data-stu-id="de850-104">verifiedDomain resource type</span></span>

<span data-ttu-id="de850-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="de850-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de850-106">指定租户的域。</span><span class="sxs-lookup"><span data-stu-id="de850-106">Specifies a domain for a tenant.</span></span> <span data-ttu-id="de850-107">组织 **实体的 verifiedDomains** 属性是 **VerifiedDomain 的集合**。 [](organization.md)</span><span class="sxs-lookup"><span data-stu-id="de850-107">The **verifiedDomains** property of the [organization](organization.md) entity is a collection of **VerifiedDomain**.</span></span>


## <a name="properties"></a><span data-ttu-id="de850-108">属性</span><span class="sxs-lookup"><span data-stu-id="de850-108">Properties</span></span>
| <span data-ttu-id="de850-109">属性</span><span class="sxs-lookup"><span data-stu-id="de850-109">Property</span></span>     | <span data-ttu-id="de850-110">类型</span><span class="sxs-lookup"><span data-stu-id="de850-110">Type</span></span>   |<span data-ttu-id="de850-111">说明</span><span class="sxs-lookup"><span data-stu-id="de850-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="de850-112">capabilities</span><span class="sxs-lookup"><span data-stu-id="de850-112">capabilities</span></span>|<span data-ttu-id="de850-113">String</span><span class="sxs-lookup"><span data-stu-id="de850-113">String</span></span>|<span data-ttu-id="de850-114">例如，“Email”、“OfficeCommunicationsOnline”。</span><span class="sxs-lookup"><span data-stu-id="de850-114">For example, “Email”, “OfficeCommunicationsOnline”.</span></span>|
|<span data-ttu-id="de850-115">isDefault</span><span class="sxs-lookup"><span data-stu-id="de850-115">isDefault</span></span>|<span data-ttu-id="de850-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="de850-116">Boolean</span></span>|                <span data-ttu-id="de850-117">如果这是与租户关联的默认域，则为 **true**；否则为 **false**。</span><span class="sxs-lookup"><span data-stu-id="de850-117">**true** if this is the default domain associated with the tenant; otherwise, **false**.</span></span>            |
|<span data-ttu-id="de850-118">isInitial</span><span class="sxs-lookup"><span data-stu-id="de850-118">isInitial</span></span>|<span data-ttu-id="de850-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="de850-119">Boolean</span></span>|<span data-ttu-id="de850-120">如果这是与租户关联的初始域，则为 **true**；否则为 **false**</span><span class="sxs-lookup"><span data-stu-id="de850-120">**true** if this is the initial domain associated with the tenant; otherwise, **false**</span></span>|
|<span data-ttu-id="de850-121">name</span><span class="sxs-lookup"><span data-stu-id="de850-121">name</span></span>|<span data-ttu-id="de850-122">字符串</span><span class="sxs-lookup"><span data-stu-id="de850-122">String</span></span>|<span data-ttu-id="de850-123">域名；例如，“contoso.onmicrosoft.com”</span><span class="sxs-lookup"><span data-stu-id="de850-123">The domain name; for example, “contoso.onmicrosoft.com”</span></span>|
|<span data-ttu-id="de850-124">type</span><span class="sxs-lookup"><span data-stu-id="de850-124">type</span></span>|<span data-ttu-id="de850-125">字符串</span><span class="sxs-lookup"><span data-stu-id="de850-125">String</span></span>|<span data-ttu-id="de850-126">例如，“Managed”。</span><span class="sxs-lookup"><span data-stu-id="de850-126">For example, “Managed”.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="de850-127">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="de850-127">JSON representation</span></span>

<span data-ttu-id="de850-128">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de850-128">Here is a JSON representation of the resource</span></span>

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
  "suppressions": []
}
-->


