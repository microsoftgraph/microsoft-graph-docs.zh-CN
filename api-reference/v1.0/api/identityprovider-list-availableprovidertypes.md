---
title: 列出 availableProviderTypes
description: 检索目录中所有可用的标识提供程序类型。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: identity-and-sign-in
ms.openlocfilehash: 6c7c2189db2d4f1ffcca093bac6dc1a9a127c85e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882971"
---
# <a name="list-availableprovidertypes"></a><span data-ttu-id="15916-103">列出 availableProviderTypes</span><span class="sxs-lookup"><span data-stu-id="15916-103">List availableProviderTypes</span></span>

<span data-ttu-id="15916-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="15916-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="15916-105">检索目录中可用的所有标识提供程序类型。</span><span class="sxs-lookup"><span data-stu-id="15916-105">Retrieves all identity provider types available in a directory.</span></span>

## <a name="permissions"></a><span data-ttu-id="15916-106">权限</span><span class="sxs-lookup"><span data-stu-id="15916-106">Permissions</span></span>

<span data-ttu-id="15916-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="15916-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="15916-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="15916-109">Permission type</span></span>      | <span data-ttu-id="15916-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="15916-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="15916-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="15916-111">Delegated (work or school account)</span></span>|<span data-ttu-id="15916-112">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15916-112">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="15916-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="15916-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="15916-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="15916-114">Not supported.</span></span>|
|<span data-ttu-id="15916-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="15916-115">Application</span></span>|<span data-ttu-id="15916-116">IdentityProvider.Read.All、IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="15916-116">IdentityProvider.Read.All, IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="15916-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="15916-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="15916-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="15916-118">Global Administrator</span></span>
* <span data-ttu-id="15916-119">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="15916-119">External Identity Provider Administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="15916-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="15916-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /identityProviders/availableProviderTypes
```

## <a name="request-headers"></a><span data-ttu-id="15916-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="15916-121">Request headers</span></span>

|<span data-ttu-id="15916-122">名称</span><span class="sxs-lookup"><span data-stu-id="15916-122">Name</span></span>|<span data-ttu-id="15916-123">说明</span><span class="sxs-lookup"><span data-stu-id="15916-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="15916-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="15916-124">Authorization</span></span>|<span data-ttu-id="15916-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="15916-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="15916-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="15916-127">Request body</span></span>

<span data-ttu-id="15916-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="15916-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="15916-129">响应</span><span class="sxs-lookup"><span data-stu-id="15916-129">Response</span></span>

<span data-ttu-id="15916-130">如果成功，此函数会在响应正文中返回 `200 OK` 响应代码和一个 String 集合。</span><span class="sxs-lookup"><span data-stu-id="15916-130">If successful, this function returns a `200 OK` response code and a String collection in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="15916-131">示例</span><span class="sxs-lookup"><span data-stu-id="15916-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="15916-132">请求</span><span class="sxs-lookup"><span data-stu-id="15916-132">Request</span></span>

<span data-ttu-id="15916-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="15916-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "identityprovider_availableprovidertypes"
}
-->

``` http
GET https://graph.microsoft.com/v1.0/identityProviders/availableProviderTypes
```

### <a name="response"></a><span data-ttu-id="15916-134">响应</span><span class="sxs-lookup"><span data-stu-id="15916-134">Response</span></span>

<span data-ttu-id="15916-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="15916-135">The following is an example of the response.</span></span>

<span data-ttu-id="15916-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="15916-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(Edm.String)"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
      "Google",
      "Facebook",
      "MicrosoftAccount",
      "EmailOTP"
  ]
}
```
