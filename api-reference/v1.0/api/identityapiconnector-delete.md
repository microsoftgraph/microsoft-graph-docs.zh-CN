---
title: 删除 identityApiConnector
description: 删除 identityApiConnector 对象。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 37217db3bce0a8cf9c7b7d998a88ca4d63e5d41e
ms.sourcegitcommit: d033e7de12bccf92efcbe40c7b671e419a3e5b94
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/17/2021
ms.locfileid: "51882918"
---
# <a name="delete-identityapiconnector"></a><span data-ttu-id="5ff80-103">删除 identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="5ff80-103">Delete identityApiConnector</span></span>

<span data-ttu-id="5ff80-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5ff80-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="5ff80-105">删除 [identityApiConnector](../resources/identityapiconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5ff80-105">Delete an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5ff80-106">权限</span><span class="sxs-lookup"><span data-stu-id="5ff80-106">Permissions</span></span>

<span data-ttu-id="5ff80-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5ff80-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5ff80-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ff80-109">Permission type</span></span>                        | <span data-ttu-id="5ff80-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5ff80-110">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="5ff80-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ff80-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5ff80-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ff80-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="5ff80-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ff80-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5ff80-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ff80-114">Not supported.</span></span>  |
| <span data-ttu-id="5ff80-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ff80-115">Application</span></span>                            | <span data-ttu-id="5ff80-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ff80-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="5ff80-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="5ff80-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="5ff80-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="5ff80-118">Global administrator</span></span>
* <span data-ttu-id="5ff80-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="5ff80-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="5ff80-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ff80-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
DELETE /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="5ff80-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ff80-121">Request headers</span></span>

|<span data-ttu-id="5ff80-122">名称</span><span class="sxs-lookup"><span data-stu-id="5ff80-122">Name</span></span>|<span data-ttu-id="5ff80-123">说明</span><span class="sxs-lookup"><span data-stu-id="5ff80-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5ff80-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ff80-124">Authorization</span></span>|<span data-ttu-id="5ff80-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5ff80-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ff80-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ff80-127">Request body</span></span>

<span data-ttu-id="5ff80-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5ff80-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5ff80-129">响应</span><span class="sxs-lookup"><span data-stu-id="5ff80-129">Response</span></span>

<span data-ttu-id="5ff80-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="5ff80-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="5ff80-131">示例</span><span class="sxs-lookup"><span data-stu-id="5ff80-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5ff80-132">请求</span><span class="sxs-lookup"><span data-stu-id="5ff80-132">Request</span></span>

<span data-ttu-id="5ff80-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5ff80-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityapiconnector"
}
-->

``` http
DELETE https://graph.microsoft.com/v1.0/identity/apiConnectors/370eeb68-dfd3-4a47-8160-8824c2358321
```

### <a name="response"></a><span data-ttu-id="5ff80-134">响应</span><span class="sxs-lookup"><span data-stu-id="5ff80-134">Response</span></span>

<span data-ttu-id="5ff80-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5ff80-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
