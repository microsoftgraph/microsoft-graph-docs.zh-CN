---
title: 创建 activityBasedTimeoutPolicy
description: 创建新的 activityBasedTimeoutPolicy。
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 18f883410957e73bab9c8c74ddb411776de9c435
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52048321"
---
# <a name="create-activitybasedtimeoutpolicy"></a><span data-ttu-id="7f835-103">创建 activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="7f835-103">Create activityBasedTimeoutPolicy</span></span>

<span data-ttu-id="7f835-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7f835-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7f835-105">创建新的 [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f835-105">Create a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="7f835-106">权限</span><span class="sxs-lookup"><span data-stu-id="7f835-106">Permissions</span></span>

<span data-ttu-id="7f835-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f835-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="7f835-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f835-109">Permission type</span></span>                        | <span data-ttu-id="7f835-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7f835-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="7f835-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f835-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="7f835-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f835-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="7f835-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f835-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7f835-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f835-114">Not supported.</span></span> |
| <span data-ttu-id="7f835-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f835-115">Application</span></span>                            | <span data-ttu-id="7f835-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f835-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="7f835-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f835-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/activityBasedTimeoutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="7f835-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f835-118">Request headers</span></span>

| <span data-ttu-id="7f835-119">名称</span><span class="sxs-lookup"><span data-stu-id="7f835-119">Name</span></span>          | <span data-ttu-id="7f835-120">说明</span><span class="sxs-lookup"><span data-stu-id="7f835-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7f835-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f835-121">Authorization</span></span> | <span data-ttu-id="7f835-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="7f835-122">Bearer {token}</span></span> |
| <span data-ttu-id="7f835-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="7f835-123">Content-type</span></span> | <span data-ttu-id="7f835-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7f835-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="7f835-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f835-125">Request body</span></span>

<span data-ttu-id="7f835-126">在请求正文中，提供 [activityBasedTimeoutPolicy 对象的](../resources/activitybasedtimeoutpolicy.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f835-126">In the request body, supply a JSON representation of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="7f835-127">响应</span><span class="sxs-lookup"><span data-stu-id="7f835-127">Response</span></span>

<span data-ttu-id="7f835-128">如果成功，此方法在响应正文中返回 响应代码和新 `201 Created` [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f835-128">If successful, this method returns a `201 Created` response code and a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="7f835-129">示例</span><span class="sxs-lookup"><span data-stu-id="7f835-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="7f835-130">请求</span><span class="sxs-lookup"><span data-stu-id="7f835-130">Request</span></span>

<span data-ttu-id="7f835-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7f835-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7f835-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="7f835-132">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="7f835-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="7f835-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="7f835-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="7f835-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="7f835-135">C#</span><span class="sxs-lookup"><span data-stu-id="7f835-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="7f835-136">Java</span><span class="sxs-lookup"><span data-stu-id="7f835-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="7f835-137">响应</span><span class="sxs-lookup"><span data-stu-id="7f835-137">Response</span></span>

<span data-ttu-id="7f835-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7f835-138">The following is an example of the response.</span></span>

> <span data-ttu-id="7f835-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7f835-139">**Note:** The response object shown here might be shortened for readability.</span></span>

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


