---
title: 应用程序： unsetVerifiedPublisher
description: 取消设置应用程序的已验证发布者。
localization_priority: Normal
author: jesakowi
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1f904a4b13e162dc503765b03d676319d3d0a510
ms.sourcegitcommit: c28da0e5feea4791c19663a30b223a0a5da0ed02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/15/2020
ms.locfileid: "48471549"
---
# <a name="application-unsetverifiedpublisher"></a><span data-ttu-id="08141-103">应用程序： unsetVerifiedPublisher</span><span class="sxs-lookup"><span data-stu-id="08141-103">application: unsetVerifiedPublisher</span></span>

<span data-ttu-id="08141-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08141-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="08141-105">取消设置之前在[应用程序](../resources/application.md)上设置的[verifiedPublisher](../resources/verifiedPublisher.md) ，并删除所有已验证的发布服务器属性。</span><span class="sxs-lookup"><span data-stu-id="08141-105">Unset the the [verifiedPublisher](../resources/verifiedPublisher.md) previously set on an [application](../resources/application.md), removing all verified publisher properties.</span></span> <span data-ttu-id="08141-106">有关详细信息，请参阅 [Publisher 验证](/azure/active-directory/develop/publisher-verification-overview)。</span><span class="sxs-lookup"><span data-stu-id="08141-106">For more information, see [Publisher verification](/azure/active-directory/develop/publisher-verification-overview).</span></span>

## <a name="permissions"></a><span data-ttu-id="08141-107">权限</span><span class="sxs-lookup"><span data-stu-id="08141-107">Permissions</span></span>

|<span data-ttu-id="08141-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="08141-108">Permission type</span></span>      | <span data-ttu-id="08141-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="08141-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="08141-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08141-110">Delegated (work or school account)</span></span> | <span data-ttu-id="08141-111">Application.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08141-111">Application.ReadWrite.All</span></span> |
|<span data-ttu-id="08141-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08141-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="08141-113">不支持</span><span class="sxs-lookup"><span data-stu-id="08141-113">Not supported</span></span> |
|<span data-ttu-id="08141-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="08141-114">Application</span></span> | <span data-ttu-id="08141-115">不支持</span><span class="sxs-lookup"><span data-stu-id="08141-115">Not supported</span></span> |

## <a name="http-request"></a><span data-ttu-id="08141-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08141-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /applications/{id}/unsetVerifiedPublisher
```

## <a name="request-headers"></a><span data-ttu-id="08141-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="08141-117">Request headers</span></span>

| <span data-ttu-id="08141-118">名称</span><span class="sxs-lookup"><span data-stu-id="08141-118">Name</span></span>           | <span data-ttu-id="08141-119">说明</span><span class="sxs-lookup"><span data-stu-id="08141-119">Description</span></span>                |
|:---------------|:---------------------------|
| <span data-ttu-id="08141-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="08141-120">Authorization</span></span>  | <span data-ttu-id="08141-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="08141-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="08141-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="08141-123">Request body</span></span>

<span data-ttu-id="08141-124">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="08141-124">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08141-125">响应</span><span class="sxs-lookup"><span data-stu-id="08141-125">Response</span></span>

<span data-ttu-id="08141-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="08141-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="08141-127">示例</span><span class="sxs-lookup"><span data-stu-id="08141-127">Example</span></span>

### <a name="request"></a><span data-ttu-id="08141-128">请求</span><span class="sxs-lookup"><span data-stu-id="08141-128">Request</span></span>

<span data-ttu-id="08141-129">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="08141-129">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "application_unsetverifiedpublisher"
}-->

```http
POST https://graph.microsoft.com/beta/applications/{id}/unsetVerifiedPublisher
```

### <a name="response"></a><span data-ttu-id="08141-130">响应</span><span class="sxs-lookup"><span data-stu-id="08141-130">Response</span></span>

<span data-ttu-id="08141-131">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="08141-131">The following is an example of the response.</span></span>

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
