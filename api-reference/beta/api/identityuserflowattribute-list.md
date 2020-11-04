---
title: 列出 identityUserFlowAttributes
description: 检索 identityUserFlowAttribute 对象的列表。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 39536cd2a8e9a2f5c1ad928384e31dcee1e7672a
ms.sourcegitcommit: 82da4012294b046416c9ae93d2294d80dab217f6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/04/2020
ms.locfileid: "48904050"
---
# <a name="list-identityuserflowattributes"></a><span data-ttu-id="8509f-103">列出 identityUserFlowAttributes</span><span class="sxs-lookup"><span data-stu-id="8509f-103">List identityUserFlowAttributes</span></span>

<span data-ttu-id="8509f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8509f-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8509f-105">检索 [identityUserFlowAttribute](../resources/identityuserflowattribute.md) 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="8509f-105">Retrieve a list of [identityUserFlowAttribute](../resources/identityuserflowattribute.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="8509f-106">权限</span><span class="sxs-lookup"><span data-stu-id="8509f-106">Permissions</span></span>

<span data-ttu-id="8509f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8509f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8509f-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8509f-109">Permission type</span></span>      | <span data-ttu-id="8509f-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8509f-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8509f-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8509f-111">Delegated (work or school account)</span></span>|<span data-ttu-id="8509f-112">IdentityUserFlow、IdentityUserflow 和所有</span><span class="sxs-lookup"><span data-stu-id="8509f-112">IdentityUserFlow.Read.All, IdentityUserflow.ReadWrite.All</span></span>|
|<span data-ttu-id="8509f-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8509f-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="8509f-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8509f-114">Not supported.</span></span>|
|<span data-ttu-id="8509f-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8509f-115">Application</span></span>|<span data-ttu-id="8509f-116">IdentityUserFlow、IdentityUserFlow 和所有</span><span class="sxs-lookup"><span data-stu-id="8509f-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="8509f-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="8509f-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="8509f-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="8509f-118">Global administrator</span></span>
* <span data-ttu-id="8509f-119">外部标识用户流属性管理员</span><span class="sxs-lookup"><span data-stu-id="8509f-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="8509f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8509f-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes
```

## <a name="request-headers"></a><span data-ttu-id="8509f-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8509f-121">Request headers</span></span>

|<span data-ttu-id="8509f-122">名称</span><span class="sxs-lookup"><span data-stu-id="8509f-122">Name</span></span>|<span data-ttu-id="8509f-123">说明</span><span class="sxs-lookup"><span data-stu-id="8509f-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="8509f-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="8509f-124">Authorization</span></span>|<span data-ttu-id="8509f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8509f-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="8509f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="8509f-127">Request body</span></span>

<span data-ttu-id="8509f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8509f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8509f-129">响应</span><span class="sxs-lookup"><span data-stu-id="8509f-129">Response</span></span>

<span data-ttu-id="8509f-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [identityUserFlowAttribute](../resources/identityuserflowattribute.md)  对象集合。</span><span class="sxs-lookup"><span data-stu-id="8509f-130">If successful, this method returns a `200 OK` response code and a collection of [identityUserFlowAttribute](../resources/identityuserflowattribute.md)  objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8509f-131">示例</span><span class="sxs-lookup"><span data-stu-id="8509f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="8509f-132">请求</span><span class="sxs-lookup"><span data-stu-id="8509f-132">Request</span></span>

<span data-ttu-id="8509f-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8509f-133">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8509f-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="8509f-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/beta/identity/userFlowAttributes
```
# <a name="c"></a>[<span data-ttu-id="8509f-135">C#</span><span class="sxs-lookup"><span data-stu-id="8509f-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-userflowattributes-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8509f-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8509f-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-userflowattributes-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8509f-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8509f-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-userflowattributes-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8509f-138">响应</span><span class="sxs-lookup"><span data-stu-id="8509f-138">Response</span></span>

<span data-ttu-id="8509f-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8509f-139">The following is an example of the response.</span></span>

<span data-ttu-id="8509f-140">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="8509f-140">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.identityUserFlowAttribute",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#userFlowAttributes",
    "value": [
      {
          "id": "City",
          "displayName": "City",
          "description": "Your city",
          "userFlowAttributeType": "builtIn",
          "dataType": "string"
      },
      {
          "id": "extension_d09380e2b4c6429a203fb816a04a7ad_Hobby",
          "displayName": "Hobby",
          "description": "Your hobby",
          "userFlowAttributeType": "custom",
          "dataType": "string",
      },
    ]
}
```
