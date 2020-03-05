---
title: governanceRoleAssignmentRequestStatus 资源类型
description: 表示 governanceRoleAssignmentRequest 的状态。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 287f9f6ab7b1442ebdd517edbb27175fc36e6108
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42497403"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="9e418-103">governanceRoleAssignmentRequestStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="9e418-103">governanceRoleAssignmentRequestStatus resource type</span></span>

<span data-ttu-id="9e418-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="9e418-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9e418-105">表示[governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md)的状态。</span><span class="sxs-lookup"><span data-stu-id="9e418-105">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="9e418-106">属性</span><span class="sxs-lookup"><span data-stu-id="9e418-106">Properties</span></span>
<span data-ttu-id="9e418-107">属性</span><span class="sxs-lookup"><span data-stu-id="9e418-107">Property</span></span>       | <span data-ttu-id="9e418-108">类型</span><span class="sxs-lookup"><span data-stu-id="9e418-108">Type</span></span> |<span data-ttu-id="9e418-109">说明</span><span class="sxs-lookup"><span data-stu-id="9e418-109">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="9e418-110">status</span><span class="sxs-lookup"><span data-stu-id="9e418-110">status</span></span> |<span data-ttu-id="9e418-111">String</span><span class="sxs-lookup"><span data-stu-id="9e418-111">String</span></span>| <span data-ttu-id="9e418-112">角色分配请求的状态。</span><span class="sxs-lookup"><span data-stu-id="9e418-112">The status of the role assignment request.</span></span> <span data-ttu-id="9e418-113">值可以是`InProgress`或`Closed`。</span><span class="sxs-lookup"><span data-stu-id="9e418-113">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="9e418-114">状态值</span><span class="sxs-lookup"><span data-stu-id="9e418-114">subStatus</span></span> |<span data-ttu-id="9e418-115">String</span><span class="sxs-lookup"><span data-stu-id="9e418-115">String</span></span>| <span data-ttu-id="9e418-116">角色分配请求的子状态。</span><span class="sxs-lookup"><span data-stu-id="9e418-116">The sub status of the role assignment request.</span></span> <span data-ttu-id="9e418-117">值可以是`Accepted`、 `PendingEvaluation`、 `Granted` `Denied` `PendingProvisioning` `Provisioned` `ProvisioningStarted`、、、、、、、、和。 `PendingApproval` `FailedAsResourceIsLocked` `PendingAdminDecision` `AdminApproved` `AdminDenied` `TimedOut` `PendingRevocation` `Revoked` `Canceled` `Failed` `PendingApprovalProvisioning`</span><span class="sxs-lookup"><span data-stu-id="9e418-117">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="9e418-118">statusDetails</span><span class="sxs-lookup"><span data-stu-id="9e418-118">statusDetails</span></span>       |<span data-ttu-id="9e418-119">[keyValue](../resources/keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="9e418-119">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="9e418-120">角色分配请求状态的详细信息。</span><span class="sxs-lookup"><span data-stu-id="9e418-120">The details of the status of the role assignment request.</span></span> <span data-ttu-id="9e418-121">它表示不同规则的评估结果。</span><span class="sxs-lookup"><span data-stu-id="9e418-121">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="9e418-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="9e418-122">JSON representation</span></span>

<span data-ttu-id="9e418-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9e418-123">Here is a JSON representation of the resource.</span></span>

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
