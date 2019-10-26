---
title: 'trustFrameworkKeySet: getActiveKey'
description: 获取键集中的活动键。
localization_priority: Normal
author: valnav
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: e0e45d1cb19f6591dac620569a2d48738b2089b5
ms.sourcegitcommit: 8bef2bc8b9e56d1a787ea2f0cda4ed94f05109ad
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/26/2019
ms.locfileid: "37734553"
---
# <a name="trustframeworkkeyset-getactivekey"></a><span data-ttu-id="2a184-103">trustFrameworkKeySet: getActiveKey</span><span class="sxs-lookup"><span data-stu-id="2a184-103">trustFrameworkKeySet: getActiveKey</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2a184-104">获取[trustFrameworkKeySet](../resources/trustframeworkkeyset.md)中当前处于活动状态的[trustFrameworkKey](../resources/trustframeworkkey.md) 。</span><span class="sxs-lookup"><span data-stu-id="2a184-104">Get the currently active [trustFrameworkKey](../resources/trustframeworkkey.md) in a [trustFrameworkKeySet](../resources/trustframeworkkeyset.md).</span></span> <span data-ttu-id="2a184-105">键集中一次只能有一个键处于活动状态。</span><span class="sxs-lookup"><span data-stu-id="2a184-105">Only one key is active in the keyset at a time.</span></span>


## <a name="permissions"></a><span data-ttu-id="2a184-106">权限</span><span class="sxs-lookup"><span data-stu-id="2a184-106">Permissions</span></span>

<span data-ttu-id="2a184-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a184-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a184-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a184-109">Permission type</span></span>                        | <span data-ttu-id="2a184-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2a184-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2a184-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a184-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a184-112">TrustFrameworkKeySet、TrustFrameworkKeySet、All。</span><span class="sxs-lookup"><span data-stu-id="2a184-112">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All.</span></span> |
| <span data-ttu-id="2a184-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a184-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a184-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a184-114">Not supported.</span></span> |
| <span data-ttu-id="2a184-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a184-115">Application</span></span>                            | <span data-ttu-id="2a184-116">TrustFrameworkKeySet、TrustFrameworkKeySet、All。</span><span class="sxs-lookup"><span data-stu-id="2a184-116">TrustFrameworkKeySet.Read.All, TrustFrameworkKeySet.ReadWrite.All.</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a184-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a184-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /trustFramework/keySets/{id}/getActiveKey
```

## <a name="request-headers"></a><span data-ttu-id="2a184-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a184-118">Request headers</span></span>

| <span data-ttu-id="2a184-119">名称</span><span class="sxs-lookup"><span data-stu-id="2a184-119">Name</span></span>          | <span data-ttu-id="2a184-120">说明</span><span class="sxs-lookup"><span data-stu-id="2a184-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="2a184-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a184-121">Authorization</span></span> | <span data-ttu-id="2a184-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2a184-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a184-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a184-124">Request body</span></span>

<span data-ttu-id="2a184-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2a184-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a184-126">响应</span><span class="sxs-lookup"><span data-stu-id="2a184-126">Response</span></span>

<span data-ttu-id="2a184-127">如果成功，此方法在响应`200 OK`正文中返回响应代码和新的[trustFrameworkKey](../resources/trustframeworkkey.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2a184-127">If successful, this method returns a `200 OK` response code and a new [trustFrameworkKey](../resources/trustframeworkkey.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a184-128">示例</span><span class="sxs-lookup"><span data-stu-id="2a184-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2a184-129">请求</span><span class="sxs-lookup"><span data-stu-id="2a184-129">Request</span></span>

<span data-ttu-id="2a184-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2a184-130">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "trustframeworkkeyset_getactivekey"
}-->

```http
POST https://graph.microsoft.com/beta/trustFramework/keySets/{id}/getActiveKey
```

### <a name="response"></a><span data-ttu-id="2a184-131">响应</span><span class="sxs-lookup"><span data-stu-id="2a184-131">Response</span></span>

<span data-ttu-id="2a184-132">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2a184-132">The following is an example of the response.</span></span>

> <span data-ttu-id="2a184-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2a184-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.trustFrameworkKey"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "k": "k-value",
  "x5c": [
    "x5c-value"
  ],
  "x5t": "x5t-value",
  "kty": "kty-value",
  "use": "use-value",
  "exp": 99
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "trustFrameworkKeySet: getActiveKey",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
