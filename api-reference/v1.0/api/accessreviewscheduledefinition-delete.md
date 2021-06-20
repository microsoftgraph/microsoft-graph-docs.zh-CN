---
title: 删除 accessReviewScheduleDefinition
description: 删除 accessReviewScheduleDefinition 对象。
author: isabelleatmsft
localization_priority: Normal
ms.prod: governance
doc_type: apiPageType
ms.openlocfilehash: 697a762ec6234d14d55dfc7f345299dc071af2f1
ms.sourcegitcommit: 5a1cc1943527aa268e3797ee514871e65eb474a6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/19/2021
ms.locfileid: "53031058"
---
# <a name="delete-accessreviewscheduledefinition"></a><span data-ttu-id="b1681-103">删除 accessReviewScheduleDefinition</span><span class="sxs-lookup"><span data-stu-id="b1681-103">Delete accessReviewScheduleDefinition</span></span>
<span data-ttu-id="b1681-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1681-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b1681-105">删除 [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b1681-105">Deletes an [accessReviewScheduleDefinition](../resources/accessreviewscheduledefinition.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="b1681-106">权限</span><span class="sxs-lookup"><span data-stu-id="b1681-106">Permissions</span></span>
<span data-ttu-id="b1681-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b1681-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b1681-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1681-109">Permission type</span></span>|<span data-ttu-id="b1681-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b1681-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b1681-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1681-111">Delegated (work or school account)</span></span>| <span data-ttu-id="b1681-112">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1681-112">AccessReview.ReadWrite.All</span></span>  |
|<span data-ttu-id="b1681-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1681-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b1681-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b1681-114">Not supported.</span></span>|
|<span data-ttu-id="b1681-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1681-115">Application</span></span>| <span data-ttu-id="b1681-116">AccessReview.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1681-116">AccessReview.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1681-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1681-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /identityGovernance/accessReviews/definitions/{accessReviewScheduleDefinitionId}
```

## <a name="request-headers"></a><span data-ttu-id="b1681-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1681-118">Request headers</span></span>
|<span data-ttu-id="b1681-119">名称</span><span class="sxs-lookup"><span data-stu-id="b1681-119">Name</span></span>|<span data-ttu-id="b1681-120">说明</span><span class="sxs-lookup"><span data-stu-id="b1681-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="b1681-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1681-121">Authorization</span></span>|<span data-ttu-id="b1681-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b1681-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1681-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1681-124">Request body</span></span>
<span data-ttu-id="b1681-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b1681-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b1681-126">响应</span><span class="sxs-lookup"><span data-stu-id="b1681-126">Response</span></span>

<span data-ttu-id="b1681-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b1681-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="b1681-128">示例</span><span class="sxs-lookup"><span data-stu-id="b1681-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b1681-129">请求</span><span class="sxs-lookup"><span data-stu-id="b1681-129">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_accessreviewscheduledefinition"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/identityGovernance/accessReviews/definitions/3856fd6f-36e2-4152-97c9-76070d19f730
```


### <a name="response"></a><span data-ttu-id="b1681-130">响应</span><span class="sxs-lookup"><span data-stu-id="b1681-130">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```
