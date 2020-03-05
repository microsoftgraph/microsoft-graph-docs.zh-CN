---
title: provisioningSystemDetails 资源类型
description: 表示用户预配或来自的系统。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 286ae448cbbaee428820d274d11d8584a9150393
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42521318"
---
# <a name="provisioningsystemdetails-resource-type"></a><span data-ttu-id="863d9-103">provisioningSystemDetails 资源类型</span><span class="sxs-lookup"><span data-stu-id="863d9-103">provisioningSystemDetails resource type</span></span>

<span data-ttu-id="863d9-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="863d9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="863d9-105">表示用户预配或来自的系统。</span><span class="sxs-lookup"><span data-stu-id="863d9-105">Represents the system that a user was provisioned to or from.</span></span> <span data-ttu-id="863d9-106">例如，在将用户从 Azure Active Directory （Azure AD）设置为 ServiceNow 时，源系统为 Azure AD，目标系统为 ServiceNow。</span><span class="sxs-lookup"><span data-stu-id="863d9-106">For example, when provisioning a user from Azure Active Directory (Azure AD) to ServiceNow, the source system is Azure AD, and the target system is ServiceNow.</span></span>

## <a name="properties"></a><span data-ttu-id="863d9-107">属性</span><span class="sxs-lookup"><span data-stu-id="863d9-107">Properties</span></span>

| <span data-ttu-id="863d9-108">属性</span><span class="sxs-lookup"><span data-stu-id="863d9-108">Property</span></span>     | <span data-ttu-id="863d9-109">类型</span><span class="sxs-lookup"><span data-stu-id="863d9-109">Type</span></span>        | <span data-ttu-id="863d9-110">说明</span><span class="sxs-lookup"><span data-stu-id="863d9-110">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="863d9-111">详细信息</span><span class="sxs-lookup"><span data-stu-id="863d9-111">details</span></span>|[<span data-ttu-id="863d9-112">detailsInfo</span><span class="sxs-lookup"><span data-stu-id="863d9-112">detailsInfo</span></span>](detailsinfo.md)|<span data-ttu-id="863d9-113">系统的详细信息。</span><span class="sxs-lookup"><span data-stu-id="863d9-113">Details of the system.</span></span>|
|<span data-ttu-id="863d9-114">displayName</span><span class="sxs-lookup"><span data-stu-id="863d9-114">displayName</span></span>|<span data-ttu-id="863d9-115">String</span><span class="sxs-lookup"><span data-stu-id="863d9-115">String</span></span>|<span data-ttu-id="863d9-116">用户预配或来自的系统的名称。</span><span class="sxs-lookup"><span data-stu-id="863d9-116">Name of the system that a user was provisioned to or from.</span></span>|
|<span data-ttu-id="863d9-117">id</span><span class="sxs-lookup"><span data-stu-id="863d9-117">id</span></span>|<span data-ttu-id="863d9-118">String</span><span class="sxs-lookup"><span data-stu-id="863d9-118">String</span></span>|<span data-ttu-id="863d9-119">用户预配或来自的系统的标识符。</span><span class="sxs-lookup"><span data-stu-id="863d9-119">Identifier of the system that a user was provisioned to or from.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="863d9-120">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="863d9-120">JSON representation</span></span>

<span data-ttu-id="863d9-121">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="863d9-121">The following is a JSON representation of the resource.</span></span>

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
