---
title: 获取 userAttributeAssignments
description: 读取 identityUserFlowAttributeAssignment 对象的属性和关系。
author: jkdouglas
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: c134e5e101080c007a0927fd18887262b8e10539
ms.sourcegitcommit: e68fdfb1124d16265deb8df268d4185d9deacac6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/05/2020
ms.locfileid: "49581331"
---
# <a name="get-identityuserflowattributeassignment"></a><span data-ttu-id="46721-103">获取 identityUserFlowAttributeAssignment</span><span class="sxs-lookup"><span data-stu-id="46721-103">Get identityUserFlowAttributeAssignment</span></span>

<span data-ttu-id="46721-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="46721-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="46721-105">读取 [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="46721-105">Read the properties and relationships of an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="46721-106">权限</span><span class="sxs-lookup"><span data-stu-id="46721-106">Permissions</span></span>

<span data-ttu-id="46721-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="46721-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="46721-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="46721-109">Permission type</span></span>|<span data-ttu-id="46721-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="46721-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="46721-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="46721-111">Delegated (work or school account)</span></span>|<span data-ttu-id="46721-112">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="46721-112">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|
|<span data-ttu-id="46721-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="46721-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="46721-114">不支持</span><span class="sxs-lookup"><span data-stu-id="46721-114">Not supported</span></span>|
|<span data-ttu-id="46721-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="46721-115">Application</span></span>|<span data-ttu-id="46721-116">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="46721-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="46721-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="46721-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
GET /identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
GET /identity/b2xUserFlows/{id}/userAttributeAssignments/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="46721-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="46721-118">Optional query parameters</span></span>

<span data-ttu-id="46721-119">此方法支持 `$select` 和 `$expand` 查询参数，以获取用户流属性的详细信息。</span><span class="sxs-lookup"><span data-stu-id="46721-119">This method supports the `$select` and `$expand` query parameters to get the details of the user flow attribute.</span></span> <span data-ttu-id="46721-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="46721-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="46721-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="46721-121">Request headers</span></span>

|<span data-ttu-id="46721-122">名称</span><span class="sxs-lookup"><span data-stu-id="46721-122">Name</span></span>|<span data-ttu-id="46721-123">说明</span><span class="sxs-lookup"><span data-stu-id="46721-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="46721-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="46721-124">Authorization</span></span>|<span data-ttu-id="46721-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="46721-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="46721-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="46721-127">Request body</span></span>

<span data-ttu-id="46721-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="46721-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="46721-129">响应</span><span class="sxs-lookup"><span data-stu-id="46721-129">Response</span></span>

<span data-ttu-id="46721-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="46721-130">If successful, this method returns a `200 OK` response code and an [identityUserFlowAttributeAssignment](../resources/identityuserflowattributeassignment.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="46721-131">示例</span><span class="sxs-lookup"><span data-stu-id="46721-131">Examples</span></span>

### <a name="example-1-get-the-details-of-an-identityuserflowattributeassignment"></a><span data-ttu-id="46721-132">示例1：获取 identityUserFlowAttributeAssignment 的详细信息</span><span class="sxs-lookup"><span data-stu-id="46721-132">Example 1: Get the details of an identityUserFlowAttributeAssignment</span></span>

#### <a name="request"></a><span data-ttu-id="46721-133">请求</span><span class="sxs-lookup"><span data-stu-id="46721-133">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}
```

#### <a name="response"></a><span data-ttu-id="46721-134">响应</span><span class="sxs-lookup"><span data-stu-id="46721-134">Response</span></span>

<span data-ttu-id="46721-135">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="46721-135">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-the-details-of-an-identityuserflowattributeassignment-and-expand-userattribute"></a><span data-ttu-id="46721-136">示例2：获取 identityUserFlowAttributeAssignment 的详细信息并展开 userAttribute</span><span class="sxs-lookup"><span data-stu-id="46721-136">Example 2: Get the details of an identityUserFlowAttributeAssignment and expand userAttribute</span></span>

#### <a name="request"></a><span data-ttu-id="46721-137">请求</span><span class="sxs-lookup"><span data-stu-id="46721-137">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityuserflowattributeassignment_expand"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/b2cUserFlows/{id}/userAttributeAssignments/{id}?$expand=userAttribute
```

#### <a name="response"></a><span data-ttu-id="46721-138">响应</span><span class="sxs-lookup"><span data-stu-id="46721-138">Response</span></span>

<span data-ttu-id="46721-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="46721-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
