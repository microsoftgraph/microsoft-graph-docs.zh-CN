---
title: 获取 userAttributeAssignments
description: 读取 identityUserFlowAttributeAssignment 对象的属性和关系。
author: jkdouglas
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: fa51cbdc0d58c9a80863eeb3743ca56ec9d2e890
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882830"
---
# <a name="get-identityuserflowattributeassignment"></a><span data-ttu-id="00423-103">获取 identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="00423-103">Get identityUserFlowAttributeAssignment</span></span>

<span data-ttu-id="00423-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="00423-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="00423-105">读取 [identityUserFlowAttributeAssignment 对象的属性和](../resources/identityuserflowattributeassignment.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="00423-105">Read the properties and relationships of an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="00423-106">权限</span><span class="sxs-lookup"><span data-stu-id="00423-106">Permissions</span></span>

<span data-ttu-id="00423-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="00423-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="00423-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="00423-109">Permission type</span></span>|<span data-ttu-id="00423-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="00423-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="00423-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="00423-111">Delegated (work or school account)</span></span>|<span data-ttu-id="00423-112">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00423-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="00423-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="00423-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="00423-114">不支持</span><span class="sxs-lookup"><span data-stu-id="00423-114">Not supported</span></span>|
|<span data-ttu-id="00423-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="00423-115">Application</span></span>|<span data-ttu-id="00423-116">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="00423-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="00423-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="00423-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="00423-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="00423-118">Optional query parameters</span></span>

<span data-ttu-id="00423-119">此方法支持 `$select` 使用 `$expand` 和 查询参数获取用户流属性的详细信息。</span><span class="sxs-lookup"><span data-stu-id="00423-119">This method supports the `$select` and `$expand` query parameters to get the details of the user flow attribute.</span></span> <span data-ttu-id="00423-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="00423-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="00423-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="00423-121">Request headers</span></span>

|<span data-ttu-id="00423-122">名称</span><span class="sxs-lookup"><span data-stu-id="00423-122">Name</span></span>|<span data-ttu-id="00423-123">说明</span><span class="sxs-lookup"><span data-stu-id="00423-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="00423-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="00423-124">Authorization</span></span>|<span data-ttu-id="00423-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="00423-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="00423-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="00423-127">Request body</span></span>

<span data-ttu-id="00423-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="00423-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="00423-129">响应</span><span class="sxs-lookup"><span data-stu-id="00423-129">Response</span></span>

<span data-ttu-id="00423-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="00423-130">If successful, this method returns a `200 OK` response code and an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="00423-131">示例</span><span class="sxs-lookup"><span data-stu-id="00423-131">Examples</span></span>

### <a name="example-1-get-the-details-of-an-identityuserflowattributeassignment"></a><span data-ttu-id="00423-132">示例 1：获取 identityUserFlowAttributeAssignment 的详细信息</span><span class="sxs-lookup"><span data-stu-id="00423-132">Example 1: Get the details of an identityUserFlowAttributeAssignment</span></span>

#### <a name="request"></a><span data-ttu-id="00423-133">请求</span><span class="sxs-lookup"><span data-stu-id="00423-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_3"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/B2X_1_Partner/userAttributeAssignments/City
```

#### <a name="response"></a><span data-ttu-id="00423-134">响应</span><span class="sxs-lookup"><span data-stu-id="00423-134">Response</span></span>

<span data-ttu-id="00423-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="00423-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('userFlowId')/userAttributeAssignments/$entity",
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

### <a name="example-2-get-the-details-of-an-identityuserflowattributeassignment-and-expand-userattribute"></a><span data-ttu-id="00423-136">示例 2：获取 identityUserFlowAttributeAssignment 的详细信息并展开 userAttribute</span><span class="sxs-lookup"><span data-stu-id="00423-136">Example 2: Get the details of an identityUserFlowAttributeAssignment and expand userAttribute</span></span>

#### <a name="request"></a><span data-ttu-id="00423-137">请求</span><span class="sxs-lookup"><span data-stu-id="00423-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_expand_3"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/b2xUserFlows/{id}/userAttributeAssignments/{id}?$expand=userAttribute
```

#### <a name="response"></a><span data-ttu-id="00423-138">响应</span><span class="sxs-lookup"><span data-stu-id="00423-138">Response</span></span>

<span data-ttu-id="00423-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="00423-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#identity/b2xUserFlows('userFlowId')/userAttributeAssignments/$entity",
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
