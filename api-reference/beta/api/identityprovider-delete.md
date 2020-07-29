---
title: 删除 identityProvider
description: 删除 Identityprovider.read.all。
localization_priority: Normal
doc_type: apiPageType
author: namkedia
ms.prod: microsoft-identity-platform
ms.openlocfilehash: c7e1d81f7a8e117bc31f9e827f83cc90bbb8db59
ms.sourcegitcommit: 9faca60f0cc4ee9d6dce33fd25c72e14b5487d34
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/29/2020
ms.locfileid: "46509761"
---
# <a name="delete-identityprovider"></a><span data-ttu-id="3106a-103">删除 identityProvider</span><span class="sxs-lookup"><span data-stu-id="3106a-103">Delete identityProvider</span></span>

<span data-ttu-id="3106a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3106a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3106a-105">删除[identityprovider.read.all](../resources/identityprovider.md)。</span><span class="sxs-lookup"><span data-stu-id="3106a-105">Delete an [identityProvider](../resources/identityprovider.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="3106a-106">权限</span><span class="sxs-lookup"><span data-stu-id="3106a-106">Permissions</span></span>

<span data-ttu-id="3106a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3106a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3106a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3106a-109">Permission type</span></span>      | <span data-ttu-id="3106a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3106a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3106a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3106a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3106a-112">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3106a-112">IdentityProvider.ReadWrite.All</span></span>|
|<span data-ttu-id="3106a-113">委派（Microsoft 个人帐户）</span><span class="sxs-lookup"><span data-stu-id="3106a-113">Delegated (personal Microsoft account)</span></span>| <span data-ttu-id="3106a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3106a-114">Not supported.</span></span>|
|<span data-ttu-id="3106a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3106a-115">Application</span></span>|<span data-ttu-id="3106a-116">IdentityProvider.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3106a-116">IdentityProvider.ReadWrite.All</span></span>|

<span data-ttu-id="3106a-117">工作或学校帐户需要属于下列角色之一：</span><span class="sxs-lookup"><span data-stu-id="3106a-117">The work or school account needs to belong to one of the following roles:</span></span>
* <span data-ttu-id="3106a-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="3106a-118">Global administrator</span></span>
* <span data-ttu-id="3106a-119">外部标识提供程序管理员</span><span class="sxs-lookup"><span data-stu-id="3106a-119">External Identity Provider administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="3106a-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3106a-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
DELETE /identityProviders/{id}
```

## <a name="request-headers"></a><span data-ttu-id="3106a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3106a-121">Request headers</span></span>

|<span data-ttu-id="3106a-122">名称</span><span class="sxs-lookup"><span data-stu-id="3106a-122">Name</span></span>|<span data-ttu-id="3106a-123">说明</span><span class="sxs-lookup"><span data-stu-id="3106a-123">Description</span></span>|
|:---------------|:----------|
|<span data-ttu-id="3106a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3106a-124">Authorization</span></span>|<span data-ttu-id="3106a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3106a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3106a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3106a-127">Request body</span></span>

<span data-ttu-id="3106a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3106a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3106a-129">响应</span><span class="sxs-lookup"><span data-stu-id="3106a-129">Response</span></span>

<span data-ttu-id="3106a-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="3106a-130">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="3106a-131">示例</span><span class="sxs-lookup"><span data-stu-id="3106a-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3106a-132">请求</span><span class="sxs-lookup"><span data-stu-id="3106a-132">Request</span></span>

<span data-ttu-id="3106a-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="3106a-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityprovider"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identityProviders/{id}
```


### <a name="response"></a><span data-ttu-id="3106a-134">响应</span><span class="sxs-lookup"><span data-stu-id="3106a-134">Response</span></span>

<span data-ttu-id="3106a-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="3106a-135">The following is an example of the response.</span></span>

<span data-ttu-id="3106a-136">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3106a-136">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->

``` http
HTTP/1.1 204 No Content
```
