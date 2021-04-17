---
title: 列出 identityUserFlowAttributes
description: 检索 identityUserFlowAttribute 对象的列表。
localization_priority: Normal
doc_type: apiPageType
author: jkdouglas
ms.prod: identity-and-sign-in
ms.openlocfilehash: 4d0a596f8710d319f5c57e651e1fa59a997e88b2
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882398"
---
# <a name="list-identityuserflowattributes"></a><span data-ttu-id="0353d-103">列出 identityUserFlowAttributes</span><span class="sxs-lookup"><span data-stu-id="0353d-103">List identityUserFlowAttributes</span></span>

<span data-ttu-id="0353d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0353d-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="0353d-105">检索 [identityUserFlowAttribute 对象](../resources/identityuserflowattribute.md) 的列表。</span><span class="sxs-lookup"><span data-stu-id="0353d-105">Retrieve a list of [identityUserFlowAttribute](../resources/identityuserflowattribute.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="0353d-106">权限</span><span class="sxs-lookup"><span data-stu-id="0353d-106">Permissions</span></span>

<span data-ttu-id="0353d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0353d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0353d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0353d-109">Permission type</span></span>      | <span data-ttu-id="0353d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0353d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0353d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0353d-111">Delegated (work or school account)</span></span>|<span data-ttu-id="0353d-112">IdentityUserFlow.Read.All、IdentityUserflow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0353d-112">IdentityUserFlow.Read.All, IdentityUserflow.ReadWrite.All</span></span>|
|<span data-ttu-id="0353d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0353d-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="0353d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0353d-114">Not supported.</span></span>|
|<span data-ttu-id="0353d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0353d-115">Application</span></span>|<span data-ttu-id="0353d-116">IdentityUserFlow.Read.All、IdentityUserFlow.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0353d-116">IdentityUserFlow.Read.All, IdentityUserFlow.ReadWrite.All</span></span>|

<span data-ttu-id="0353d-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="0353d-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="0353d-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="0353d-118">Global administrator</span></span>
* <span data-ttu-id="0353d-119">外部标识用户流属性管理员</span><span class="sxs-lookup"><span data-stu-id="0353d-119">External Identity User Flow Attribute administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="0353d-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0353d-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identity/userFlowAttributes
```

## <a name="request-headers"></a><span data-ttu-id="0353d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0353d-121">Request headers</span></span>

|<span data-ttu-id="0353d-122">名称</span><span class="sxs-lookup"><span data-stu-id="0353d-122">Name</span></span>|<span data-ttu-id="0353d-123">说明</span><span class="sxs-lookup"><span data-stu-id="0353d-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="0353d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0353d-124">Authorization</span></span>|<span data-ttu-id="0353d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0353d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0353d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0353d-127">Request body</span></span>

<span data-ttu-id="0353d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0353d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0353d-129">响应</span><span class="sxs-lookup"><span data-stu-id="0353d-129">Response</span></span>

<span data-ttu-id="0353d-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [identityUserFlowAttribute](../resources/identityuserflowattribute.md)  对象集合。</span><span class="sxs-lookup"><span data-stu-id="0353d-130">If successful, this method returns a `200 OK` response code and a collection of [identityUserFlowAttribute](../resources/identityuserflowattribute.md)  objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0353d-131">示例</span><span class="sxs-lookup"><span data-stu-id="0353d-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="0353d-132">请求</span><span class="sxs-lookup"><span data-stu-id="0353d-132">Request</span></span>

<span data-ttu-id="0353d-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0353d-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "list_userFlowAttributes"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identity/userFlowAttributes
```

### <a name="response"></a><span data-ttu-id="0353d-134">响应</span><span class="sxs-lookup"><span data-stu-id="0353d-134">Response</span></span>

<span data-ttu-id="0353d-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0353d-135">The following is an example of the response.</span></span>

<span data-ttu-id="0353d-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0353d-136">**Note:** The response object shown here might be shortened for readability.</span></span>

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
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#userFlowAttributes",
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
