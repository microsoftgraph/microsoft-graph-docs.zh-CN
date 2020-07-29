---
title: externalDomainFederation 资源类型
description: ExternalDomainFederation 类型将具有配置的标识提供程序的非租户域标识为连接的组织的标识源。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: ffeaa955ac43a52a0e3485f4a561163d4d27a957
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510019"
---
# <a name="externaldomainfederation-resource-type"></a><span data-ttu-id="53eb5-103">externalDomainFederation 资源类型</span><span class="sxs-lookup"><span data-stu-id="53eb5-103">externalDomainFederation resource type</span></span>

<span data-ttu-id="53eb5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53eb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="53eb5-105">在[connectedOrganization](connectedOrganization.md)的标识源中使用。</span><span class="sxs-lookup"><span data-stu-id="53eb5-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="53eb5-106">`@odata.type`该值 `#microsoft.graph.externalDomainFederation` 指示此类型将具有已配置标识提供程序的域标识为连接的组织的标识源。</span><span class="sxs-lookup"><span data-stu-id="53eb5-106">The `@odata.type` value `#microsoft.graph.externalDomainFederation` indicates that this type identifies a domain with a configured identity provider as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="53eb5-107">属性</span><span class="sxs-lookup"><span data-stu-id="53eb5-107">Properties</span></span>

| <span data-ttu-id="53eb5-108">属性</span><span class="sxs-lookup"><span data-stu-id="53eb5-108">Property</span></span>                     | <span data-ttu-id="53eb5-109">类型</span><span class="sxs-lookup"><span data-stu-id="53eb5-109">Type</span></span>                      | <span data-ttu-id="53eb5-110">说明</span><span class="sxs-lookup"><span data-stu-id="53eb5-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="53eb5-111">displayName</span><span class="sxs-lookup"><span data-stu-id="53eb5-111">displayName</span></span> |<span data-ttu-id="53eb5-112">String</span><span class="sxs-lookup"><span data-stu-id="53eb5-112">String</span></span> | <span data-ttu-id="53eb5-113">标识源的名称，通常也是域名。</span><span class="sxs-lookup"><span data-stu-id="53eb5-113">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="53eb5-114">只读。</span><span class="sxs-lookup"><span data-stu-id="53eb5-114">Read only.</span></span> |
| <span data-ttu-id="53eb5-115">domainName</span><span class="sxs-lookup"><span data-stu-id="53eb5-115">domainName</span></span> |<span data-ttu-id="53eb5-116">String</span><span class="sxs-lookup"><span data-stu-id="53eb5-116">String</span></span> | <span data-ttu-id="53eb5-117">域名称。</span><span class="sxs-lookup"><span data-stu-id="53eb5-117">The domain name.</span></span> <span data-ttu-id="53eb5-118">只读。</span><span class="sxs-lookup"><span data-stu-id="53eb5-118">Read only.</span></span> |
| <span data-ttu-id="53eb5-119">issuerUri</span><span class="sxs-lookup"><span data-stu-id="53eb5-119">issuerUri</span></span> |<span data-ttu-id="53eb5-120">字符串</span><span class="sxs-lookup"><span data-stu-id="53eb5-120">String</span></span> | <span data-ttu-id="53eb5-121">传入联合身份验证的 issuerURI。</span><span class="sxs-lookup"><span data-stu-id="53eb5-121">The issuerURI of the incoming federation.</span></span> <span data-ttu-id="53eb5-122">只读。</span><span class="sxs-lookup"><span data-stu-id="53eb5-122">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="53eb5-123">关系</span><span class="sxs-lookup"><span data-stu-id="53eb5-123">Relationships</span></span>

<span data-ttu-id="53eb5-124">无。</span><span class="sxs-lookup"><span data-stu-id="53eb5-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="53eb5-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="53eb5-125">JSON representation</span></span>

<span data-ttu-id="53eb5-126">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53eb5-126">The following is a JSON representation of the type.</span></span>

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
