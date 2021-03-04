---
title: 获取 userAttributeAssignments
description: 读取 identityUserFlowAttributeAssignment 对象的属性和关系。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ec932b01dfae55dd9958063fccc57e99be9b3958
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50435165"
---
# <a name="get-identityuserflowattributeassignment"></a><span data-ttu-id="0b091-103">获取 identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="0b091-103">Get identityUserFlowAttributeAssignment</span></span>

<span data-ttu-id="0b091-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0b091-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0b091-105">读取 [identityUserFlowAttributeAssignment 对象的属性和](../resources/identityuserflowattributeassignment.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="0b091-105">Read the properties and relationships of an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0b091-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="0b091-106">Permissions</span></span>

<span data-ttu-id="0b091-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0b091-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0b091-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0b091-109">Permission type</span></span>|<span data-ttu-id="0b091-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0b091-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0b091-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0b091-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0b091-112">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b091-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="0b091-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0b091-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0b091-114">不支持</span><span class="sxs-lookup"><span data-stu-id="0b091-114">Not supported</span></span>|
|<span data-ttu-id="0b091-115">Application</span><span class="sxs-lookup"><span data-stu-id="0b091-115">Application</span></span>|<span data-ttu-id="0b091-116">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0b091-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0b091-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0b091-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
GET /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0b091-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0b091-118">Optional query parameters</span></span>

<span data-ttu-id="0b091-119">此方法支持 `$select` 使用和 `$expand` 查询参数获取用户流属性的详细信息。</span><span class="sxs-lookup"><span data-stu-id="0b091-119">This method supports the `$select` and `$expand` query parameters to get the details of the user flow attribute.</span></span> <span data-ttu-id="0b091-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="0b091-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="0b091-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0b091-121">Request headers</span></span>

|<span data-ttu-id="0b091-122">名称</span><span class="sxs-lookup"><span data-stu-id="0b091-122">Name</span></span>|<span data-ttu-id="0b091-123">说明</span><span class="sxs-lookup"><span data-stu-id="0b091-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0b091-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0b091-124">Authorization</span></span>|<span data-ttu-id="0b091-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0b091-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0b091-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0b091-127">Request body</span></span>

<span data-ttu-id="0b091-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0b091-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0b091-129">响应</span><span class="sxs-lookup"><span data-stu-id="0b091-129">Response</span></span>

<span data-ttu-id="0b091-130">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0b091-130">If successful, this method returns a `200 OK` response code and an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0b091-131">示例</span><span class="sxs-lookup"><span data-stu-id="0b091-131">Examples</span></span>

### <a name="example-1-get-the-details-of-an-identityuserflowattributeassignment"></a><span data-ttu-id="0b091-132">示例 1：获取 identityUserFlowAttributeAssignment 的详细信息</span><span class="sxs-lookup"><span data-stu-id="0b091-132">Example 1: Get the details of an identityUserFlowAttributeAssignment</span></span>

#### <a name="request"></a><span data-ttu-id="0b091-133">请求</span><span class="sxs-lookup"><span data-stu-id="0b091-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0b091-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b091-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
```
# <a name="c"></a>[<span data-ttu-id="0b091-135">C#</span><span class="sxs-lookup"><span data-stu-id="0b091-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflowattributeassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b091-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b091-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflowattributeassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b091-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b091-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflowattributeassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b091-138">Java</span><span class="sxs-lookup"><span data-stu-id="0b091-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityuserflowattributeassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b091-139">响应</span><span class="sxs-lookup"><span data-stu-id="0b091-139">Response</span></span>

<span data-ttu-id="0b091-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b091-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('userFlowId')/userAttributeAssignments/$entity",
    "id": "City",
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "City",
    "userAttributeValues": [
        {
            "name": "S",
            "value": "1",
            "isDefault": true
        }
    ]
}
```

### <a name="example-2-get-the-details-of-an-identityuserflowattributeassignment-and-expand-userattribute"></a><span data-ttu-id="0b091-141">示例 2：获取 identityUserFlowAttributeAssignment 的详细信息并展开 userAttribute</span><span class="sxs-lookup"><span data-stu-id="0b091-141">Example 2: Get the details of an identityUserFlowAttributeAssignment and expand userAttribute</span></span>

#### <a name="request"></a><span data-ttu-id="0b091-142">请求</span><span class="sxs-lookup"><span data-stu-id="0b091-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="0b091-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="0b091-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}?$expand=userAttribute
```
# <a name="c"></a>[<span data-ttu-id="0b091-144">C#</span><span class="sxs-lookup"><span data-stu-id="0b091-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflowattributeassignment-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0b091-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0b091-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflowattributeassignment-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0b091-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0b091-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflowattributeassignment-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0b091-147">Java</span><span class="sxs-lookup"><span data-stu-id="0b091-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityuserflowattributeassignment-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="0b091-148">响应</span><span class="sxs-lookup"><span data-stu-id="0b091-148">Response</span></span>

<span data-ttu-id="0b091-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0b091-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttributeAssignment"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#identity/b2cUserFlows('userFlowId')/userAttributeAssignments/$entity",
    "id": "City",
    "isOptional": false,
    "requiresVerification": false,
    "userInputType": "TextBox",
    "displayName": "City",
    "userAttributeValues": [
        {
            "name": "S",
            "value": "1",
            "isDefault": true
        }
    ],
    "userAttribute": {
        "id": "City",
        "displayName": "City",
        "description": "Your city",
        "userFlowAttributeType": "builtIn",
        "dataType": "string"
  }
}
```
