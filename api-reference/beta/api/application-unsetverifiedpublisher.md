---
title: 应用程序： unsetVerifiedPublisher
description: 取消设置应用程序的已验证发布者。
localization_priority: Normal
author: jesakowi
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 88bf73cbd90b5bf1eb2c4c8f22d11a232d1cc581
ms.sourcegitcommit: 21481acf54471ff17ab8043b3a96fcb1d2f863d7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/21/2020
ms.locfileid: "48634677"
---
# <a name="application-unsetverifiedpublisher"></a><span data-ttu-id="63565-103">应用程序： unsetVerifiedPublisher</span><span class="sxs-lookup"><span data-stu-id="63565-103">application: unsetVerifiedPublisher</span></span>

<span data-ttu-id="63565-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63565-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63565-105">取消设置之前在[应用程序](../resources/application.md)上设置的[verifiedPublisher](../resources/verifiedPublisher.md) ，并删除所有已验证的发布服务器属性。</span><span class="sxs-lookup"><span data-stu-id="63565-105">Unset the the [verifiedPublisher](../resources/verifiedPublisher.md) previously set on an [application](../resources/application.md), removing all verified publisher properties.</span></span> <span data-ttu-id="63565-106">有关详细信息，请参阅 [Publisher 验证](/azure/active-directory/develop/publisher-verification-overview)。</span><span class="sxs-lookup"><span data-stu-id="63565-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="63565-107">权限</span><span class="sxs-lookup"><span data-stu-id="63565-107">Permissions</span></span>

|<span data-ttu-id="63565-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="63565-108">Permission type</span></span>      | <span data-ttu-id="63565-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63565-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63565-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63565-110">Delegated (work or school account)</span></span> | <span data-ttu-id="63565-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="63565-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="63565-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63565-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63565-113">不支持</span><span class="sxs-lookup"><span data-stu-id="63565-113">Not supported</span></span> |
|<span data-ttu-id="63565-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="63565-114">Application</span></span> | <span data-ttu-id="63565-115">不支持</span><span class="sxs-lookup"><span data-stu-id="63565-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="63565-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63565-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/unsetVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="63565-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="63565-117">Request headers</span></span>

| <span data-ttu-id="63565-118">名称</span><span class="sxs-lookup"><span data-stu-id="63565-118">Name</span></span>           | <span data-ttu-id="63565-119">说明</span><span class="sxs-lookup"><span data-stu-id="63565-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="63565-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="63565-120">Authorization</span></span>  | <span data-ttu-id="63565-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="63565-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="63565-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="63565-123">Request body</span></span>

<span data-ttu-id="63565-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="63565-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63565-125">响应</span><span class="sxs-lookup"><span data-stu-id="63565-125">Response</span></span>

<span data-ttu-id="63565-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="63565-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="63565-127">示例</span><span class="sxs-lookup"><span data-stu-id="63565-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="63565-128">请求</span><span class="sxs-lookup"><span data-stu-id="63565-128">Request</span></span>

<span data-ttu-id="63565-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="63565-129">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="63565-130">HTTP</span><span class="sxs-lookup"><span data-stu-id="63565-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "application_unsetverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/unsetVerifiedPublisher
```
# <a name="javascript"></a>[<span data-ttu-id="63565-131">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63565-131">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/application-unsetverifiedpublisher-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63565-132">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63565-132">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/application-unsetverifiedpublisher-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="63565-133">响应</span><span class="sxs-lookup"><span data-stu-id="63565-133">Response</span></span>

<span data-ttu-id="63565-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="63565-134">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: b0ed721f-7e6a-446c-89bc-2d03e1744dfe
2020-09-09 21:26:11 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "application: unsetVerifiedPublisher",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}-->
