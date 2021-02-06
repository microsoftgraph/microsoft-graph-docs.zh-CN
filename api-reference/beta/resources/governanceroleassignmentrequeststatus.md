---
title: governanceRoleAssignmentRequestStatus 资源类型
description: 表示 governanceRoleAssignmentRequest 的状态。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 99fc5ef72c40a5eff30a5e33ed89316e56c26962
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128608"
---
# <a name="governanceroleassignmentrequeststatus-resource-type"></a><span data-ttu-id="12368-103">governanceRoleAssignmentRequestStatus 资源类型</span><span class="sxs-lookup"><span data-stu-id="12368-103">governanceRoleAssignmentRequestStatus resource type</span></span>

<span data-ttu-id="12368-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="12368-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="12368-105">表示 [governanceRoleAssignmentRequest 的状态](../resources/governanceroleassignmentrequest.md)。</span><span class="sxs-lookup"><span data-stu-id="12368-105">Represents the status of the [governanceRoleAssignmentRequest](../resources/governanceroleassignmentrequest.md).</span></span>


## <a name="properties"></a><span data-ttu-id="12368-106">属性</span><span class="sxs-lookup"><span data-stu-id="12368-106">Properties</span></span>
<span data-ttu-id="12368-107">属性</span><span class="sxs-lookup"><span data-stu-id="12368-107">Property</span></span>       | <span data-ttu-id="12368-108">类型</span><span class="sxs-lookup"><span data-stu-id="12368-108">Type</span></span> |<span data-ttu-id="12368-109">说明</span><span class="sxs-lookup"><span data-stu-id="12368-109">Description</span></span>|
|:----|:-------------|:-----|
|<span data-ttu-id="12368-110">status</span><span class="sxs-lookup"><span data-stu-id="12368-110">status</span></span> |<span data-ttu-id="12368-111">字符串</span><span class="sxs-lookup"><span data-stu-id="12368-111">String</span></span>| <span data-ttu-id="12368-112">请求角色分配状态。</span><span class="sxs-lookup"><span data-stu-id="12368-112">The status of the role assignment request.</span></span> <span data-ttu-id="12368-113">值可以是或 `InProgress` `Closed` 。</span><span class="sxs-lookup"><span data-stu-id="12368-113">The value can be `InProgress` or `Closed`.</span></span>|
|<span data-ttu-id="12368-114">subStatus</span><span class="sxs-lookup"><span data-stu-id="12368-114">subStatus</span></span> |<span data-ttu-id="12368-115">字符串</span><span class="sxs-lookup"><span data-stu-id="12368-115">String</span></span>| <span data-ttu-id="12368-116">请求的子角色分配状态。</span><span class="sxs-lookup"><span data-stu-id="12368-116">The sub status of the role assignment request.</span></span> <span data-ttu-id="12368-117">值可以是 `Accepted` ， `PendingEvaluation` ， ， ， ， `Granted` ， ， ， ， ， ， `Denied` `PendingProvisioning` `Provisioned` `PendingRevocation` `Revoked` `Canceled` 和 `Failed` `PendingApprovalProvisioning` `PendingApproval` `FailedAsResourceIsLocked` `PendingAdminDecision` `AdminApproved` `AdminDenied` `TimedOut` `ProvisioningStarted` 。</span><span class="sxs-lookup"><span data-stu-id="12368-117">The values can be `Accepted`, `PendingEvaluation`, `Granted`, `Denied`, `PendingProvisioning`, `Provisioned`, `PendingRevocation`, `Revoked`, `Canceled`, `Failed`, `PendingApprovalProvisioning`, `PendingApproval`, `FailedAsResourceIsLocked`, `PendingAdminDecision`, `AdminApproved`, `AdminDenied`, `TimedOut`, and `ProvisioningStarted`.</span></span>|
|<span data-ttu-id="12368-118">statusDetails</span><span class="sxs-lookup"><span data-stu-id="12368-118">statusDetails</span></span>       |<span data-ttu-id="12368-119">[keyValue](../resources/keyvalue.md) 集合</span><span class="sxs-lookup"><span data-stu-id="12368-119">[keyValue](../resources/keyvalue.md) collection</span></span>| <span data-ttu-id="12368-120">请求角色分配的详细信息。</span><span class="sxs-lookup"><span data-stu-id="12368-120">The details of the status of the role assignment request.</span></span> <span data-ttu-id="12368-121">它表示不同规则的评估结果。</span><span class="sxs-lookup"><span data-stu-id="12368-121">It represents the evaluation results of different rules.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="12368-122">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="12368-122">JSON representation</span></span>

<span data-ttu-id="12368-123">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="12368-123">Here is a JSON representation of the resource.</span></span>

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


