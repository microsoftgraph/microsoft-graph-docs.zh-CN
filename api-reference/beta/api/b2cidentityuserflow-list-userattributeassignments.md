---
title: 列出 userAttributeAssignments
description: 从 b2cIdentityUserFlow 中的 userAttributeAssignments 导航属性获取 identityUserFlowAttributeAssignment 资源。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 9e364ae76d0680a6d2b2dc59fef0336eda53d5fc
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438265"
---
# <a name="list-userattributeassignments"></a><span data-ttu-id="9f048-103">列出 userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="9f048-103">List userAttributeAssignments</span></span>

<span data-ttu-id="9f048-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9f048-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="9f048-105">从 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)中的 userAttributeAssignments 导航属性获取 identityUserFlowAttributeAssignment 资源。</span><span class="sxs-lookup"><span data-stu-id="9f048-105">Get the identityUserFlowAttributeAssignment resources from the userAttributeAssignments navigation property in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="9f048-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="9f048-106">Permissions</span></span>

<span data-ttu-id="9f048-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9f048-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9f048-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9f048-109">Permission type</span></span>|<span data-ttu-id="9f048-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9f048-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9f048-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9f048-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9f048-112">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f048-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="9f048-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9f048-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9f048-114">不支持</span><span class="sxs-lookup"><span data-stu-id="9f048-114">Not supported</span></span>|
|<span data-ttu-id="9f048-115">Application</span><span class="sxs-lookup"><span data-stu-id="9f048-115">Application</span></span>|<span data-ttu-id="9f048-116">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9f048-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9f048-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9f048-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/userAttributeAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="9f048-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="9f048-118">Optional query parameters</span></span>

<span data-ttu-id="9f048-119">此方法支持 `$select` 和 `$expand` 参数，以获取用户流属性的详细信息。</span><span class="sxs-lookup"><span data-stu-id="9f048-119">This method supports the `$select` and `$expand` parameters to get the details of the user flow attribute.</span></span> <span data-ttu-id="9f048-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="9f048-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="9f048-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="9f048-121">Request headers</span></span>

|<span data-ttu-id="9f048-122">名称</span><span class="sxs-lookup"><span data-stu-id="9f048-122">Name</span></span>|<span data-ttu-id="9f048-123">说明</span><span class="sxs-lookup"><span data-stu-id="9f048-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="9f048-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="9f048-124">Authorization</span></span>|<span data-ttu-id="9f048-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="9f048-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="9f048-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9f048-127">Request body</span></span>

<span data-ttu-id="9f048-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9f048-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9f048-129">响应</span><span class="sxs-lookup"><span data-stu-id="9f048-129">Response</span></span>

<span data-ttu-id="9f048-130">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9f048-130">If successful, this method returns a `200 OK` response code and a collection of [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="9f048-131">示例</span><span class="sxs-lookup"><span data-stu-id="9f048-131">Examples</span></span>

### <a name="example-1-list-userattributeassignments-in-a-b2cidentityuserflow"></a><span data-ttu-id="9f048-132">示例 1：在 b2cIdentityUserFlow 中列出 userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="9f048-132">Example 1: List userAttributeAssignments in a b2cIdentityUserFlow</span></span>

#### <a name="request"></a><span data-ttu-id="9f048-133">请求</span><span class="sxs-lookup"><span data-stu-id="9f048-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9f048-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f048-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments?
```
# <a name="c"></a>[<span data-ttu-id="9f048-135">C#</span><span class="sxs-lookup"><span data-stu-id="9f048-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflowattributeassignment-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f048-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f048-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflowattributeassignment-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f048-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f048-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflowattributeassignment-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9f048-138">Java</span><span class="sxs-lookup"><span data-stu-id="9f048-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityuserflowattributeassignment-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9f048-139">响应</span><span class="sxs-lookup"><span data-stu-id="9f048-139">Response</span></span>

<span data-ttu-id="9f048-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9f048-140">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.identityUserFlowAttributeAssignment)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.identityUserFlowAttributeAssignment",
    "value": [
        {
            "id": "City",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "RadioSingleSelect",
            "displayName": "City",
            "userAttributeValues": [
                {
                    "name": "S",
                    "value": "1",
                    "isDefault": true
                }
            ]
        },
        {
            "id": "extension_guid_shoeSize",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "TextBox",
            "displayName": "Shoe size",
            "userFlowId": "B2C_1_Consumer",
            "userAttributeValues": []
        }
    ]
}
```

### <a name="example-2-list-userattributeassignments-in-a-b2cidentityuserflow-and-expand-userattribute"></a><span data-ttu-id="9f048-141">示例 2：在 b2cIdentityUserFlow 中列出 userAttributeAssignments 并展开 userAttribute</span><span class="sxs-lookup"><span data-stu-id="9f048-141">Example 2: List userAttributeAssignments in a b2cIdentityUserFlow and expand userAttribute</span></span>

#### <a name="request"></a><span data-ttu-id="9f048-142">请求</span><span class="sxs-lookup"><span data-stu-id="9f048-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="9f048-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="9f048-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments?$expand=userAttribute
```
# <a name="c"></a>[<span data-ttu-id="9f048-144">C#</span><span class="sxs-lookup"><span data-stu-id="9f048-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflowattributeassignment-expand-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="9f048-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="9f048-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflowattributeassignment-expand-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="9f048-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="9f048-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflowattributeassignment-expand-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="9f048-147">Java</span><span class="sxs-lookup"><span data-stu-id="9f048-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityuserflowattributeassignment-expand-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="9f048-148">响应</span><span class="sxs-lookup"><span data-stu-id="9f048-148">Response</span></span>

<span data-ttu-id="9f048-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="9f048-149">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.identityUserFlowAttributeAssignment)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.type": "#microsoft.graph.identityUserFlowAttributeAssignment",
    "value": [
        {
            "id": "City",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "RadioSingleSelect",
            "displayName": "City",
            "userAttributeValues": [
                {
                    "name": "S",
                    "value": "1",
                    "isDefault": true
                }
            ],
            "userAttribute": {
                "@odata.type": "#Microsoft.Graph.BuiltInUserFlowAttribute",
                "id": "City",
                "displayName": "City",
                "description": "your city",
                "userFlowAttributeType": "builtIn",
                "dataType": "string"
            }
        },
        {
            "id": "extension_guid_shoeSize",
            "isOptional": false,
            "requiresVerification": false,
            "userInputType": "TextBox",
            "displayName": "Shoe size",
            "userFlowId": "B2C_1_Consumer",
            "userAttributeValues": [],
            "userAttribute": {
                "@odata.type": "#Microsoft.Graph.CustomUserFlowAttribute",
                "id": "extension_guid_shoeSize",
                "displayName": "Shoe size",
                "description": "Your shoe size",
                "userFlowAttributeType": "custom",
                "dataType": "string"
            }
        }
    ]
}
```
