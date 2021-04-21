---
title: 列出语言
description: 检索 B2X 用户流中支持自定义的语言列表。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 21f2611fe61d1a4165ba1fe0896f711869809aea
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51919895"
---
# <a name="list-languages"></a><span data-ttu-id="403e3-103">列出语言</span><span class="sxs-lookup"><span data-stu-id="403e3-103">List languages</span></span>

<span data-ttu-id="403e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="403e3-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="403e3-105">检索 B2X 用户流中支持自定义的语言列表。</span><span class="sxs-lookup"><span data-stu-id="403e3-105">Retrieve a list of languages supported for customization in a B2X user flow.</span></span>

## <a name="permissions"></a><span data-ttu-id="403e3-106">权限</span><span class="sxs-lookup"><span data-stu-id="403e3-106">Permissions</span></span>

<span data-ttu-id="403e3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="403e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="403e3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="403e3-109">Permission type</span></span>      | <span data-ttu-id="403e3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="403e3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="403e3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="403e3-111">Delegated (work or school account)</span></span>|<span data-ttu-id="403e3-112">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="403e3-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="403e3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="403e3-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="403e3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="403e3-114">Not supported.</span></span>|
|<span data-ttu-id="403e3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="403e3-115">Application</span></span>|<span data-ttu-id="403e3-116">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="403e3-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="403e3-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="403e3-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="403e3-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="403e3-118">Global administrator</span></span>
* <span data-ttu-id="403e3-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="403e3-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="403e3-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="403e3-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/languages
```

## <a name="request-headers"></a><span data-ttu-id="403e3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="403e3-121">Request headers</span></span>

|<span data-ttu-id="403e3-122">名称</span><span class="sxs-lookup"><span data-stu-id="403e3-122">Name</span></span>|<span data-ttu-id="403e3-123">说明</span><span class="sxs-lookup"><span data-stu-id="403e3-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="403e3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="403e3-124">Authorization</span></span>|<span data-ttu-id="403e3-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="403e3-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="403e3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="403e3-127">Request body</span></span>

<span data-ttu-id="403e3-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="403e3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="403e3-129">响应</span><span class="sxs-lookup"><span data-stu-id="403e3-129">Response</span></span>

<span data-ttu-id="403e3-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="403e3-130">If successful, this method returns a `200 OK` response code and a collection of [userFlowLanguageConfiguration](../resources/userflowlanguageconfiguration.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="403e3-131">示例</span><span class="sxs-lookup"><span data-stu-id="403e3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="403e3-132">请求</span><span class="sxs-lookup"><span data-stu-id="403e3-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="403e3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="403e3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userflowlanguageconfiguration_2"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_PartnerSignUp/languages
```
# <a name="c"></a>[<span data-ttu-id="403e3-134">C#</span><span class="sxs-lookup"><span data-stu-id="403e3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowlanguageconfiguration-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="403e3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="403e3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowlanguageconfiguration-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="403e3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="403e3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowlanguageconfiguration-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="403e3-137">Java</span><span class="sxs-lookup"><span data-stu-id="403e3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowlanguageconfiguration-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="403e3-138">响应</span><span class="sxs-lookup"><span data-stu-id="403e3-138">Response</span></span>

<span data-ttu-id="403e3-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="403e3-139">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.userFlowLanguageConfiguration)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('B2X_1_PartnerSignUp')/languages",
  "value": [
    {
      "id": "en",
      "isEnabled": true,
      "displayName": "English"
    },
    {
      "id": "de",
      "isEnabled": true,
      "displayName": "Deutsch"
    }
  ]
}
```
