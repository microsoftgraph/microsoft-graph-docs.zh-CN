---
title: 列出 userAttributeAssignments
description: 从 b2cIdentityUserFlow 中的 userAttributeAssignments 导航属性获取 identityUserFlowAttributeAssignment 资源。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 46a3f1d7c33440976a71b142b1ec5fc4616c26cf
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50944718"
---
# <a name="list-userattributeassignments"></a><span data-ttu-id="51ebd-103">列出 userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="51ebd-103">List userAttributeAssignments</span></span>

<span data-ttu-id="51ebd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51ebd-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="51ebd-105">从 [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md)中的 userAttributeAssignments 导航属性获取 identityUserFlowAttributeAssignment 资源。</span><span class="sxs-lookup"><span data-stu-id="51ebd-105">Get the identityUserFlowAttributeAssignment resources from the userAttributeAssignments navigation property in a [b2cIdentityUserFlow](../resources/b2cidentityuserflow.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="51ebd-106">权限</span><span class="sxs-lookup"><span data-stu-id="51ebd-106">Permissions</span></span>

<span data-ttu-id="51ebd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51ebd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51ebd-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="51ebd-109">Permission type</span></span>|<span data-ttu-id="51ebd-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="51ebd-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51ebd-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51ebd-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51ebd-112">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51ebd-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="51ebd-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51ebd-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51ebd-114">不支持</span><span class="sxs-lookup"><span data-stu-id="51ebd-114">Not supported</span></span>|
|<span data-ttu-id="51ebd-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="51ebd-115">Application</span></span>|<span data-ttu-id="51ebd-116">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51ebd-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="51ebd-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51ebd-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/userAttributeAssignments
```

## <a name="optional-query-parameters"></a><span data-ttu-id="51ebd-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="51ebd-118">Optional query parameters</span></span>

<span data-ttu-id="51ebd-119">此方法支持 `$select` 和 `$expand` 参数获取用户流属性的详细信息。</span><span class="sxs-lookup"><span data-stu-id="51ebd-119">This method supports the `$select` and `$expand` parameters to get the details of the user flow attribute.</span></span> <span data-ttu-id="51ebd-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="51ebd-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="51ebd-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="51ebd-121">Request headers</span></span>

|<span data-ttu-id="51ebd-122">名称</span><span class="sxs-lookup"><span data-stu-id="51ebd-122">Name</span></span>|<span data-ttu-id="51ebd-123">说明</span><span class="sxs-lookup"><span data-stu-id="51ebd-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="51ebd-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="51ebd-124">Authorization</span></span>|<span data-ttu-id="51ebd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="51ebd-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="51ebd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="51ebd-127">Request body</span></span>

<span data-ttu-id="51ebd-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="51ebd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51ebd-129">响应</span><span class="sxs-lookup"><span data-stu-id="51ebd-129">Response</span></span>

<span data-ttu-id="51ebd-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="51ebd-130">If successful, this method returns a `200 OK` response code and a collection of [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="51ebd-131">示例</span><span class="sxs-lookup"><span data-stu-id="51ebd-131">Examples</span></span>

### <a name="example-1-list-userattributeassignments-in-a-b2cidentityuserflow"></a><span data-ttu-id="51ebd-132">示例 1：在 b2cIdentityUserFlow 中列出 userAttributeAssignments</span><span class="sxs-lookup"><span data-stu-id="51ebd-132">Example 1: List userAttributeAssignments in a b2cIdentityUserFlow</span></span>

#### <a name="request"></a><span data-ttu-id="51ebd-133">请求</span><span class="sxs-lookup"><span data-stu-id="51ebd-133">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="51ebd-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="51ebd-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments?
```
# <a name="c"></a>[<span data-ttu-id="51ebd-135">C#</span><span class="sxs-lookup"><span data-stu-id="51ebd-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflowattributeassignment-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51ebd-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51ebd-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflowattributeassignment-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51ebd-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51ebd-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflowattributeassignment-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51ebd-138">Java</span><span class="sxs-lookup"><span data-stu-id="51ebd-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityuserflowattributeassignment-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51ebd-139">响应</span><span class="sxs-lookup"><span data-stu-id="51ebd-139">Response</span></span>

<span data-ttu-id="51ebd-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="51ebd-140">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-list-userattributeassignments-in-a-b2cidentityuserflow-and-expand-userattribute"></a><span data-ttu-id="51ebd-141">示例 2：在 b2cIdentityUserFlow 中列出 userAttributeAssignments 并展开 userAttribute</span><span class="sxs-lookup"><span data-stu-id="51ebd-141">Example 2: List userAttributeAssignments in a b2cIdentityUserFlow and expand userAttribute</span></span>

#### <a name="request"></a><span data-ttu-id="51ebd-142">请求</span><span class="sxs-lookup"><span data-stu-id="51ebd-142">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="51ebd-143">HTTP</span><span class="sxs-lookup"><span data-stu-id="51ebd-143">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_expand_1"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments?$expand=userAttribute
```
# <a name="c"></a>[<span data-ttu-id="51ebd-144">C#</span><span class="sxs-lookup"><span data-stu-id="51ebd-144">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-identityuserflowattributeassignment-expand-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51ebd-145">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51ebd-145">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-identityuserflowattributeassignment-expand-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51ebd-146">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51ebd-146">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-identityuserflowattributeassignment-expand-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51ebd-147">Java</span><span class="sxs-lookup"><span data-stu-id="51ebd-147">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-identityuserflowattributeassignment-expand-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="51ebd-148">响应</span><span class="sxs-lookup"><span data-stu-id="51ebd-148">Response</span></span>

<span data-ttu-id="51ebd-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="51ebd-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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
