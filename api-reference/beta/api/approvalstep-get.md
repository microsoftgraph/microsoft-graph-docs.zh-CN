---
title: 获取审批步骤
description: 检索 approvalStep 对象的属性。
localization_priority: Normal
author: sbounouh
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: e4de431a5fca9321d2b60f4a3a978d5cb40fb973
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50760753"
---
# <a name="get-approvalstep"></a><span data-ttu-id="665df-103">获取审批步骤</span><span class="sxs-lookup"><span data-stu-id="665df-103">Get approvalStep</span></span>

<span data-ttu-id="665df-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="665df-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="665df-105">检索 [approvalStep 对象](../resources/approvalstep.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="665df-105">Retrieve the properties of an [approvalStep](../resources/approvalstep.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="665df-106">权限</span><span class="sxs-lookup"><span data-stu-id="665df-106">Permissions</span></span>

<span data-ttu-id="665df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="665df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="665df-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="665df-109">Permission type</span></span>                        | <span data-ttu-id="665df-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="665df-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="665df-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="665df-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="665df-112">EntitlementManagement.Read.All、EntitlementManagement.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="665df-112">EntitlementManagement.Read.All, EntitlementManagement.ReadWrite.All</span></span> |
| <span data-ttu-id="665df-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="665df-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="665df-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="665df-114">Not supported.</span></span> |
| <span data-ttu-id="665df-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="665df-115">Application</span></span>                            | <span data-ttu-id="665df-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="665df-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="665df-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="665df-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/{id}/steps/{id}
```

## <a name="request-headers"></a><span data-ttu-id="665df-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="665df-118">Request headers</span></span>

| <span data-ttu-id="665df-119">名称</span><span class="sxs-lookup"><span data-stu-id="665df-119">Name</span></span>      |<span data-ttu-id="665df-120">说明</span><span class="sxs-lookup"><span data-stu-id="665df-120">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="665df-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="665df-121">Authorization</span></span> | <span data-ttu-id="665df-122">持有者 \{token\}。</span><span class="sxs-lookup"><span data-stu-id="665df-122">Bearer \{token\}.</span></span> <span data-ttu-id="665df-123">必需。</span><span class="sxs-lookup"><span data-stu-id="665df-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="665df-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="665df-124">Request body</span></span>

<span data-ttu-id="665df-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="665df-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="665df-126">响应</span><span class="sxs-lookup"><span data-stu-id="665df-126">Response</span></span>

<span data-ttu-id="665df-127">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [approvalStep](../resources/approvalstep.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="665df-127">If successful, this method returns a `200 OK` response code and the [approvalStep](../resources/approvalstep.md) object in the response body.</span></span> <span data-ttu-id="665df-128">但是，如果调用方没有正确的权限，该方法将返回 响应 `403 Forbidden` 代码。</span><span class="sxs-lookup"><span data-stu-id="665df-128">However, if the caller does not have the right permissions, the method returns a `403 Forbidden` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="665df-129">示例</span><span class="sxs-lookup"><span data-stu-id="665df-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="665df-130">请求</span><span class="sxs-lookup"><span data-stu-id="665df-130">Request</span></span>

<span data-ttu-id="665df-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="665df-131">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "get_approvalstep"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/identityGovernance/entitlementManagement/accessPackageAssignmentApprovals/abd306ef-f7b2-4a10-9fd1-493454322489/steps/d4fa4045-4716-436d-aec5-57b0a713f095
```
---


### <a name="response"></a><span data-ttu-id="665df-132">响应</span><span class="sxs-lookup"><span data-stu-id="665df-132">Response</span></span>

<span data-ttu-id="665df-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="665df-133">The following is an example of the response.</span></span>

> <span data-ttu-id="665df-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="665df-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approvalStep"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "d4fa4045-4716-436d-aec5-57b0a713f095",
    "displayName": null,
    "reviewedDateTime": null,
    "reviewResult": "NotReviewed",
    "status": "InProgress",
    "assignedToMe": true,
    "justification": "",
    "reviewedBy": null
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2021-02-12 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get approvalStep",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


