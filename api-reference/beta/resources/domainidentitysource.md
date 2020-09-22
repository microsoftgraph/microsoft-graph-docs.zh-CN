---
title: domainIdentitySource 资源类型
description: DomainIdentitySource 类型将非租户域标识为连接的组织的标识源。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 63301dbf42a4589fd204290c157c6e6f63e473d2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48010304"
---
# <a name="domainidentitysource-resource-type"></a><span data-ttu-id="62cc8-103">domainIdentitySource 资源类型</span><span class="sxs-lookup"><span data-stu-id="62cc8-103">domainIdentitySource resource type</span></span>

<span data-ttu-id="62cc8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62cc8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="62cc8-105">在 [connectedOrganization](connectedOrganization.md)的标识源中使用。</span><span class="sxs-lookup"><span data-stu-id="62cc8-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="62cc8-106">`@odata.type`该值 `#microsoft.graph.domainIdentitySource` 指示此类型将域标识为连接的组织的标识源。</span><span class="sxs-lookup"><span data-stu-id="62cc8-106">The `@odata.type` value `#microsoft.graph.domainIdentitySource` indicates that this type identifies a domain as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="62cc8-107">属性</span><span class="sxs-lookup"><span data-stu-id="62cc8-107">Properties</span></span>

| <span data-ttu-id="62cc8-108">属性</span><span class="sxs-lookup"><span data-stu-id="62cc8-108">Property</span></span>                     | <span data-ttu-id="62cc8-109">类型</span><span class="sxs-lookup"><span data-stu-id="62cc8-109">Type</span></span>                      | <span data-ttu-id="62cc8-110">说明</span><span class="sxs-lookup"><span data-stu-id="62cc8-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="62cc8-111">displayName</span><span class="sxs-lookup"><span data-stu-id="62cc8-111">displayName</span></span> |<span data-ttu-id="62cc8-112">String</span><span class="sxs-lookup"><span data-stu-id="62cc8-112">String</span></span> | <span data-ttu-id="62cc8-113">标识源的名称，通常也是域名。</span><span class="sxs-lookup"><span data-stu-id="62cc8-113">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="62cc8-114">只读。</span><span class="sxs-lookup"><span data-stu-id="62cc8-114">Read only.</span></span> |
| <span data-ttu-id="62cc8-115">domainName</span><span class="sxs-lookup"><span data-stu-id="62cc8-115">domainName</span></span> |<span data-ttu-id="62cc8-116">String</span><span class="sxs-lookup"><span data-stu-id="62cc8-116">String</span></span> | <span data-ttu-id="62cc8-117">域名称。</span><span class="sxs-lookup"><span data-stu-id="62cc8-117">The domain name.</span></span> <span data-ttu-id="62cc8-118">只读。</span><span class="sxs-lookup"><span data-stu-id="62cc8-118">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="62cc8-119">关系</span><span class="sxs-lookup"><span data-stu-id="62cc8-119">Relationships</span></span>

<span data-ttu-id="62cc8-120">无。</span><span class="sxs-lookup"><span data-stu-id="62cc8-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="62cc8-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="62cc8-121">JSON representation</span></span>

<span data-ttu-id="62cc8-122">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62cc8-122">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.domainIdentitySource",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "domainName": "String",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "domainIdentitySource resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


