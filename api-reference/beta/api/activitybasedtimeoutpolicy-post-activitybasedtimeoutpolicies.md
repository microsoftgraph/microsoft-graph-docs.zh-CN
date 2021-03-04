---
title: 创建 activityBasedTimeoutPolicy
description: 创建新的 activityBasedTimeoutPolicy。
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 40ca870f0ca8f65578723a2bc613077d735700e7
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50438979"
---
# <a name="create-activitybasedtimeoutpolicy"></a><span data-ttu-id="deefb-103">创建 activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="deefb-103">Create activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="deefb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="deefb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="deefb-105">创建新的 [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="deefb-105">Create a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="deefb-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="deefb-106">Permissions</span></span>

<span data-ttu-id="deefb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="deefb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="deefb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="deefb-109">Permission type</span></span>                        | <span data-ttu-id="deefb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="deefb-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="deefb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="deefb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="deefb-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="deefb-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="deefb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="deefb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="deefb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="deefb-114">Not supported.</span></span> |
| <span data-ttu-id="deefb-115">Application</span><span class="sxs-lookup"><span data-stu-id="deefb-115">Application</span></span>                            | <span data-ttu-id="deefb-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="deefb-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="deefb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="deefb-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/activityBasedTimeoutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="deefb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="deefb-118">Request headers</span></span>

| <span data-ttu-id="deefb-119">名称</span><span class="sxs-lookup"><span data-stu-id="deefb-119">Name</span></span>          | <span data-ttu-id="deefb-120">说明</span><span class="sxs-lookup"><span data-stu-id="deefb-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="deefb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="deefb-121">Authorization</span></span> | <span data-ttu-id="deefb-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="deefb-122">Bearer {token}</span></span> |
| <span data-ttu-id="deefb-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="deefb-123">Content-type</span></span> | <span data-ttu-id="deefb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="deefb-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="deefb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="deefb-125">Request body</span></span>

<span data-ttu-id="deefb-126">在请求正文中，提供 [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="deefb-126">In the request body, supply a JSON representation of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="deefb-127">响应</span><span class="sxs-lookup"><span data-stu-id="deefb-127">Response</span></span>

<span data-ttu-id="deefb-128">如果成功，此方法在响应正文中返回响应 `201 Created` 代码和新的 [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="deefb-128">If successful, this method returns a `201 Created` response code and a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="deefb-129">示例</span><span class="sxs-lookup"><span data-stu-id="deefb-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="deefb-130">请求</span><span class="sxs-lookup"><span data-stu-id="deefb-130">Request</span></span>

<span data-ttu-id="deefb-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="deefb-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="deefb-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="deefb-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_activitybasedtimeoutpolicy_from_activitybasedtimeoutpolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/activityBasedTimeoutPolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="deefb-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="deefb-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="deefb-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="deefb-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="deefb-135">C#</span><span class="sxs-lookup"><span data-stu-id="deefb-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="deefb-136">Java</span><span class="sxs-lookup"><span data-stu-id="deefb-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="deefb-137">响应</span><span class="sxs-lookup"><span data-stu-id="deefb-137">Response</span></span>

<span data-ttu-id="deefb-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="deefb-138">The following is an example of the response.</span></span>

> <span data-ttu-id="deefb-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="deefb-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.activityBasedTimeoutPolicy"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true,
  "id": "id-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create activityBasedTimeoutPolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


