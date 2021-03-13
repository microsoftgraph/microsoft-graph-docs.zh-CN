---
title: 删除 printConnector
description: 删除 (取消) printConnector。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 71edae5cf61e9e3ab7e9d8ec8b36ed679d0c04f6
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772154"
---
# <a name="delete-printconnector"></a><span data-ttu-id="a46bd-103">删除 printConnector</span><span class="sxs-lookup"><span data-stu-id="a46bd-103">Delete printConnector</span></span>
<span data-ttu-id="a46bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a46bd-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="a46bd-105">删除 (注销) **printConnector**。</span><span class="sxs-lookup"><span data-stu-id="a46bd-105">Delete (unregister) a **printConnector**.</span></span>

## <a name="permissions"></a><span data-ttu-id="a46bd-106">权限</span><span class="sxs-lookup"><span data-stu-id="a46bd-106">Permissions</span></span>
<span data-ttu-id="a46bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a46bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a46bd-109">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="a46bd-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="a46bd-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="a46bd-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="a46bd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a46bd-111">Permission type</span></span> | <span data-ttu-id="a46bd-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a46bd-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a46bd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a46bd-113">Delegated (work or school account)</span></span>| <span data-ttu-id="a46bd-114">PrintConnector.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a46bd-114">PrintConnector.ReadWrite.All</span></span> |
|<span data-ttu-id="a46bd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a46bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a46bd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a46bd-116">Not Supported.</span></span>|
|<span data-ttu-id="a46bd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a46bd-117">Application</span></span>|<span data-ttu-id="a46bd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a46bd-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a46bd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a46bd-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/connectors/{printConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="a46bd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a46bd-120">Request headers</span></span>
|<span data-ttu-id="a46bd-121">名称</span><span class="sxs-lookup"><span data-stu-id="a46bd-121">Name</span></span>|<span data-ttu-id="a46bd-122">说明</span><span class="sxs-lookup"><span data-stu-id="a46bd-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a46bd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a46bd-123">Authorization</span></span>|<span data-ttu-id="a46bd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a46bd-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a46bd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a46bd-126">Request body</span></span>
<span data-ttu-id="a46bd-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a46bd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a46bd-128">响应</span><span class="sxs-lookup"><span data-stu-id="a46bd-128">Response</span></span>
<span data-ttu-id="a46bd-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a46bd-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

### <a name="error-conditions-and-messages"></a><span data-ttu-id="a46bd-131">错误条件和消息</span><span class="sxs-lookup"><span data-stu-id="a46bd-131">Error conditions and messages</span></span>

|<span data-ttu-id="a46bd-132">方案</span><span class="sxs-lookup"><span data-stu-id="a46bd-132">Scenario</span></span>|<span data-ttu-id="a46bd-133">方法</span><span class="sxs-lookup"><span data-stu-id="a46bd-133">Method</span></span>|<span data-ttu-id="a46bd-134">代码</span><span class="sxs-lookup"><span data-stu-id="a46bd-134">Code</span></span>|<span data-ttu-id="a46bd-135">消息</span><span class="sxs-lookup"><span data-stu-id="a46bd-135">Message</span></span>|
|--------|------|----|-------|
|<span data-ttu-id="a46bd-136">用户尝试删除已注册一个或多个打印机的连接器</span><span class="sxs-lookup"><span data-stu-id="a46bd-136">User attempts to delete a connector that has one or more printers registered</span></span>|<span data-ttu-id="a46bd-137">DELETE</span><span class="sxs-lookup"><span data-stu-id="a46bd-137">DELETE</span></span>|<span data-ttu-id="a46bd-138">409</span><span class="sxs-lookup"><span data-stu-id="a46bd-138">409</span></span>|<span data-ttu-id="a46bd-139">删除连接器之前，请注销关联的打印机。</span><span class="sxs-lookup"><span data-stu-id="a46bd-139">Before deleting the connector, please unregister the associated printers.</span></span>|

## <a name="examples"></a><span data-ttu-id="a46bd-140">示例</span><span class="sxs-lookup"><span data-stu-id="a46bd-140">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a46bd-141">请求</span><span class="sxs-lookup"><span data-stu-id="a46bd-141">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a46bd-142">HTTP</span><span class="sxs-lookup"><span data-stu-id="a46bd-142">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_printconnector"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/connectors/{printConnectorId}
```
# <a name="c"></a>[<span data-ttu-id="a46bd-143">C#</span><span class="sxs-lookup"><span data-stu-id="a46bd-143">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-printconnector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a46bd-144">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a46bd-144">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-printconnector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a46bd-145">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a46bd-145">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-printconnector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a46bd-146">Java</span><span class="sxs-lookup"><span data-stu-id="a46bd-146">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-printconnector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="a46bd-147">响应</span><span class="sxs-lookup"><span data-stu-id="a46bd-147">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

