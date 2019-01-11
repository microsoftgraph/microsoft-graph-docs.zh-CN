---
title: 列表 identityProviders
description: 检索所有 identityProviders 目录中。
localization_priority: Normal
ms.openlocfilehash: 43442a0bf354816c8c104d57d9720940d83bc0d0
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27837965"
---
# <a name="list-identityproviders"></a><span data-ttu-id="b2da9-103">列表 identityProviders</span><span class="sxs-lookup"><span data-stu-id="b2da9-103">List identityProviders</span></span>

> <span data-ttu-id="b2da9-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b2da9-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b2da9-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b2da9-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b2da9-106">检索所有[identityProviders](../resources/identityprovider.md)目录中。</span><span class="sxs-lookup"><span data-stu-id="b2da9-106">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="b2da9-107">权限</span><span class="sxs-lookup"><span data-stu-id="b2da9-107">Permissions</span></span>

<span data-ttu-id="b2da9-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b2da9-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b2da9-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b2da9-110">Permission type</span></span>      | <span data-ttu-id="b2da9-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b2da9-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b2da9-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b2da9-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b2da9-113">IdentityProvider.Read.All IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b2da9-113">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="b2da9-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b2da9-114">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="b2da9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2da9-115">Not supported.</span></span>|
|<span data-ttu-id="b2da9-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b2da9-116">Application</span></span>|<span data-ttu-id="b2da9-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b2da9-117">Not supported.</span></span>|

<span data-ttu-id="b2da9-118">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="b2da9-118">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="b2da9-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b2da9-119">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="b2da9-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b2da9-120">Request headers</span></span>

|<span data-ttu-id="b2da9-121">名称</span><span class="sxs-lookup"><span data-stu-id="b2da9-121">Name</span></span>|<span data-ttu-id="b2da9-122">说明</span><span class="sxs-lookup"><span data-stu-id="b2da9-122">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="b2da9-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b2da9-123">Authorization</span></span>|<span data-ttu-id="b2da9-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b2da9-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b2da9-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b2da9-126">Request body</span></span>

<span data-ttu-id="b2da9-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b2da9-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b2da9-128">响应</span><span class="sxs-lookup"><span data-stu-id="b2da9-128">Response</span></span>

<span data-ttu-id="b2da9-129">如果成功，此方法返回`200 OK`响应代码和[identityProviders](../resources/identityprovider.md)中响应正文中的 JSON 表示形式的集合。</span><span class="sxs-lookup"><span data-stu-id="b2da9-129">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityprovider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b2da9-130">示例</span><span class="sxs-lookup"><span data-stu-id="b2da9-130">Example</span></span>

<span data-ttu-id="b2da9-131">以下示例检索所有**identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="b2da9-131">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="b2da9-132">请求</span><span class="sxs-lookup"><span data-stu-id="b2da9-132">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "get_identityproviders"
}-->
```http
GET https://graph.microsoft.com/beta/identityProviders
```

##### <a name="response"></a><span data-ttu-id="b2da9-133">响应</span><span class="sxs-lookup"><span data-stu-id="b2da9-133">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.IdentityProvider",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
    "value": [
      {
        "id": "Amazon-OAUTH",
        "name": "Login with Amazon",
        "type": "Amazon",
        "clientId": "56433757-cadd-4135-8431-2c9e3fd68ae8",
        "clientSecret": "*****"
      }
    ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List identityProviders",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
