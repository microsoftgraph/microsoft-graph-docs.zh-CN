---
title: provisioningSystemDetails 资源类型
description: 表示用户已预配到或来自的系统。
localization_priority: Normal
author: ArvindHarinder1
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 5400088c1f239bd73e093679bbc13b8034800f28
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135336"
---
# <a name="provisioningsystemdetails-resource-type"></a><span data-ttu-id="364d6-103">provisioningSystemDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="364d6-103">provisioningSystemDetails resource type</span></span>

<span data-ttu-id="364d6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="364d6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="364d6-105">表示用户已预配到或来自的系统。</span><span class="sxs-lookup"><span data-stu-id="364d6-105">Represents the system that a user was provisioned to or from.</span></span> <span data-ttu-id="364d6-106">例如，将用户从 Azure Active Directory (Azure AD) 预配到 ServiceNow 时，源系统为 Azure AD，目标系统为 ServiceNow。</span><span class="sxs-lookup"><span data-stu-id="364d6-106">For example, when provisioning a user from Azure Active Directory (Azure AD) to ServiceNow, the source system is Azure AD, and the target system is ServiceNow.</span></span>

## <a name="properties"></a><span data-ttu-id="364d6-107">属性</span><span class="sxs-lookup"><span data-stu-id="364d6-107">Properties</span></span>

| <span data-ttu-id="364d6-108">属性</span><span class="sxs-lookup"><span data-stu-id="364d6-108">Property</span></span>     | <span data-ttu-id="364d6-109">类型</span><span class="sxs-lookup"><span data-stu-id="364d6-109">Type</span></span>        | <span data-ttu-id="364d6-110">说明</span><span class="sxs-lookup"><span data-stu-id="364d6-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="364d6-111">详细信息</span><span class="sxs-lookup"><span data-stu-id="364d6-111">details</span></span>|[<span data-ttu-id="364d6-112">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="364d6-112">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="364d6-113">系统的详细信息。</span><span class="sxs-lookup"><span data-stu-id="364d6-113">Details of the system.</span></span>|
|<span data-ttu-id="364d6-114">displayName</span><span class="sxs-lookup"><span data-stu-id="364d6-114">displayName</span></span>|<span data-ttu-id="364d6-115">字符串</span><span class="sxs-lookup"><span data-stu-id="364d6-115">String</span></span>|<span data-ttu-id="364d6-116">用户预配到或来自的系统的名称。</span><span class="sxs-lookup"><span data-stu-id="364d6-116">Name of the system that a user was provisioned to or from.</span></span>|
|<span data-ttu-id="364d6-117">id</span><span class="sxs-lookup"><span data-stu-id="364d6-117">id</span></span>|<span data-ttu-id="364d6-118">字符串</span><span class="sxs-lookup"><span data-stu-id="364d6-118">String</span></span>|<span data-ttu-id="364d6-119">用户预配到或设置自的系统标识符。</span><span class="sxs-lookup"><span data-stu-id="364d6-119">Identifier of the system that a user was provisioned to or from.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="364d6-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="364d6-120">JSON representation</span></span>

<span data-ttu-id="364d6-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="364d6-121">The following is a JSON representation of the resource.</span></span>

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


