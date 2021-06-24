---
title: activateService 资源类型
description: 表示要激活的服务。
author: dkershaw10
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a1ab2112406d0049df002327be784c46b7e879e6
ms.sourcegitcommit: d586ddb253d27f9ccb621bd128f6a6b4b1933918
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2021
ms.locfileid: "53109082"
---
# <a name="activateservice-resource-type"></a><span data-ttu-id="a94f7-103">activateService 资源类型</span><span class="sxs-lookup"><span data-stu-id="a94f7-103">activateService resource type</span></span>

<span data-ttu-id="a94f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a94f7-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a94f7-105">表示要激活的服务。</span><span class="sxs-lookup"><span data-stu-id="a94f7-105">Represents a service to be activated.</span></span>

## <a name="properties"></a><span data-ttu-id="a94f7-106">属性</span><span class="sxs-lookup"><span data-stu-id="a94f7-106">Properties</span></span>

| <span data-ttu-id="a94f7-107">属性</span><span class="sxs-lookup"><span data-stu-id="a94f7-107">Property</span></span>         | <span data-ttu-id="a94f7-108">类型</span><span class="sxs-lookup"><span data-stu-id="a94f7-108">Type</span></span>         | <span data-ttu-id="a94f7-109">说明</span><span class="sxs-lookup"><span data-stu-id="a94f7-109">Description</span></span>                           |
| ----------------- | ------------ | ------------------------------------- |
| <span data-ttu-id="a94f7-110">service</span><span class="sxs-lookup"><span data-stu-id="a94f7-110">service</span></span>| <span data-ttu-id="a94f7-111">String</span><span class="sxs-lookup"><span data-stu-id="a94f7-111">String</span></span> | <span data-ttu-id="a94f7-112">要激活的服务的名称。</span><span class="sxs-lookup"><span data-stu-id="a94f7-112">The name of the service to activate.</span></span> |
| <span data-ttu-id="a94f7-113">servicePlanId</span><span class="sxs-lookup"><span data-stu-id="a94f7-113">servicePlanId</span></span> | <span data-ttu-id="a94f7-114">GUID</span><span class="sxs-lookup"><span data-stu-id="a94f7-114">GUID</span></span> | <span data-ttu-id="a94f7-115">要激活的服务计划的计划标识符。</span><span class="sxs-lookup"><span data-stu-id="a94f7-115">The plan identifier of the service plan to activate.</span></span> |
| <span data-ttu-id="a94f7-116">skuId</span><span class="sxs-lookup"><span data-stu-id="a94f7-116">skuId</span></span> | <span data-ttu-id="a94f7-117">GUID</span><span class="sxs-lookup"><span data-stu-id="a94f7-117">GUID</span></span> | <span data-ttu-id="a94f7-118">服务计划的 SKU 标识符。</span><span class="sxs-lookup"><span data-stu-id="a94f7-118">The SKU identifier of the service plan.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="a94f7-119">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="a94f7-119">JSON representation</span></span>

<span data-ttu-id="a94f7-120">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a94f7-120">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.activateService"
}-->

```json
{
    "service": "string",
    "skuId": "guid",
    "servicePlanId": "guid"
}

```

<!-- uuid: 20fd7863-9545-40d4-ae8f-fee2d115a690
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "activateService",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
