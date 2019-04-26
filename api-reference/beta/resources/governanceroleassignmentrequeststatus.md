---
title: governanceRoleAssignmentRequestStatus 资源类型
description: 表示 governanceRoleAssignmentRequest 的状态。
localization_priority: Normal
ms.openlocfilehash: 768ef092dbe52b0989277905bae03eee091ca8c6
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33340290"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="f7a3a-103">governanceRoleAssignmentRequestStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="f7a3a-103">governanceRoleAssignmentRequestStatus resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7a3a-104">表示[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)的状态。</span><span class="sxs-lookup"><span data-stu-id="f7a3a-104">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="f7a3a-105">属性</span><span class="sxs-lookup"><span data-stu-id="f7a3a-105">Properties</span></span>
<span data-ttu-id="f7a3a-106">属性</span><span class="sxs-lookup"><span data-stu-id="f7a3a-106">Property</span></span>       | <span data-ttu-id="f7a3a-107">类型</span><span class="sxs-lookup"><span data-stu-id="f7a3a-107">Type</span></span> |<span data-ttu-id="f7a3a-108">说明</span><span class="sxs-lookup"><span data-stu-id="f7a3a-108">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="f7a3a-109">status</span><span class="sxs-lookup"><span data-stu-id="f7a3a-109">status</span></span> |<span data-ttu-id="f7a3a-110">String</span><span class="sxs-lookup"><span data-stu-id="f7a3a-110">String</span></span>| <span data-ttu-id="f7a3a-111">角色分配请求的状态。</span><span class="sxs-lookup"><span data-stu-id="f7a3a-111">The status of the role assignment request.</span></span> <span data-ttu-id="f7a3a-112">值可以是`InProgress`或`Closed`。</span><span class="sxs-lookup"><span data-stu-id="f7a3a-112">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="f7a3a-113">状态值</span><span class="sxs-lookup"><span data-stu-id="f7a3a-113">subStatus</span></span> |<span data-ttu-id="f7a3a-114">String</span><span class="sxs-lookup"><span data-stu-id="f7a3a-114">String</span></span>| <span data-ttu-id="f7a3a-115">角色分配请求的子状态。</span><span class="sxs-lookup"><span data-stu-id="f7a3a-115">The sub status of the role assignment request.</span></span> <span data-ttu-id="f7a3a-116">值可以是`Accepted`、 `PendingEvaluation`、 `Granted` `Denied` `PendingProvisioning` `Provisioned` `ProvisioningStarted`、、、、、、、、和。 `PendingApproval` `FailedAsResourceIsLocked` `PendingAdminDecision` `AdminApproved` `AdminDenied` `TimedOut` `PendingRevocation` `Revoked` `Canceled` `Failed` `PendingApprovalProvisioning`</span><span class="sxs-lookup"><span data-stu-id="f7a3a-116">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="f7a3a-117">statusDetails</span><span class="sxs-lookup"><span data-stu-id="f7a3a-117">statusDetails</span></span>       |<span data-ttu-id="f7a3a-118">[keyValue](../resources/keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="f7a3a-118">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="f7a3a-119">角色分配请求状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="f7a3a-119">The details of the status of the role assignment request.</span></span> <span data-ttu-id="f7a3a-120">它表示不同规则的评估结果。</span><span class="sxs-lookup"><span data-stu-id="f7a3a-120">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="f7a3a-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f7a3a-121">JSON representation</span></span>

<span data-ttu-id="f7a3a-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7a3a-122">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.governanceRoleAssignmentRequestStatus"
}-->


```json
{
  "status": "String",
  "subStatus": "String",
  "statusDetails": [{"@odata.type": "microsoft.graph.keyValue"}],
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
  "suppressions": []
}
-->
