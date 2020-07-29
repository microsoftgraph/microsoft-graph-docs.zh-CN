---
title: azureActiveDirectoryTenant 资源类型
description: AzureActiveDirectoryTenant 类型将另一个 Azure Active Directory 租户标识为连接的组织的标识源。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 881454f9658ae266705804518c3b5d8a876861eb
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46510144"
---
# <a name="azureactivedirectorytenant-resource-type"></a><span data-ttu-id="c1954-103">azureActiveDirectoryTenant 资源类型</span><span class="sxs-lookup"><span data-stu-id="c1954-103">azureActiveDirectoryTenant resource type</span></span>

<span data-ttu-id="c1954-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1954-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1954-105">在[connectedOrganization](connectedOrganization.md)的标识源中使用。</span><span class="sxs-lookup"><span data-stu-id="c1954-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="c1954-106">`@odata.type`该值 `#microsoft.graph.azureActiveDirectoryTenant` 指示此类型将另一个 Azure Active Directory 租户标识为连接的组织的标识源。</span><span class="sxs-lookup"><span data-stu-id="c1954-106">The `@odata.type` value `#microsoft.graph.azureActiveDirectoryTenant` indicates that this type identifies another Azure Active Directory tenant as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="c1954-107">属性</span><span class="sxs-lookup"><span data-stu-id="c1954-107">Properties</span></span>

| <span data-ttu-id="c1954-108">属性</span><span class="sxs-lookup"><span data-stu-id="c1954-108">Property</span></span>                     | <span data-ttu-id="c1954-109">类型</span><span class="sxs-lookup"><span data-stu-id="c1954-109">Type</span></span>                      | <span data-ttu-id="c1954-110">说明</span><span class="sxs-lookup"><span data-stu-id="c1954-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="c1954-111">displayName</span><span class="sxs-lookup"><span data-stu-id="c1954-111">displayName</span></span> |<span data-ttu-id="c1954-112">String</span><span class="sxs-lookup"><span data-stu-id="c1954-112">String</span></span> | <span data-ttu-id="c1954-113">Azure Active Directory 租户的名称。</span><span class="sxs-lookup"><span data-stu-id="c1954-113">The name of the Azure Active Directory tenant.</span></span> <span data-ttu-id="c1954-114">只读。</span><span class="sxs-lookup"><span data-stu-id="c1954-114">Read only.</span></span> |
| <span data-ttu-id="c1954-115">tenantId</span><span class="sxs-lookup"><span data-stu-id="c1954-115">tenantId</span></span> |<span data-ttu-id="c1954-116">字符串</span><span class="sxs-lookup"><span data-stu-id="c1954-116">String</span></span> | <span data-ttu-id="c1954-117">Azure Active Directory 租户的 ID。</span><span class="sxs-lookup"><span data-stu-id="c1954-117">The ID of the Azure Active Directory tenant.</span></span> <span data-ttu-id="c1954-118">只读。</span><span class="sxs-lookup"><span data-stu-id="c1954-118">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="c1954-119">关系</span><span class="sxs-lookup"><span data-stu-id="c1954-119">Relationships</span></span>

<span data-ttu-id="c1954-120">无。</span><span class="sxs-lookup"><span data-stu-id="c1954-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="c1954-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c1954-121">JSON representation</span></span>

<span data-ttu-id="c1954-122">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c1954-122">The following is a JSON representation of the type.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.azureActiveDirectoryTenant",
  "baseType": "microsoft.graph.identitySource"
}-->

```json
{
  "tenantId": "String (identifier)",
  "displayName": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "azureActiveDirectoryTenant resource type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
