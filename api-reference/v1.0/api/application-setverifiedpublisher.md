---
title: application： setVerifiedPublisher
description: 设置应用程序的已验证发布者。
localization_priority: Normal
author: jesakowi
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: ff0558f8618020eca6437d7528f1f6d0f17eafa6
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761147"
---
# <a name="application-setverifiedpublisher"></a><span data-ttu-id="b1a4c-103">application： setVerifiedPublisher</span><span class="sxs-lookup"><span data-stu-id="b1a4c-103">application: setVerifiedPublisher</span></span>

<span data-ttu-id="b1a4c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b1a4c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="b1a4c-105">在应用程序[上设置 verifiedPublisher。](../resources/verifiedPublisher.md) [](../resources/application.md)</span><span class="sxs-lookup"><span data-stu-id="b1a4c-105">Set the [verifiedPublisher](../resources/verifiedPublisher.md) on an [application](../resources/application.md).</span></span> <span data-ttu-id="b1a4c-106">有关详细信息，包括设置已验证发布者的先决条件，请参阅 [发布者验证](/azure/active-directory/develop/publisher-verification-overview)。</span><span class="sxs-lookup"><span data-stu-id="b1a4c-106">For more information, including prerequisites to setting a verified publisher, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="b1a4c-107">权限</span><span class="sxs-lookup"><span data-stu-id="b1a4c-107">Permissions</span></span>

|<span data-ttu-id="b1a4c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="b1a4c-108">Permission type</span></span>      | <span data-ttu-id="b1a4c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b1a4c-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b1a4c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b1a4c-110">Delegated (work or school account)</span></span> | <span data-ttu-id="b1a4c-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b1a4c-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="b1a4c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b1a4c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b1a4c-113">不支持</span><span class="sxs-lookup"><span data-stu-id="b1a4c-113">Not supported</span></span> |
|<span data-ttu-id="b1a4c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="b1a4c-114">Application</span></span> | <span data-ttu-id="b1a4c-115">不支持</span><span class="sxs-lookup"><span data-stu-id="b1a4c-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="b1a4c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b1a4c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/setVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="b1a4c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="b1a4c-117">Request headers</span></span>

| <span data-ttu-id="b1a4c-118">名称</span><span class="sxs-lookup"><span data-stu-id="b1a4c-118">Name</span></span>           | <span data-ttu-id="b1a4c-119">说明</span><span class="sxs-lookup"><span data-stu-id="b1a4c-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="b1a4c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="b1a4c-120">Authorization</span></span>  | <span data-ttu-id="b1a4c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b1a4c-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="b1a4c-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b1a4c-123">Content-Type</span></span>   | <span data-ttu-id="b1a4c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b1a4c-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="b1a4c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b1a4c-126">Request body</span></span>

<span data-ttu-id="b1a4c-127">在请求正文中，提供以下必需属性。</span><span class="sxs-lookup"><span data-stu-id="b1a4c-127">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="b1a4c-128">属性</span><span class="sxs-lookup"><span data-stu-id="b1a4c-128">Property</span></span>     | <span data-ttu-id="b1a4c-129">类型</span><span class="sxs-lookup"><span data-stu-id="b1a4c-129">Type</span></span>   |<span data-ttu-id="b1a4c-130">说明</span><span class="sxs-lookup"><span data-stu-id="b1a4c-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="b1a4c-131">verifiedPublisherId</span><span class="sxs-lookup"><span data-stu-id="b1a4c-131">verifiedPublisherId</span></span> | <span data-ttu-id="b1a4c-132">string</span><span class="sxs-lookup"><span data-stu-id="b1a4c-132">string</span></span> | <span data-ttu-id="b1a4c-133">Microsoft 合作伙伴网络 ID (MPNID) 从发布者的合作伙伴中心帐户在应用程序上设置的已验证发布者的 MPNID。</span><span class="sxs-lookup"><span data-stu-id="b1a4c-133">The Microsoft Partner Network ID (MPNID) of the verified publisher to be set on the application, from the publisher's Partner Center account.</span></span> |

## <a name="response"></a><span data-ttu-id="b1a4c-134">响应</span><span class="sxs-lookup"><span data-stu-id="b1a4c-134">Response</span></span>

<span data-ttu-id="b1a4c-135">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b1a4c-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b1a4c-136">示例</span><span class="sxs-lookup"><span data-stu-id="b1a4c-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="b1a4c-137">请求</span><span class="sxs-lookup"><span data-stu-id="b1a4c-137">Request</span></span>

<span data-ttu-id="b1a4c-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b1a4c-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="b1a4c-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="b1a4c-139">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_setverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/v1.0/applications/{id}/setVerifiedPublisher
Content-type: application/json

{
    "verifiedPublisherId": "1234567"
}
```
# <a name="javascript"></a>[<span data-ttu-id="b1a4c-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b1a4c-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-setverifiedpublisher-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b1a4c-141">响应</span><span class="sxs-lookup"><span data-stu-id="b1a4c-141">Response</span></span>

<span data-ttu-id="b1a4c-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b1a4c-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8c7a28dd-cebd-4dc0-b195-b2c7476e7a65
2020-09-09 21:28:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: setVerifiedPublisher",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
