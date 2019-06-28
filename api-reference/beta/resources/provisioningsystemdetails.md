---
title: provisioningSystemDetails 资源类型
description: 表示用户预配或来自的系统。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e84af77ac7d2b14fb25ce07939bc1a542102fb19
ms.sourcegitcommit: e0de4e41773e361752870411d1b1a74270738127
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/28/2019
ms.locfileid: "35349351"
---
# <a name="provisioningsystemdetails-resource-type"></a><span data-ttu-id="52aa8-103">provisioningSystemDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="52aa8-103">provisioningSystemDetails resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="52aa8-104">表示用户预配或来自的系统。</span><span class="sxs-lookup"><span data-stu-id="52aa8-104">Represents the system that a user was provisioned to or from.</span></span> <span data-ttu-id="52aa8-105">例如, 在将用户从 Azure Active Directory (Azure AD) 设置为 ServiceNow 时, 源系统为 Azure AD, 目标系统为 ServiceNow。</span><span class="sxs-lookup"><span data-stu-id="52aa8-105">For example, when provisioning a user from Azure Active Directory (Azure AD) to ServiceNow, the source system is Azure AD, and the target system is ServiceNow.</span></span>

## <a name="properties"></a><span data-ttu-id="52aa8-106">属性</span><span class="sxs-lookup"><span data-stu-id="52aa8-106">Properties</span></span>

| <span data-ttu-id="52aa8-107">属性</span><span class="sxs-lookup"><span data-stu-id="52aa8-107">Property</span></span>     | <span data-ttu-id="52aa8-108">类型</span><span class="sxs-lookup"><span data-stu-id="52aa8-108">Type</span></span>        | <span data-ttu-id="52aa8-109">说明</span><span class="sxs-lookup"><span data-stu-id="52aa8-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="52aa8-110">详细信息</span><span class="sxs-lookup"><span data-stu-id="52aa8-110">details</span></span>|[<span data-ttu-id="52aa8-111">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="52aa8-111">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="52aa8-112">系统的详细信息。</span><span class="sxs-lookup"><span data-stu-id="52aa8-112">Details of the system.</span></span>|
|<span data-ttu-id="52aa8-113">displayName</span><span class="sxs-lookup"><span data-stu-id="52aa8-113">displayName</span></span>|<span data-ttu-id="52aa8-114">String</span><span class="sxs-lookup"><span data-stu-id="52aa8-114">String</span></span>|<span data-ttu-id="52aa8-115">用户预配或来自的系统的名称。</span><span class="sxs-lookup"><span data-stu-id="52aa8-115">Name of the system that a user was provisioned to or from.</span></span>|
|<span data-ttu-id="52aa8-116">id</span><span class="sxs-lookup"><span data-stu-id="52aa8-116">id</span></span>|<span data-ttu-id="52aa8-117">String</span><span class="sxs-lookup"><span data-stu-id="52aa8-117">String</span></span>|<span data-ttu-id="52aa8-118">用户预配或来自的系统的标识符。</span><span class="sxs-lookup"><span data-stu-id="52aa8-118">Identifier of the system that a user was provisioned to or from.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="52aa8-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="52aa8-119">JSON representation</span></span>

<span data-ttu-id="52aa8-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="52aa8-120">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.provisioningSystemDetails",
  "baseType": null
}-->

```json
{
  "details": {"@odata.type": "microsoft.graph.detailsInfo"},
  "displayName": "String",
  "id": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "provisioningSystemDetails resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
