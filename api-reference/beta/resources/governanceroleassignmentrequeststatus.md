---
title: governanceRoleAssignmentRequestStatus 资源类型
description: 代表 governanceRoleAssignmentRequest 的状态。
localization_priority: Normal
ms.openlocfilehash: f4f0b23cf13de5beedb1964484ec4fbbb6e98720
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29510174"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="811a1-103">governanceRoleAssignmentRequestStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="811a1-103">governanceRoleAssignmentRequestStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="811a1-104">代表[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)的状态。</span><span class="sxs-lookup"><span data-stu-id="811a1-104">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="811a1-105">属性</span><span class="sxs-lookup"><span data-stu-id="811a1-105">Properties</span></span>
<span data-ttu-id="811a1-106">属性</span><span class="sxs-lookup"><span data-stu-id="811a1-106">Property</span></span>       | <span data-ttu-id="811a1-107">类型</span><span class="sxs-lookup"><span data-stu-id="811a1-107">Type</span></span> |<span data-ttu-id="811a1-108">说明</span><span class="sxs-lookup"><span data-stu-id="811a1-108">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="811a1-109">状态</span><span class="sxs-lookup"><span data-stu-id="811a1-109">status</span></span> |<span data-ttu-id="811a1-110">String</span><span class="sxs-lookup"><span data-stu-id="811a1-110">String</span></span>| <span data-ttu-id="811a1-111">角色分配请求的状态。</span><span class="sxs-lookup"><span data-stu-id="811a1-111">The status of the role assignment request.</span></span> <span data-ttu-id="811a1-112">值可以是`InProgress`或`Closed`。</span><span class="sxs-lookup"><span data-stu-id="811a1-112">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="811a1-113">子状态</span><span class="sxs-lookup"><span data-stu-id="811a1-113">subStatus</span></span> |<span data-ttu-id="811a1-114">String</span><span class="sxs-lookup"><span data-stu-id="811a1-114">String</span></span>| <span data-ttu-id="811a1-115">Sub 角色分配请求的状态。</span><span class="sxs-lookup"><span data-stu-id="811a1-115">The sub status of the role assignment request.</span></span> <span data-ttu-id="811a1-116">值可以是`Accepted`， `PendingEvaluation`， `Granted`， `Denied`， `PendingProvisioning`， `Provisioned`， `PendingRevocation`， `Revoked`， `Canceled`， `Failed`， `PendingApprovalProvisioning`， `PendingApproval`， `FailedAsResourceIsLocked`， `PendingAdminDecision`， `AdminApproved`， `AdminDenied`， `TimedOut`，和`ProvisioningStarted`。</span><span class="sxs-lookup"><span data-stu-id="811a1-116">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="811a1-117">statusDetails</span><span class="sxs-lookup"><span data-stu-id="811a1-117">statusDetails</span></span>       |<span data-ttu-id="811a1-118">[keyValue](../resources/keyvalue.md)集合</span><span class="sxs-lookup"><span data-stu-id="811a1-118">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="811a1-119">角色分配请求的状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="811a1-119">The details of the status of the role assignment request.</span></span> <span data-ttu-id="811a1-120">它所表示不同规则评估的结果。</span><span class="sxs-lookup"><span data-stu-id="811a1-120">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="811a1-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="811a1-121">JSON representation</span></span>

<span data-ttu-id="811a1-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="811a1-122">Here is a JSON representation of the resource.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "governanceRoleAssignmentRequestStatus",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governanceroleassignmentrequeststatus.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
