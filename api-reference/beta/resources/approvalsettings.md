---
title: approvalSettings 复杂类型
description: 用于访问包分配策略的 requestApprovalSettings 属性。 提供其他设置，以选择必须批准每个请求的执行者。
localization_priority: Normal
author: markwahl-msft
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 23227bd4f363748bade73999a4004747d691a364
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42508231"
---
# <a name="approvalsettings-complex-type"></a><span data-ttu-id="0e986-104">approvalSettings 复杂类型</span><span class="sxs-lookup"><span data-stu-id="0e986-104">approvalSettings complex type</span></span>

<span data-ttu-id="0e986-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="0e986-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0e986-106">用于`requestApprovalSettings` [访问包分配策略](accesspackageassignmentpolicy.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="0e986-106">Used for the `requestApprovalSettings` property of an [access package assignment policy](accesspackageassignmentpolicy.md).</span></span> <span data-ttu-id="0e986-107">提供其他设置，以选择必须批准每个请求的执行者。</span><span class="sxs-lookup"><span data-stu-id="0e986-107">Provides additional settings to select who must approve each request.</span></span> 

## <a name="properties"></a><span data-ttu-id="0e986-108">属性</span><span class="sxs-lookup"><span data-stu-id="0e986-108">Properties</span></span>

| <span data-ttu-id="0e986-109">属性</span><span class="sxs-lookup"><span data-stu-id="0e986-109">Property</span></span>                     | <span data-ttu-id="0e986-110">类型</span><span class="sxs-lookup"><span data-stu-id="0e986-110">Type</span></span>                      | <span data-ttu-id="0e986-111">说明</span><span class="sxs-lookup"><span data-stu-id="0e986-111">Description</span></span> |
| :--------------------------- | :------------------------ | :---------- |
| <span data-ttu-id="0e986-112">isApprovalRequired</span><span class="sxs-lookup"><span data-stu-id="0e986-112">isApprovalRequired</span></span> | <span data-ttu-id="0e986-113">布尔</span><span class="sxs-lookup"><span data-stu-id="0e986-113">Boolean</span></span> | <span data-ttu-id="0e986-114">如果为 false，则此策略中的请求不需要审批。</span><span class="sxs-lookup"><span data-stu-id="0e986-114">If false, then approval is not required for requests in this policy.</span></span> |
| <span data-ttu-id="0e986-115">isApprovalRequiredForExtension</span><span class="sxs-lookup"><span data-stu-id="0e986-115">isApprovalRequiredForExtension</span></span> | <span data-ttu-id="0e986-116">布尔</span><span class="sxs-lookup"><span data-stu-id="0e986-116">Boolean</span></span>| <span data-ttu-id="0e986-117">如果为 false，则已有分配扩展其工作分配的用户不需要进行审批。</span><span class="sxs-lookup"><span data-stu-id="0e986-117">If false, then approval is not required for a user who already has an assignment to extend their assignment.</span></span> |
| <span data-ttu-id="0e986-118">isRequestorJustificationRequired</span><span class="sxs-lookup"><span data-stu-id="0e986-118">isRequestorJustificationRequired</span></span> | <span data-ttu-id="0e986-119">布尔</span><span class="sxs-lookup"><span data-stu-id="0e986-119">Boolean</span></span> | <span data-ttu-id="0e986-120">指示请求者是否需要提供其请求中的理由。</span><span class="sxs-lookup"><span data-stu-id="0e986-120">Indicates whether the requestor is required to supply a justification in their request.</span></span> |
| <span data-ttu-id="0e986-121">approvalMode</span><span class="sxs-lookup"><span data-stu-id="0e986-121">approvalMode</span></span>| <span data-ttu-id="0e986-122">String</span><span class="sxs-lookup"><span data-stu-id="0e986-122">String</span></span> | <span data-ttu-id="0e986-123">或`Serial`中`NoApproval` `SingleStage`的一个。</span><span class="sxs-lookup"><span data-stu-id="0e986-123">One of `NoApproval`, `SingleStage` or `Serial`.</span></span> <span data-ttu-id="0e986-124">时`NoApproval` `isApprovalRequired`使用的是 false。</span><span class="sxs-lookup"><span data-stu-id="0e986-124">The `NoApproval` is used when `isApprovalRequired` is false.</span></span> |
| <span data-ttu-id="0e986-125">approvalStages</span><span class="sxs-lookup"><span data-stu-id="0e986-125">approvalStages</span></span> | <span data-ttu-id="0e986-126">[approvalStage](approvalstage.md)集合</span><span class="sxs-lookup"><span data-stu-id="0e986-126">[approvalStage](approvalstage.md) collection</span></span>| <span data-ttu-id="0e986-127">如果需要审批，则此集合的一个或两个元素将定义每个审批阶段。</span><span class="sxs-lookup"><span data-stu-id="0e986-127">If approval is required, the one or two elements of this collection define each of the stages of approval.</span></span> <span data-ttu-id="0e986-128">如果不需要审批，则为空数组。</span><span class="sxs-lookup"><span data-stu-id="0e986-128">An empty array if no approval is required.</span></span>  |

## <a name="json-representation"></a><span data-ttu-id="0e986-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="0e986-129">JSON representation</span></span>

<span data-ttu-id="0e986-130">以下是请求审批设置属性的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e986-130">The following is a JSON representation of the request approval settings property.</span></span>

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
