---
title: externalDomainFederation 资源类型
description: ExternalDomainFederation 类型将具有配置的标识提供程序的非租户域标识为连接的组织的标识源。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: d81255a3687bf3d6aafe9369f901b209f5827b77
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48026913"
---
# <a name="externaldomainfederation-resource-type"></a><span data-ttu-id="af9e0-103">externalDomainFederation 资源类型</span><span class="sxs-lookup"><span data-stu-id="af9e0-103">externalDomainFederation resource type</span></span>

<span data-ttu-id="af9e0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="af9e0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="af9e0-105">在 [connectedOrganization](connectedOrganization.md)的标识源中使用。</span><span class="sxs-lookup"><span data-stu-id="af9e0-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="af9e0-106">`@odata.type`该值 `#microsoft.graph.externalDomainFederation` 指示此类型将具有已配置标识提供程序的域标识为连接的组织的标识源。</span><span class="sxs-lookup"><span data-stu-id="af9e0-106">The `@odata.type` value `#microsoft.graph.externalDomainFederation` indicates that this type identifies a domain with a configured identity provider as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="af9e0-107">属性</span><span class="sxs-lookup"><span data-stu-id="af9e0-107">Properties</span></span>

| <span data-ttu-id="af9e0-108">属性</span><span class="sxs-lookup"><span data-stu-id="af9e0-108">Property</span></span>                     | <span data-ttu-id="af9e0-109">类型</span><span class="sxs-lookup"><span data-stu-id="af9e0-109">Type</span></span>                      | <span data-ttu-id="af9e0-110">说明</span><span class="sxs-lookup"><span data-stu-id="af9e0-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="af9e0-111">displayName</span><span class="sxs-lookup"><span data-stu-id="af9e0-111">displayName</span></span> |<span data-ttu-id="af9e0-112">String</span><span class="sxs-lookup"><span data-stu-id="af9e0-112">String</span></span> | <span data-ttu-id="af9e0-113">标识源的名称，通常也是域名。</span><span class="sxs-lookup"><span data-stu-id="af9e0-113">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="af9e0-114">只读。</span><span class="sxs-lookup"><span data-stu-id="af9e0-114">Read only.</span></span> |
| <span data-ttu-id="af9e0-115">domainName</span><span class="sxs-lookup"><span data-stu-id="af9e0-115">domainName</span></span> |<span data-ttu-id="af9e0-116">String</span><span class="sxs-lookup"><span data-stu-id="af9e0-116">String</span></span> | <span data-ttu-id="af9e0-117">域名称。</span><span class="sxs-lookup"><span data-stu-id="af9e0-117">The domain name.</span></span> <span data-ttu-id="af9e0-118">只读。</span><span class="sxs-lookup"><span data-stu-id="af9e0-118">Read only.</span></span> |
| <span data-ttu-id="af9e0-119">issuerUri</span><span class="sxs-lookup"><span data-stu-id="af9e0-119">issuerUri</span></span> |<span data-ttu-id="af9e0-120">String</span><span class="sxs-lookup"><span data-stu-id="af9e0-120">String</span></span> | <span data-ttu-id="af9e0-121">传入联合身份验证的 issuerURI。</span><span class="sxs-lookup"><span data-stu-id="af9e0-121">The issuerURI of the incoming federation.</span></span> <span data-ttu-id="af9e0-122">只读。</span><span class="sxs-lookup"><span data-stu-id="af9e0-122">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="af9e0-123">关系</span><span class="sxs-lookup"><span data-stu-id="af9e0-123">Relationships</span></span>

<span data-ttu-id="af9e0-124">无。</span><span class="sxs-lookup"><span data-stu-id="af9e0-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="af9e0-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="af9e0-125">JSON representation</span></span>

<span data-ttu-id="af9e0-126">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="af9e0-126">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.externalDomainFederation",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "domainName": "String",
  "displayName": "String",
  "issuerUri": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "externalDomainFederation resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


