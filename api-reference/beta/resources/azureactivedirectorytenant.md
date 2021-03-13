---
title: azureActiveDirectoryTenant 资源类型
description: azureActiveDirectoryTenant 类型将另一个 Azure Active Directory 租户标识为已连接组织的标识源。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: acd59c82f1968cbb161b74d1e7c1a551b6b2e397
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50759907"
---
# <a name="azureactivedirectorytenant-resource-type"></a><span data-ttu-id="9bc0f-103">azureActiveDirectoryTenant 资源类型</span><span class="sxs-lookup"><span data-stu-id="9bc0f-103">azureActiveDirectoryTenant resource type</span></span>

<span data-ttu-id="9bc0f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9bc0f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9bc0f-105">在 [connectedOrganization 的标识源中使用](connectedOrganization.md)。</span><span class="sxs-lookup"><span data-stu-id="9bc0f-105">Used in the identity sources of an [connectedOrganization](connectedOrganization.md).</span></span> <span data-ttu-id="9bc0f-106">该值 `@odata.type` `#microsoft.graph.azureActiveDirectoryTenant` 指示此类型将另一个 Azure Active Directory 租户标识为已连接组织的标识源。</span><span class="sxs-lookup"><span data-stu-id="9bc0f-106">The `@odata.type` value `#microsoft.graph.azureActiveDirectoryTenant` indicates that this type identifies another Azure Active Directory tenant as an identity source for a connected organization.</span></span>

## <a name="properties"></a><span data-ttu-id="9bc0f-107">属性</span><span class="sxs-lookup"><span data-stu-id="9bc0f-107">Properties</span></span>

| <span data-ttu-id="9bc0f-108">属性</span><span class="sxs-lookup"><span data-stu-id="9bc0f-108">Property</span></span>                     | <span data-ttu-id="9bc0f-109">类型</span><span class="sxs-lookup"><span data-stu-id="9bc0f-109">Type</span></span>                      | <span data-ttu-id="9bc0f-110">说明</span><span class="sxs-lookup"><span data-stu-id="9bc0f-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="9bc0f-111">displayName</span><span class="sxs-lookup"><span data-stu-id="9bc0f-111">displayName</span></span> |<span data-ttu-id="9bc0f-112">String</span><span class="sxs-lookup"><span data-stu-id="9bc0f-112">String</span></span> | <span data-ttu-id="9bc0f-113">Azure Active Directory 租户的名称。</span><span class="sxs-lookup"><span data-stu-id="9bc0f-113">The name of the Azure Active Directory tenant.</span></span> <span data-ttu-id="9bc0f-114">只读。</span><span class="sxs-lookup"><span data-stu-id="9bc0f-114">Read only.</span></span> |
| <span data-ttu-id="9bc0f-115">tenantId</span><span class="sxs-lookup"><span data-stu-id="9bc0f-115">tenantId</span></span> |<span data-ttu-id="9bc0f-116">String</span><span class="sxs-lookup"><span data-stu-id="9bc0f-116">String</span></span> | <span data-ttu-id="9bc0f-117">Azure Active Directory 租户的 ID。</span><span class="sxs-lookup"><span data-stu-id="9bc0f-117">The ID of the Azure Active Directory tenant.</span></span> <span data-ttu-id="9bc0f-118">只读。</span><span class="sxs-lookup"><span data-stu-id="9bc0f-118">Read only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="9bc0f-119">关系</span><span class="sxs-lookup"><span data-stu-id="9bc0f-119">Relationships</span></span>

<span data-ttu-id="9bc0f-120">无。</span><span class="sxs-lookup"><span data-stu-id="9bc0f-120">None.</span></span>

## <a name="json-representation"></a><span data-ttu-id="9bc0f-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9bc0f-121">JSON representation</span></span>

<span data-ttu-id="9bc0f-122">以下是类型的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9bc0f-122">The following is a JSON representation of the type.</span></span>

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


