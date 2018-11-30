---
title: 获取 identityProvider
description: 检索现有 identityProvider 的属性。
ms.openlocfilehash: 238e222c820e62685fa7c9e7ca50f5efb33693cf
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044486"
---
# <a name="get-identityprovider"></a><span data-ttu-id="fdefd-103">获取 identityProvider</span><span class="sxs-lookup"><span data-stu-id="fdefd-103">Get identityProvider</span></span>

> <span data-ttu-id="fdefd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fdefd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fdefd-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fdefd-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fdefd-106">检索现有[identityProvider](../resources/identityprovider.md)的属性。</span><span class="sxs-lookup"><span data-stu-id="fdefd-106">Retrieve the properties of an existing [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fdefd-107">权限</span><span class="sxs-lookup"><span data-stu-id="fdefd-107">Permissions</span></span>

<span data-ttu-id="fdefd-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fdefd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fdefd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fdefd-110">Permission type</span></span>      | <span data-ttu-id="fdefd-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fdefd-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fdefd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fdefd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fdefd-113">IdentityProvider.Read.All IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fdefd-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="fdefd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fdefd-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="fdefd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fdefd-115">Not supported.</span></span>|
|<span data-ttu-id="fdefd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fdefd-116">Application</span></span>|<span data-ttu-id="fdefd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fdefd-117">Not supported.</span></span>|

<span data-ttu-id="fdefd-118">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="fdefd-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="fdefd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fdefd-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fdefd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fdefd-120">Request headers</span></span>

|<span data-ttu-id="fdefd-121">名称</span><span class="sxs-lookup"><span data-stu-id="fdefd-121">Name</span></span>|<span data-ttu-id="fdefd-122">说明</span><span class="sxs-lookup"><span data-stu-id="fdefd-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="fdefd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fdefd-123">Authorization</span></span>|<span data-ttu-id="fdefd-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fdefd-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fdefd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fdefd-126">Request body</span></span>

<span data-ttu-id="fdefd-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fdefd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fdefd-128">响应</span><span class="sxs-lookup"><span data-stu-id="fdefd-128">Response</span></span>

<span data-ttu-id="fdefd-129">如果成功，此方法返回`200 OK`响应代码和[identityProvider](../resources/identityprovider.md)响应正文中的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fdefd-129">If successful, this method returns `200 OK` response code and a JSON representation of the [identityProvider](../resources/identityprovider.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fdefd-130">示例</span><span class="sxs-lookup"><span data-stu-id="fdefd-130">Example</span></span>

<span data-ttu-id="fdefd-131">以下示例检索特定**identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="fdefd-131">The following example retrieves a specific **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="fdefd-132">请求</span><span class="sxs-lookup"><span data-stu-id="fdefd-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityprovider"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders/Amazon-OAuth
```

##### <a name="response"></a><span data-ttu-id="fdefd-133">响应</span><span class="sxs-lookup"><span data-stu-id="fdefd-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "id": "Amazon-OAUTH",
    "type": "Amazon",
    "name": "Login with Amazon",
    "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
    "clientSecret": "*****"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get identityProvider",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->