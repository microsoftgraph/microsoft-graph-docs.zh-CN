---
title: unifiedRoleEligibilityScheduleRequest：cancel
description: 取消 unifiedRoleEligibilityScheduleRequest。
author: shauliu
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 325eb611042cf4627cb1a02f15fad8513ba70870
ms.sourcegitcommit: b8b0e88b3ba9a434dc45f5ab640cb46f66fae299
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/13/2021
ms.locfileid: "52474452"
---
# <a name="unifiedroleeligibilityschedulerequest-cancel"></a><span data-ttu-id="cebca-103">unifiedRoleEligibilityScheduleRequest：cancel</span><span class="sxs-lookup"><span data-stu-id="cebca-103">unifiedRoleEligibilityScheduleRequest: cancel</span></span>
<span data-ttu-id="cebca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cebca-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cebca-105">立即取消 [unifiedRoleEligibilityScheduleRequest，](../resources/unifiedroleeligibilityschedulerequest.md) 并要求系统在 30 天后自动删除已取消的请求。</span><span class="sxs-lookup"><span data-stu-id="cebca-105">Immediately cancel a [unifiedRoleEligibilityScheduleRequest](../resources/unifiedroleeligibilityschedulerequest.md) and have the system automatically delete the cancelled request after 30 days.</span></span>

## <a name="permissions"></a><span data-ttu-id="cebca-106">权限</span><span class="sxs-lookup"><span data-stu-id="cebca-106">Permissions</span></span>
<span data-ttu-id="cebca-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cebca-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cebca-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cebca-109">Permission type</span></span>|<span data-ttu-id="cebca-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cebca-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cebca-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cebca-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cebca-112">PrivilegedAccess.ReadWrite.AzureAD</span><span class="sxs-lookup"><span data-stu-id="cebca-112">PrivilegedAccess.ReadWrite.AzureAD</span></span>|
|<span data-ttu-id="cebca-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cebca-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cebca-114">不支持</span><span class="sxs-lookup"><span data-stu-id="cebca-114">Not supported</span></span>|
|<span data-ttu-id="cebca-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cebca-115">Application</span></span>|<span data-ttu-id="cebca-116">不支持</span><span class="sxs-lookup"><span data-stu-id="cebca-116">Not supported</span></span>|

## <a name="http-request"></a><span data-ttu-id="cebca-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cebca-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}/cancel
```

## <a name="request-headers"></a><span data-ttu-id="cebca-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cebca-118">Request headers</span></span>
|<span data-ttu-id="cebca-119">名称</span><span class="sxs-lookup"><span data-stu-id="cebca-119">Name</span></span>|<span data-ttu-id="cebca-120">说明</span><span class="sxs-lookup"><span data-stu-id="cebca-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="cebca-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cebca-121">Authorization</span></span>|<span data-ttu-id="cebca-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cebca-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cebca-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="cebca-124">Request body</span></span>
<span data-ttu-id="cebca-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cebca-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cebca-126">响应</span><span class="sxs-lookup"><span data-stu-id="cebca-126">Response</span></span>

<span data-ttu-id="cebca-127">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cebca-127">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="cebca-128">示例</span><span class="sxs-lookup"><span data-stu-id="cebca-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cebca-129">请求</span><span class="sxs-lookup"><span data-stu-id="cebca-129">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="cebca-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="cebca-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "unifiedroleeligibilityschedulerequest_cancel"
}
-->
``` http
POST https://graph.microsoft.com/beta/roleManagement/directory/roleEligibilityScheduleRequests/{unifiedRoleEligibilityScheduleRequestsId}/cancel
```
# <a name="c"></a>[<span data-ttu-id="cebca-131">C#</span><span class="sxs-lookup"><span data-stu-id="cebca-131">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/unifiedroleeligibilityschedulerequest-cancel-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="cebca-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cebca-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/unifiedroleeligibilityschedulerequest-cancel-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="cebca-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="cebca-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/unifiedroleeligibilityschedulerequest-cancel-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="cebca-134">Java</span><span class="sxs-lookup"><span data-stu-id="cebca-134">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/unifiedroleeligibilityschedulerequest-cancel-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="cebca-135">响应</span><span class="sxs-lookup"><span data-stu-id="cebca-135">Response</span></span>
<span data-ttu-id="cebca-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cebca-136">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

