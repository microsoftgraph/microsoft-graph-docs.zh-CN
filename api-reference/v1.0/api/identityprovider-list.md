---
title: 列出 identityProvider
description: 检索所有 identityProvider
localization_priority: Priority
author: valnav
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 06cf62ef006348b46b38f78b50dae95267921489
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577698"
---
# <a name="list-identityproviders"></a><span data-ttu-id="005c9-103">列出 identityProvider</span><span class="sxs-lookup"><span data-stu-id="005c9-103">List identityProviders</span></span>

<span data-ttu-id="005c9-104">检索目录中的所有 [identityProvider](../resources/identityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="005c9-104">Retrieve all [identityProviders](../resources/identityprovider.md) in the directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="005c9-105">权限</span><span class="sxs-lookup"><span data-stu-id="005c9-105">Permissions</span></span>

<span data-ttu-id="005c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="005c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="005c9-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="005c9-108">Permission type</span></span>      | <span data-ttu-id="005c9-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="005c9-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="005c9-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="005c9-110">Delegated (work or school account)</span></span>|<span data-ttu-id="005c9-111">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="005c9-111">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="005c9-112">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="005c9-112">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="005c9-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="005c9-113">Not supported.</span></span>|
|<span data-ttu-id="005c9-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="005c9-114">Application</span></span>|<span data-ttu-id="005c9-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="005c9-115">Not supported.</span></span>|

<span data-ttu-id="005c9-116">工作或学校帐户必须是租户的全局管理员。</span><span class="sxs-lookup"><span data-stu-id="005c9-116">The work or school account must be a global administrator of the tenant.</span></span>

## <a name="http-request"></a><span data-ttu-id="005c9-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="005c9-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /identityProviders
```

## <a name="request-headers"></a><span data-ttu-id="005c9-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="005c9-118">Request headers</span></span>

|<span data-ttu-id="005c9-119">名称</span><span class="sxs-lookup"><span data-stu-id="005c9-119">Name</span></span>|<span data-ttu-id="005c9-120">说明</span><span class="sxs-lookup"><span data-stu-id="005c9-120">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="005c9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="005c9-121">Authorization</span></span>|<span data-ttu-id="005c9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="005c9-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="005c9-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="005c9-124">Request body</span></span>

<span data-ttu-id="005c9-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="005c9-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="005c9-126">响应</span><span class="sxs-lookup"><span data-stu-id="005c9-126">Response</span></span>

<span data-ttu-id="005c9-127">如果成功，则此方法将在响应正文中返回 `200 OK` 响应代码和 JSON 表示形式的 [identityProviders](../resources/identityProvider.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="005c9-127">If successful, this method returns `200 OK` response code and a collection of [identityProviders](../resources/identityProvider.md) in JSON representation in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="005c9-128">示例</span><span class="sxs-lookup"><span data-stu-id="005c9-128">Example</span></span>

<span data-ttu-id="005c9-129">以下示例会检索所有 **identityProvider**。</span><span class="sxs-lookup"><span data-stu-id="005c9-129">The following example retrieves all **identityProvider**.</span></span>

##### <a name="request"></a><span data-ttu-id="005c9-130">请求</span><span class="sxs-lookup"><span data-stu-id="005c9-130">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "list-identityproviders"
}-->
```http
GET https://graph.microsoft.com/v1.0/identityProviders
```

##### <a name="response"></a><span data-ttu-id="005c9-131">响应</span><span class="sxs-lookup"><span data-stu-id="005c9-131">Response</span></span>

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
