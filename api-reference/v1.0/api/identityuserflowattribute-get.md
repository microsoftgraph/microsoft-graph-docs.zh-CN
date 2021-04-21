---
title: 获取 identityUserFlowAttribute
description: 检索 identityUserFlowAttribute 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 3fca21be59ce2f54bf23633075ff2823c959f921
ms.sourcegitcommit: 32c83957ee69f21a10cd5f759adb884ce4b41c52
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/21/2021
ms.locfileid: "51920911"
---
# <a name="get-identityuserflowattribute"></a><span data-ttu-id="4908c-103">获取 identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="4908c-103">Get identityUserFlowAttribute</span></span>

<span data-ttu-id="4908c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4908c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="4908c-105">检索 [identityUserFlowAttribute](../resources/identityuserflowattribute.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="4908c-105">Retrieve the properties and relationships of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4908c-106">权限</span><span class="sxs-lookup"><span data-stu-id="4908c-106">Permissions</span></span>

<span data-ttu-id="4908c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4908c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4908c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4908c-109">Permission type</span></span>      | <span data-ttu-id="4908c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="4908c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="4908c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4908c-111">Delegated (work or school account)</span></span>|<span data-ttu-id="4908c-112">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4908c-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="4908c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4908c-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="4908c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4908c-114">Not supported.</span></span>|
|<span data-ttu-id="4908c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4908c-115">Application</span></span>|<span data-ttu-id="4908c-116">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4908c-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="4908c-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="4908c-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="4908c-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="4908c-118">Global administrator</span></span>
* <span data-ttu-id="4908c-119">外部标识用户流属性管理员</span><span class="sxs-lookup"><span data-stu-id="4908c-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="4908c-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4908c-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="4908c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4908c-121">Request headers</span></span>

|<span data-ttu-id="4908c-122">名称</span><span class="sxs-lookup"><span data-stu-id="4908c-122">Name</span></span>|<span data-ttu-id="4908c-123">说明</span><span class="sxs-lookup"><span data-stu-id="4908c-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="4908c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4908c-124">Authorization</span></span>|<span data-ttu-id="4908c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4908c-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4908c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4908c-127">Request body</span></span>

<span data-ttu-id="4908c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4908c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4908c-129">响应</span><span class="sxs-lookup"><span data-stu-id="4908c-129">Response</span></span>

<span data-ttu-id="4908c-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [identityUserFlowAttribute 的](../resources/identityuserflowattribute.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4908c-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityUserFlowAttribute](../resources/identityuserflowattribute.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="4908c-131">示例</span><span class="sxs-lookup"><span data-stu-id="4908c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4908c-132">请求</span><span class="sxs-lookup"><span data-stu-id="4908c-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="4908c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="4908c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/userFlowAttributes/{id}
```
# <a name="c"></a>[<span data-ttu-id="4908c-134">C#</span><span class="sxs-lookup"><span data-stu-id="4908c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="4908c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="4908c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="4908c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="4908c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="4908c-137">Java</span><span class="sxs-lookup"><span data-stu-id="4908c-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-userflowattributes-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="4908c-138">响应</span><span class="sxs-lookup"><span data-stu-id="4908c-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "City",
    "displayName": "City",
    "description": "Your city",
    "userFlowAttributeType": "builtIn",
    "dataType": "string"
}
```
