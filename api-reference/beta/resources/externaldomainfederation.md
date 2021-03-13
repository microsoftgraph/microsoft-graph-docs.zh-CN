---
title: externalDomainFederation 资源类型
description: externalDomainFederation 类型将已配置的标识提供程序标识为已连接组织的标识源的非租户域。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: df88fef22c2acb86cadcfaed9a8f5be25da70f9d
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760986"
---
# <a name="externaldomainfederation-resource-type"></a><span data-ttu-id="9db68-103">externalDomainFederation 资源类型</span><span class="sxs-lookup"><span data-stu-id="9db68-103">externalDomainFederation resource type</span></span>

<span data-ttu-id="9db68-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9db68-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9db68-105">在 [connectedOrganization 的标识源中使用](connectedOrganization.md)。</span><span class="sxs-lookup"><span data-stu-id="9db68-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="9db68-106">`@odata.type`该值指示此类型将已配置的标识提供程序标识为已连接组织的标识 `#microsoft.graph.externalDomainFederation` 源的域。</span><span class="sxs-lookup"><span data-stu-id="9db68-106">The `@odata.type` value `#microsoft.graph.externalDomainFederation` indicates that this type identifies a domain with a configured identity provider as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="9db68-107">属性</span><span class="sxs-lookup"><span data-stu-id="9db68-107">Properties</span></span>

| <span data-ttu-id="9db68-108">属性</span><span class="sxs-lookup"><span data-stu-id="9db68-108">Property</span></span>                     | <span data-ttu-id="9db68-109">类型</span><span class="sxs-lookup"><span data-stu-id="9db68-109">Type</span></span>                      | <span data-ttu-id="9db68-110">说明</span><span class="sxs-lookup"><span data-stu-id="9db68-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="9db68-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9db68-111">displayName</span></span> |<span data-ttu-id="9db68-112">String</span><span class="sxs-lookup"><span data-stu-id="9db68-112">String</span></span> | <span data-ttu-id="9db68-113">标识源的名称，通常也是域名。</span><span class="sxs-lookup"><span data-stu-id="9db68-113">The name of the identity source, typically also the domain name.</span></span> <span data-ttu-id="9db68-114">只读。</span><span class="sxs-lookup"><span data-stu-id="9db68-114">Read only.</span></span> |
| <span data-ttu-id="9db68-115">domainName</span><span class="sxs-lookup"><span data-stu-id="9db68-115">domainName</span></span> |<span data-ttu-id="9db68-116">String</span><span class="sxs-lookup"><span data-stu-id="9db68-116">String</span></span> | <span data-ttu-id="9db68-117">域名。</span><span class="sxs-lookup"><span data-stu-id="9db68-117">The domain name.</span></span> <span data-ttu-id="9db68-118">只读。</span><span class="sxs-lookup"><span data-stu-id="9db68-118">Read only.</span></span> |
| <span data-ttu-id="9db68-119">issuerUri</span><span class="sxs-lookup"><span data-stu-id="9db68-119">issuerUri</span></span> |<span data-ttu-id="9db68-120">String</span><span class="sxs-lookup"><span data-stu-id="9db68-120">String</span></span> | <span data-ttu-id="9db68-121">传入联盟的 issuerURI。</span><span class="sxs-lookup"><span data-stu-id="9db68-121">The issuerURI of the incoming federation.</span></span> <span data-ttu-id="9db68-122">只读。</span><span class="sxs-lookup"><span data-stu-id="9db68-122">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9db68-123">关系</span><span class="sxs-lookup"><span data-stu-id="9db68-123">Relationships</span></span>

<span data-ttu-id="9db68-124">无。</span><span class="sxs-lookup"><span data-stu-id="9db68-124">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9db68-125">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9db68-125">JSON representation</span></span>

<span data-ttu-id="9db68-126">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9db68-126">The following is a JSON representation of the type.</span></span>

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


