---
title: 应用程序： setVerifiedPublisher
description: 设置应用程序的已验证发布者。
localization_priority: Normal
author: jesakowi
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 60681396c5f1c7e74b2ef04cd1984815e3a5e7a0
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48635543"
---
# <a name="application-setverifiedpublisher"></a><span data-ttu-id="11149-103">应用程序： setVerifiedPublisher</span><span class="sxs-lookup"><span data-stu-id="11149-103">application: setVerifiedPublisher</span></span>

<span data-ttu-id="11149-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11149-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="11149-105">在[应用程序](../resources/application.md)上设置[verifiedPublisher](../resources/verifiedPublisher.md) 。</span><span class="sxs-lookup"><span data-stu-id="11149-105">Set the [verifiedPublisher](../resources/verifiedPublisher.md) on an [application](../resources/application.md).</span></span> <span data-ttu-id="11149-106">有关详细信息，包括设置已验证的发布者的先决条件，请参阅 [publisher 验证](/azure/active-directory/develop/publisher-verification-overview)。</span><span class="sxs-lookup"><span data-stu-id="11149-106">For more information, including prerequisites to setting a verified publisher, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="11149-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="11149-107">Permissions</span></span>

|<span data-ttu-id="11149-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="11149-108">Permission type</span></span>      | <span data-ttu-id="11149-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="11149-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="11149-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11149-110">Delegated (work or school account)</span></span> | <span data-ttu-id="11149-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11149-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="11149-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11149-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="11149-113">不支持</span><span class="sxs-lookup"><span data-stu-id="11149-113">Not supported</span></span> |
|<span data-ttu-id="11149-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="11149-114">Application</span></span> | <span data-ttu-id="11149-115">不支持</span><span class="sxs-lookup"><span data-stu-id="11149-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="11149-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11149-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/setVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="11149-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="11149-117">Request headers</span></span>

| <span data-ttu-id="11149-118">名称</span><span class="sxs-lookup"><span data-stu-id="11149-118">Name</span></span>           | <span data-ttu-id="11149-119">说明</span><span class="sxs-lookup"><span data-stu-id="11149-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="11149-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="11149-120">Authorization</span></span>  | <span data-ttu-id="11149-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="11149-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="11149-123">Content-Type</span><span class="sxs-lookup"><span data-stu-id="11149-123">Content-Type</span></span>   | <span data-ttu-id="11149-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="11149-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="11149-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="11149-126">Request body</span></span>

<span data-ttu-id="11149-127">在请求正文中，提供以下必需属性。</span><span class="sxs-lookup"><span data-stu-id="11149-127">In the request body, provide the following required properties.</span></span>

| <span data-ttu-id="11149-128">属性</span><span class="sxs-lookup"><span data-stu-id="11149-128">Property</span></span>     | <span data-ttu-id="11149-129">类型</span><span class="sxs-lookup"><span data-stu-id="11149-129">Type</span></span>   |<span data-ttu-id="11149-130">Description</span><span class="sxs-lookup"><span data-stu-id="11149-130">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="11149-131">verifiedPublisherId</span><span class="sxs-lookup"><span data-stu-id="11149-131">verifiedPublisherId</span></span> | <span data-ttu-id="11149-132">string</span><span class="sxs-lookup"><span data-stu-id="11149-132">string</span></span> | <span data-ttu-id="11149-133">Microsoft 合作伙伴网络 ID 从发布者的合作伙伴中心帐户在应用程序上设置已验证的发布者 (MPNID) 。</span><span class="sxs-lookup"><span data-stu-id="11149-133">The Microsoft Partner Network ID (MPNID) of the verified publisher to be set on the application, from the publisher's Partner Center account.</span></span> |

## <a name="response"></a><span data-ttu-id="11149-134">响应</span><span class="sxs-lookup"><span data-stu-id="11149-134">Response</span></span>

<span data-ttu-id="11149-135">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="11149-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="11149-136">示例</span><span class="sxs-lookup"><span data-stu-id="11149-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="11149-137">请求</span><span class="sxs-lookup"><span data-stu-id="11149-137">Request</span></span>

<span data-ttu-id="11149-138">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="11149-138">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="11149-139">HTTP</span><span class="sxs-lookup"><span data-stu-id="11149-139">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="11149-140">JavaScript</span><span class="sxs-lookup"><span data-stu-id="11149-140">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-setverifiedpublisher-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="11149-141">响应</span><span class="sxs-lookup"><span data-stu-id="11149-141">Response</span></span>

<span data-ttu-id="11149-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="11149-142">The following is an example of the response.</span></span>

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
