---
title: governanceRoleAssignmentRequestStatus 资源类型
description: 代表 governanceRoleAssignmentRequest 的状态。
localization_priority: Normal
ms.openlocfilehash: c5daac53661cc607d51e5bfd1ec9031cfa599fca
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27808069"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="56429-103">governanceRoleAssignmentRequestStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="56429-103">governanceRoleAssignmentRequestStatus resource type</span></span>

> <span data-ttu-id="56429-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="56429-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="56429-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="56429-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="56429-106">代表[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)的状态。</span><span class="sxs-lookup"><span data-stu-id="56429-106">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="56429-107">属性</span><span class="sxs-lookup"><span data-stu-id="56429-107">Properties</span></span>
<span data-ttu-id="56429-108">属性</span><span class="sxs-lookup"><span data-stu-id="56429-108">Property</span></span>       | <span data-ttu-id="56429-109">类型</span><span class="sxs-lookup"><span data-stu-id="56429-109">Type</span></span> |<span data-ttu-id="56429-110">说明</span><span class="sxs-lookup"><span data-stu-id="56429-110">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="56429-111">状态</span><span class="sxs-lookup"><span data-stu-id="56429-111">status</span></span> |<span data-ttu-id="56429-112">字符串</span><span class="sxs-lookup"><span data-stu-id="56429-112">String</span></span>| <span data-ttu-id="56429-113">角色分配请求的状态。</span><span class="sxs-lookup"><span data-stu-id="56429-113">The status of the role assignment request.</span></span> <span data-ttu-id="56429-114">值可以是`InProgress`或`Closed`。</span><span class="sxs-lookup"><span data-stu-id="56429-114">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="56429-115">子状态</span><span class="sxs-lookup"><span data-stu-id="56429-115">subStatus</span></span> |<span data-ttu-id="56429-116">字符串</span><span class="sxs-lookup"><span data-stu-id="56429-116">String</span></span>| <span data-ttu-id="56429-117">Sub 角色分配请求的状态。</span><span class="sxs-lookup"><span data-stu-id="56429-117">The sub status of the role assignment request.</span></span> <span data-ttu-id="56429-118">值可以是`Accepted`， `PendingEvaluation`， `Granted`， `Denied`， `PendingProvisioning`， `Provisioned`， `PendingRevocation`， `Revoked`， `Canceled`， `Failed`， `PendingApprovalProvisioning`， `PendingApproval`， `FailedAsResourceIsLocked`， `PendingAdminDecision`， `AdminApproved`， `AdminDenied`， `TimedOut`，和`ProvisioningStarted`。</span><span class="sxs-lookup"><span data-stu-id="56429-118">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="56429-119">statusDetails</span><span class="sxs-lookup"><span data-stu-id="56429-119">statusDetails</span></span>       |<span data-ttu-id="56429-120">[keyValue](../resources/keyvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="56429-120">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="56429-121">角色分配请求的状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="56429-121">The details of the status of the role assignment request.</span></span> <span data-ttu-id="56429-122">它所表示不同规则评估的结果。</span><span class="sxs-lookup"><span data-stu-id="56429-122">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="56429-123">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="56429-123">JSON representation</span></span>

<span data-ttu-id="56429-124">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="56429-124">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"
}-->


```json
{
  "status": "String",
  "subStatus": "String",
  "statusDetails": [{"@odata.type": "microsoft.graph.keyvalue"}],
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequestStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
