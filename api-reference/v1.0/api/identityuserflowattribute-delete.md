---
title: 删除 identityUserFlowAttribute
description: 删除 identityUserFlowAttribute。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 31943128cbc51b8ead929cebbcb7397accf7d251
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51921576"
---
# <a name="delete-identityuserflowattribute"></a><span data-ttu-id="11bde-103">删除 identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="11bde-103">Delete identityUserFlowAttribute</span></span>

<span data-ttu-id="11bde-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11bde-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11bde-105">删除 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)。</span><span class="sxs-lookup"><span data-stu-id="11bde-105">Delete an [identityUserFlowAttribute](../resources/identityuserflowattribute.md).</span></span> <span data-ttu-id="11bde-106">只能删除自定义用户流属性。</span><span class="sxs-lookup"><span data-stu-id="11bde-106">Only custom user flow attributes can be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="11bde-107">权限</span><span class="sxs-lookup"><span data-stu-id="11bde-107">Permissions</span></span>

<span data-ttu-id="11bde-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="11bde-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11bde-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="11bde-110">Permission type</span></span>      | <span data-ttu-id="11bde-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="11bde-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11bde-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11bde-112">Delegated (work or school account)</span></span>|<span data-ttu-id="11bde-113">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11bde-113">IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="11bde-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11bde-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="11bde-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="11bde-115">Not supported.</span></span>|
|<span data-ttu-id="11bde-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="11bde-116">Application</span></span>|<span data-ttu-id="11bde-117">IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11bde-117">IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="11bde-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="11bde-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="11bde-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="11bde-119">Global administrator</span></span>
* <span data-ttu-id="11bde-120">外部标识用户流属性管理员</span><span class="sxs-lookup"><span data-stu-id="11bde-120">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="11bde-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11bde-121">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="11bde-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="11bde-122">Request headers</span></span>

|<span data-ttu-id="11bde-123">名称</span><span class="sxs-lookup"><span data-stu-id="11bde-123">Name</span></span>|<span data-ttu-id="11bde-124">说明</span><span class="sxs-lookup"><span data-stu-id="11bde-124">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="11bde-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="11bde-125">Authorization</span></span>|<span data-ttu-id="11bde-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="11bde-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="11bde-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="11bde-128">Request body</span></span>

<span data-ttu-id="11bde-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="11bde-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11bde-130">响应</span><span class="sxs-lookup"><span data-stu-id="11bde-130">Response</span></span>

<span data-ttu-id="11bde-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="11bde-131">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="11bde-132">示例</span><span class="sxs-lookup"><span data-stu-id="11bde-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="11bde-133">请求</span><span class="sxs-lookup"><span data-stu-id="11bde-133">Request</span></span>

<span data-ttu-id="11bde-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="11bde-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="11bde-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="11bde-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_userFlowAttributes"
}
-->

``` http
DELETE https://graph.microsoft.com/v1.0/identity/userFlowAttributes/extension_d09380e2b4c642b9a203fb816a04a7ad_Hobby
```
# <a name="c"></a>[<span data-ttu-id="11bde-136">C#</span><span class="sxs-lookup"><span data-stu-id="11bde-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="11bde-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11bde-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="11bde-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="11bde-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="11bde-139">Java</span><span class="sxs-lookup"><span data-stu-id="11bde-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="11bde-140">响应</span><span class="sxs-lookup"><span data-stu-id="11bde-140">Response</span></span>

<span data-ttu-id="11bde-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="11bde-141">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
