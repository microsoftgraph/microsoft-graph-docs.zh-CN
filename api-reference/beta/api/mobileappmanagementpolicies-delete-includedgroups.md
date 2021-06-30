---
title: 删除 includedGroup
description: 从移动应用管理策略中包含的组列表中删除组。
author: ravennMSFT
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: 4097b71b17467f32d7b7c687c004ab4a8a59a556
ms.sourcegitcommit: 7f674112f5b95446fac86d829509f889c60f1693
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/30/2021
ms.locfileid: "53208335"
---
# <a name="delete-includedgroup"></a><span data-ttu-id="e2b91-103">删除 includedGroup</span><span class="sxs-lookup"><span data-stu-id="e2b91-103">Delete includedGroup</span></span>

<span data-ttu-id="e2b91-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e2b91-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e2b91-105">从移动应用管理策略中包含的组列表中删除组。</span><span class="sxs-lookup"><span data-stu-id="e2b91-105">Delete a group from the list of groups included in a mobile app management policy.</span></span>

## <a name="permissions"></a><span data-ttu-id="e2b91-106">权限</span><span class="sxs-lookup"><span data-stu-id="e2b91-106">Permissions</span></span>

<span data-ttu-id="e2b91-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e2b91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e2b91-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e2b91-109">Permission type</span></span>|<span data-ttu-id="e2b91-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e2b91-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e2b91-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e2b91-111">Delegated (work or school account)</span></span>|<span data-ttu-id="e2b91-112">Policy.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e2b91-112">Policy.ReadWrite.All</span></span>|
|<span data-ttu-id="e2b91-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e2b91-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e2b91-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2b91-114">Not supported.</span></span>|
|<span data-ttu-id="e2b91-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e2b91-115">Application</span></span> | <span data-ttu-id="e2b91-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e2b91-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e2b91-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e2b91-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /policies/mobileAppManagementPolicies/{id}/includedGroups/{id}/$ref
```

## <a name="request-headers"></a><span data-ttu-id="e2b91-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="e2b91-118">Request headers</span></span>

|<span data-ttu-id="e2b91-119">名称</span><span class="sxs-lookup"><span data-stu-id="e2b91-119">Name</span></span>|<span data-ttu-id="e2b91-120">说明</span><span class="sxs-lookup"><span data-stu-id="e2b91-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e2b91-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="e2b91-121">Authorization</span></span>|<span data-ttu-id="e2b91-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e2b91-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e2b91-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="e2b91-124">Request body</span></span>

<span data-ttu-id="e2b91-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e2b91-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e2b91-126">响应</span><span class="sxs-lookup"><span data-stu-id="e2b91-126">Response</span></span>

<span data-ttu-id="e2b91-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="e2b91-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e2b91-129">示例</span><span class="sxs-lookup"><span data-stu-id="e2b91-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e2b91-130">请求</span><span class="sxs-lookup"><span data-stu-id="e2b91-130">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="e2b91-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="e2b91-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_group"
}
-->

```http
DELETE https://graph.microsoft.com/beta/policies/mobileAppManagementPolicies/ab90bacf-55a3-4a3e-839a-aa4b74e4f020/includedGroups/1a9db3ab-0acf-4808-99ae-e8ed581cb2e0/$ref
```
# <a name="c"></a>[<span data-ttu-id="e2b91-132">C#</span><span class="sxs-lookup"><span data-stu-id="e2b91-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e2b91-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e2b91-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e2b91-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e2b91-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e2b91-135">Java</span><span class="sxs-lookup"><span data-stu-id="e2b91-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="e2b91-136">响应</span><span class="sxs-lookup"><span data-stu-id="e2b91-136">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
