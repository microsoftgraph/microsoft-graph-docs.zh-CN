---
title: 列出 defaultPages
description: 从 defaultPages 导航属性获取 userFlowLanguagePage 资源。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9c4701db54661cd4cb30fc4e75d96ed364b8d1ab
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50955217"
---
# <a name="list-defaultpages"></a><span data-ttu-id="d7949-103">列出 defaultPages</span><span class="sxs-lookup"><span data-stu-id="d7949-103">List defaultPages</span></span>

<span data-ttu-id="d7949-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d7949-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d7949-105">从 defaultPages 导航属性获取 userFlowLanguagePage 资源。</span><span class="sxs-lookup"><span data-stu-id="d7949-105">Get the userFlowLanguagePage resources from the defaultPages navigation property.</span></span> <span data-ttu-id="d7949-106">这些包含用户流的默认用户旅程中向用户显示的值。</span><span class="sxs-lookup"><span data-stu-id="d7949-106">These contain the values shown to the user in a default user journey of a user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="d7949-107">权限</span><span class="sxs-lookup"><span data-stu-id="d7949-107">Permissions</span></span>

<span data-ttu-id="d7949-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d7949-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d7949-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d7949-110">Permission type</span></span>      | <span data-ttu-id="d7949-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d7949-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d7949-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d7949-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d7949-113">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7949-113">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="d7949-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d7949-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="d7949-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d7949-115">Not supported.</span></span>|
|<span data-ttu-id="d7949-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d7949-116">Application</span></span>|<span data-ttu-id="d7949-117">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d7949-117">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="d7949-118">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="d7949-118">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="d7949-119">全局管理员</span><span class="sxs-lookup"><span data-stu-id="d7949-119">Global administrator</span></span>
* <span data-ttu-id="d7949-120">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="d7949-120">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="d7949-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d7949-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/languages/{id}/defaultPages
GET /identity/b2xUserFlows/{id}/languages/{id}/defaultPages
```

## <a name="request-headers"></a><span data-ttu-id="d7949-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="d7949-122">Request headers</span></span>

|<span data-ttu-id="d7949-123">名称</span><span class="sxs-lookup"><span data-stu-id="d7949-123">Name</span></span>|<span data-ttu-id="d7949-124">说明</span><span class="sxs-lookup"><span data-stu-id="d7949-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d7949-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="d7949-125">Authorization</span></span>|<span data-ttu-id="d7949-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d7949-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d7949-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="d7949-128">Request body</span></span>

<span data-ttu-id="d7949-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d7949-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d7949-130">响应</span><span class="sxs-lookup"><span data-stu-id="d7949-130">Response</span></span>

<span data-ttu-id="d7949-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userFlowLanguagePage](../resources/userflowlanguagepage.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d7949-131">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguagePage](../resources/userflowlanguagepage.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d7949-132">示例</span><span class="sxs-lookup"><span data-stu-id="d7949-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d7949-133">请求</span><span class="sxs-lookup"><span data-stu-id="d7949-133">Request</span></span>

<span data-ttu-id="d7949-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="d7949-134">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="d7949-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="d7949-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguagepage_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/B2C_1_Customer/languages/en/defaultPages
```
# <a name="c"></a>[<span data-ttu-id="d7949-136">C#</span><span class="sxs-lookup"><span data-stu-id="d7949-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguagepage-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d7949-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d7949-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguagepage-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d7949-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d7949-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguagepage-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d7949-139">Java</span><span class="sxs-lookup"><span data-stu-id="d7949-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguagepage-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="d7949-140">响应</span><span class="sxs-lookup"><span data-stu-id="d7949-140">Response</span></span>

<span data-ttu-id="d7949-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="d7949-141">The following is an example of the response.</span></span>

<span data-ttu-id="d7949-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="d7949-142">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguagePage)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "idpselections"
    },
    {
      "id": "phonefactor"
    }
  ]
}
```
