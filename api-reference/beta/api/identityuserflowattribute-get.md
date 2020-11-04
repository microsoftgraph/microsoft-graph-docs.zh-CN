---
title: 获取 identityUserFlowAttribute
description: 检索 identityUserFlowAttribute 对象的属性和关系。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: be05476a136a8a9512a102d11c516603f42aaaa7
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48903903"
---
# <a name="get-identityuserflowattribute"></a><span data-ttu-id="29765-103">获取 identityUserFlowAttribute</span><span class="sxs-lookup"><span data-stu-id="29765-103">Get identityUserFlowAttribute</span></span>

<span data-ttu-id="29765-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="29765-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="29765-105">检索 [identityUserFlowAttribute](../resources/identityuserflowattribute.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="29765-105">Retrieve the properties and relationships of a [identityUserFlowAttribute](../resources/identityuserflowattribute.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="29765-106">权限</span><span class="sxs-lookup"><span data-stu-id="29765-106">Permissions</span></span>

<span data-ttu-id="29765-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="29765-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="29765-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="29765-109">Permission type</span></span>      | <span data-ttu-id="29765-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="29765-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="29765-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="29765-111">Delegated (work or school account)</span></span>|<span data-ttu-id="29765-112">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="29765-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="29765-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="29765-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="29765-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="29765-114">Not supported.</span></span>|
|<span data-ttu-id="29765-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="29765-115">Application</span></span>|<span data-ttu-id="29765-116">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="29765-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="29765-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="29765-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="29765-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="29765-118">Global administrator</span></span>
* <span data-ttu-id="29765-119">外部标识用户流属性管理员</span><span class="sxs-lookup"><span data-stu-id="29765-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="29765-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="29765-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes/{id}
```

## <a name="request-headers"></a><span data-ttu-id="29765-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="29765-121">Request headers</span></span>

|<span data-ttu-id="29765-122">名称</span><span class="sxs-lookup"><span data-stu-id="29765-122">Name</span></span>|<span data-ttu-id="29765-123">说明</span><span class="sxs-lookup"><span data-stu-id="29765-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="29765-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="29765-124">Authorization</span></span>|<span data-ttu-id="29765-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="29765-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="29765-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="29765-127">Request body</span></span>

<span data-ttu-id="29765-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="29765-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="29765-129">响应</span><span class="sxs-lookup"><span data-stu-id="29765-129">Response</span></span>

<span data-ttu-id="29765-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [IDENTITYUSERFLOWATTRIBUTE](../resources/identityuserflowattribute.md) 的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="29765-130">If successful, this method returns a `200 OK` response code and a JSON representation of the [identityUserFlowAttribute](../resources/identityuserflowattribute.md) in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="29765-131">示例</span><span class="sxs-lookup"><span data-stu-id="29765-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="29765-132">请求</span><span class="sxs-lookup"><span data-stu-id="29765-132">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="29765-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="29765-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/userFlowAttributes/{id}
```
# <a name="c"></a>[<span data-ttu-id="29765-134">C#</span><span class="sxs-lookup"><span data-stu-id="29765-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="29765-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="29765-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="29765-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="29765-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="29765-137">响应</span><span class="sxs-lookup"><span data-stu-id="29765-137">Response</span></span>

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
