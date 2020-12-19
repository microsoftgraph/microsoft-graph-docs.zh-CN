---
title: 删除 identityApiConnector
description: 删除 identityApiConnector 对象。
author: nickgmicrosoft
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: da37c47620c82ee254b2e26ef97a72ecad4b8e3e
ms.sourcegitcommit: 424735f8ab46de76b9d850e10c7d97ffd164f62a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/19/2020
ms.locfileid: "49720142"
---
# <a name="delete-identityapiconnector"></a><span data-ttu-id="4459d-103">删除 identityApiConnector</span><span class="sxs-lookup"><span data-stu-id="4459d-103">Delete identityApiConnector</span></span>

<span data-ttu-id="4459d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4459d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4459d-105">删除 [identityApiConnector](../resources/identityapiconnector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4459d-105">Deletes an [identityApiConnector](../resources/identityapiconnector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="4459d-106">权限</span><span class="sxs-lookup"><span data-stu-id="4459d-106">Permissions</span></span>

<span data-ttu-id="4459d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4459d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="4459d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="4459d-109">Permission type</span></span>                        | <span data-ttu-id="4459d-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4459d-110">Permissions (from most to least privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="4459d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4459d-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="4459d-112">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4459d-112">APIConnectors.ReadWrite.All</span></span> |
| <span data-ttu-id="4459d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4459d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="4459d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="4459d-114">Not supported.</span></span>  |
| <span data-ttu-id="4459d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="4459d-115">Application</span></span>                            | <span data-ttu-id="4459d-116">APIConnectors.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4459d-116">APIConnectors.ReadWrite.All</span></span> |

<span data-ttu-id="4459d-117">工作或学校帐户需要属于以下角色之一：</span><span class="sxs-lookup"><span data-stu-id="4459d-117">The work or school account needs to belong to one of the following roles:</span></span>

* <span data-ttu-id="4459d-118">全局管理员</span><span class="sxs-lookup"><span data-stu-id="4459d-118">Global administrator</span></span>
* <span data-ttu-id="4459d-119">外部标识用户流管理员</span><span class="sxs-lookup"><span data-stu-id="4459d-119">External Identity User Flow administrator</span></span>

## <a name="http-request"></a><span data-ttu-id="4459d-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4459d-120">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /identity/apiConnectors/{identityApiConnectorId}
```

## <a name="request-headers"></a><span data-ttu-id="4459d-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="4459d-121">Request headers</span></span>
|<span data-ttu-id="4459d-122">名称</span><span class="sxs-lookup"><span data-stu-id="4459d-122">Name</span></span>|<span data-ttu-id="4459d-123">说明</span><span class="sxs-lookup"><span data-stu-id="4459d-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="4459d-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="4459d-124">Authorization</span></span>|<span data-ttu-id="4459d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="4459d-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="4459d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4459d-127">Request body</span></span>
<span data-ttu-id="4459d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="4459d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="4459d-129">响应</span><span class="sxs-lookup"><span data-stu-id="4459d-129">Response</span></span>

<span data-ttu-id="4459d-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="4459d-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="4459d-131">示例</span><span class="sxs-lookup"><span data-stu-id="4459d-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="4459d-132">请求</span><span class="sxs-lookup"><span data-stu-id="4459d-132">Request</span></span>

<span data-ttu-id="4459d-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="4459d-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_identityapiconnector"
}
-->

``` http
DELETE https://graph.microsoft.com/beta/identity/apiConnectors/{id}
```

### <a name="response"></a><span data-ttu-id="4459d-134">响应</span><span class="sxs-lookup"><span data-stu-id="4459d-134">Response</span></span>

<span data-ttu-id="4459d-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="4459d-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
}
-->

``` http
HTTP/1.1 204 No Content
```
