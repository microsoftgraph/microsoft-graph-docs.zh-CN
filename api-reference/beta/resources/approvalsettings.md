---
title: approvalSettings 复杂类型
description: 用于访问包分配策略的 requestApprovalSettings 属性。 提供其他设置，以选择必须批准每个请求的执行者。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: e248e47cf94e2c26e80b505cbaead450e03561d4
ms.sourcegitcommit: ec6aa498067c9df6139a469e694a89447b155a1e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/28/2020
ms.locfileid: "42331387"
---
# <a name="approvalsettings-complex-type"></a><span data-ttu-id="39063-104">approvalSettings 复杂类型</span><span class="sxs-lookup"><span data-stu-id="39063-104">approvalSettings complex type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="39063-105">用于`requestApprovalSettings` [访问包分配策略](accesspackageassignmentpolicy.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="39063-105">Used for the `requestApprovalSettings` property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="39063-106">提供其他设置，以选择必须批准每个请求的执行者。</span><span class="sxs-lookup"><span data-stu-id="39063-106">Provides additional settings to select who must approve each request.</span></span> 

## <a name="properties"></a><span data-ttu-id="39063-107">属性</span><span class="sxs-lookup"><span data-stu-id="39063-107">Properties</span></span>

| <span data-ttu-id="39063-108">属性</span><span class="sxs-lookup"><span data-stu-id="39063-108">Property</span></span>                     | <span data-ttu-id="39063-109">类型</span><span class="sxs-lookup"><span data-stu-id="39063-109">Type</span></span>                      | <span data-ttu-id="39063-110">说明</span><span class="sxs-lookup"><span data-stu-id="39063-110">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="39063-111">isApprovalRequired</span><span class="sxs-lookup"><span data-stu-id="39063-111">isApprovalRequired</span></span> | <span data-ttu-id="39063-112">布尔值</span><span class="sxs-lookup"><span data-stu-id="39063-112">Boolean</span></span> | <span data-ttu-id="39063-113">如果为 false，则此策略中的请求不需要审批。</span><span class="sxs-lookup"><span data-stu-id="39063-113">If false, then approval is not required for requests in this policy.</span></span> |
| <span data-ttu-id="39063-114">isApprovalRequiredForExtension</span><span class="sxs-lookup"><span data-stu-id="39063-114">isApprovalRequiredForExtension</span></span> | <span data-ttu-id="39063-115">布尔值</span><span class="sxs-lookup"><span data-stu-id="39063-115">Boolean</span></span>| <span data-ttu-id="39063-116">如果为 false，则已有分配扩展其工作分配的用户不需要进行审批。</span><span class="sxs-lookup"><span data-stu-id="39063-116">If false, then approval is not required for a user who already has an assignment to extend their assignment.</span></span> |
| <span data-ttu-id="39063-117">isRequestorJustificationRequired</span><span class="sxs-lookup"><span data-stu-id="39063-117">isRequestorJustificationRequired</span></span> | <span data-ttu-id="39063-118">布尔值</span><span class="sxs-lookup"><span data-stu-id="39063-118">Boolean</span></span> | <span data-ttu-id="39063-119">指示请求者是否需要提供其请求中的理由。</span><span class="sxs-lookup"><span data-stu-id="39063-119">Indicates whether the requestor is required to supply a justification in their request.</span></span> |
| <span data-ttu-id="39063-120">approvalMode</span><span class="sxs-lookup"><span data-stu-id="39063-120">approvalMode</span></span>| <span data-ttu-id="39063-121">String</span><span class="sxs-lookup"><span data-stu-id="39063-121">String</span></span> | <span data-ttu-id="39063-122">或`Serial`中`NoApproval` `SingleStage`的一个。</span><span class="sxs-lookup"><span data-stu-id="39063-122">One of `NoApproval`, `SingleStage` or `Serial`.</span></span> <span data-ttu-id="39063-123">时`NoApproval` `isApprovalRequired`使用的是 false。</span><span class="sxs-lookup"><span data-stu-id="39063-123">The `NoApproval` is used when `isApprovalRequired` is false.</span></span> |
| <span data-ttu-id="39063-124">approvalStages</span><span class="sxs-lookup"><span data-stu-id="39063-124">approvalStages</span></span> | <span data-ttu-id="39063-125">[approvalStage](approvalstage.md)集合</span><span class="sxs-lookup"><span data-stu-id="39063-125">[approvalStage](approvalstage.md) collection</span></span>| <span data-ttu-id="39063-126">如果需要审批，则此集合的一个或两个元素将定义每个审批阶段。</span><span class="sxs-lookup"><span data-stu-id="39063-126">If approval is required, the one or two elements of this collection define each of the stages of approval.</span></span> <span data-ttu-id="39063-127">如果不需要审批，则为空数组。</span><span class="sxs-lookup"><span data-stu-id="39063-127">An empty array if no approval is required.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="39063-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="39063-128">JSON representation</span></span>

<span data-ttu-id="39063-129">以下是请求审批设置属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="39063-129">The following is a JSON representation of the request approval settings property.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalSettings",
  "baseType": ""
}-->

```json
{
    "isApprovalRequired": true,
    "isApprovalRequiredForExtension": false,
    "isRequestorJustificationRequired": true,
    "approvalMode": "Serial",
    "approvalStages": [{"@odata.type": "microsoft.graph.approvalStage"}]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "approvalSettings complex type",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
