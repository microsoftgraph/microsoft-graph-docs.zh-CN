---
title: approvalSettings 复杂类型
description: 用于访问包分配策略的 requestApprovalSettings 属性。 提供其他设置，以选择必须批准每个请求的人。
localization_priority: Normal
author: markwahl-msft
ms.prod: governance
doc_type: resourcePageType
ms.openlocfilehash: 99892e0943b993fe43edb4bd104fd2a3a8736a51
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50135254"
---
# <a name="approvalsettings-complex-type"></a><span data-ttu-id="781a9-104">approvalSettings 复杂类型</span><span class="sxs-lookup"><span data-stu-id="781a9-104">approvalSettings complex type</span></span>

<span data-ttu-id="781a9-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="781a9-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="781a9-106">用于 `requestApprovalSettings` 访问包分配 [策略的属性](accesspackageassignmentpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="781a9-106">Used for the `requestApprovalSettings` property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="781a9-107">提供其他设置，以选择必须批准每个请求的人。</span><span class="sxs-lookup"><span data-stu-id="781a9-107">Provides additional settings to select who must approve each request.</span></span> 

## <a name="properties"></a><span data-ttu-id="781a9-108">属性</span><span class="sxs-lookup"><span data-stu-id="781a9-108">Properties</span></span>

| <span data-ttu-id="781a9-109">属性</span><span class="sxs-lookup"><span data-stu-id="781a9-109">Property</span></span>                     | <span data-ttu-id="781a9-110">类型</span><span class="sxs-lookup"><span data-stu-id="781a9-110">Type</span></span>                      | <span data-ttu-id="781a9-111">说明</span><span class="sxs-lookup"><span data-stu-id="781a9-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="781a9-112">isApprovalRequired</span><span class="sxs-lookup"><span data-stu-id="781a9-112">isApprovalRequired</span></span> | <span data-ttu-id="781a9-113">Boolean</span><span class="sxs-lookup"><span data-stu-id="781a9-113">Boolean</span></span> | <span data-ttu-id="781a9-114">如果为 false，则不需要批准此策略中的请求。</span><span class="sxs-lookup"><span data-stu-id="781a9-114">If false, then approval is not required for requests in this policy.</span></span> |
| <span data-ttu-id="781a9-115">isApprovalRequiredForExtension</span><span class="sxs-lookup"><span data-stu-id="781a9-115">isApprovalRequiredForExtension</span></span> | <span data-ttu-id="781a9-116">Boolean</span><span class="sxs-lookup"><span data-stu-id="781a9-116">Boolean</span></span>| <span data-ttu-id="781a9-117">如果为 false，则已拥有工作分配的用户不需要批准以扩展其工作分配。</span><span class="sxs-lookup"><span data-stu-id="781a9-117">If false, then approval is not required for a user who already has an assignment to extend their assignment.</span></span> |
| <span data-ttu-id="781a9-118">isRequestorJustificationRequired</span><span class="sxs-lookup"><span data-stu-id="781a9-118">isRequestorJustificationRequired</span></span> | <span data-ttu-id="781a9-119">Boolean</span><span class="sxs-lookup"><span data-stu-id="781a9-119">Boolean</span></span> | <span data-ttu-id="781a9-120">指示请求者是否需要在请求中提供理由。</span><span class="sxs-lookup"><span data-stu-id="781a9-120">Indicates whether the requestor is required to supply a justification in their request.</span></span> |
| <span data-ttu-id="781a9-121">approvalMode</span><span class="sxs-lookup"><span data-stu-id="781a9-121">approvalMode</span></span>| <span data-ttu-id="781a9-122">字符串</span><span class="sxs-lookup"><span data-stu-id="781a9-122">String</span></span> | <span data-ttu-id="781a9-123">之 `NoApproval` 一， `SingleStage` 或 `Serial` 。</span><span class="sxs-lookup"><span data-stu-id="781a9-123">One of `NoApproval`, `SingleStage` or `Serial`.</span></span> <span data-ttu-id="781a9-124">如果 `NoApproval` 为 `isApprovalRequired` false，则使用 。</span><span class="sxs-lookup"><span data-stu-id="781a9-124">The `NoApproval` is used when `isApprovalRequired` is false.</span></span> |
| <span data-ttu-id="781a9-125">approvalStages</span><span class="sxs-lookup"><span data-stu-id="781a9-125">approvalStages</span></span> | <span data-ttu-id="781a9-126">[approvalStage](approvalstage.md) 集合</span><span class="sxs-lookup"><span data-stu-id="781a9-126">[approvalStage](approvalstage.md) collection</span></span>| <span data-ttu-id="781a9-127">如果需要审批，则此集合的一个或两个元素定义审批的每个阶段。</span><span class="sxs-lookup"><span data-stu-id="781a9-127">If approval is required, the one or two elements of this collection define each of the stages of approval.</span></span> <span data-ttu-id="781a9-128">如果不需要批准，则为空数组。</span><span class="sxs-lookup"><span data-stu-id="781a9-128">An empty array if no approval is required.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="781a9-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="781a9-129">JSON representation</span></span>

<span data-ttu-id="781a9-130">以下是请求审批设置属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="781a9-130">The following is a JSON representation of the request approval settings property.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.approvalSettings"
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


