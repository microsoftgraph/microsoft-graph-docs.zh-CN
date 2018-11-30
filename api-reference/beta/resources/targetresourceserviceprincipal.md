---
title: targetResourceServicePrincipal 资源类型
description: 指示资源的影响审核活动 ServicePrincipalId。 派生 targetResource 资源。
ms.openlocfilehash: 6d6e19997f4bfead771fc0230207df62dde6c6cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047396"
---
# <a name="targetresourceserviceprincipal-resource-type"></a><span data-ttu-id="86be8-104">targetResourceServicePrincipal 资源类型</span><span class="sxs-lookup"><span data-stu-id="86be8-104">targetResourceServicePrincipal resource type</span></span>
<span data-ttu-id="86be8-105">指示资源的影响审核活动 ServicePrincipalId。</span><span class="sxs-lookup"><span data-stu-id="86be8-105">Indicates the ServicePrincipalId for the resource that impacted the audit activity.</span></span> <span data-ttu-id="86be8-106">派生[targetResource](targetresource.md)资源。</span><span class="sxs-lookup"><span data-stu-id="86be8-106">Derived from the [targetResource](targetresource.md) resource.</span></span>



## <a name="properties"></a><span data-ttu-id="86be8-107">属性</span><span class="sxs-lookup"><span data-stu-id="86be8-107">Properties</span></span>
| <span data-ttu-id="86be8-108">属性</span><span class="sxs-lookup"><span data-stu-id="86be8-108">Property</span></span>     | <span data-ttu-id="86be8-109">类型</span><span class="sxs-lookup"><span data-stu-id="86be8-109">Type</span></span>   |<span data-ttu-id="86be8-110">说明</span><span class="sxs-lookup"><span data-stu-id="86be8-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="86be8-111">appId</span><span class="sxs-lookup"><span data-stu-id="86be8-111">appId</span></span>|<span data-ttu-id="86be8-112">String</span><span class="sxs-lookup"><span data-stu-id="86be8-112">String</span></span>|<span data-ttu-id="86be8-113">指示应用程序的唯一 Id。</span><span class="sxs-lookup"><span data-stu-id="86be8-113">Indicates the Unique Id of the application.</span></span> <span data-ttu-id="86be8-114">指的特定应用程序的应用程序 Id。</span><span class="sxs-lookup"><span data-stu-id="86be8-114">Refers to App Id for a specfic app.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="86be8-115">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="86be8-115">JSON representation</span></span>

<span data-ttu-id="86be8-116">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="86be8-116">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResourceServicePrincipal"
}-->

```json
{
  "appId": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResourceServicePrincipal resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->