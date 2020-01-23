---
title: 创建 activityBasedTimeoutPolicy
description: 创建新的 activityBasedTimeoutPolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7f061510c17cbd4a6ac1c41017a52f0e0d3160fa
ms.sourcegitcommit: 2f78ac96a9b0462626a242429055ef824590bd3f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2020
ms.locfileid: "41475426"
---
# <a name="create-activitybasedtimeoutpolicy"></a><span data-ttu-id="0092c-103">创建 activityBasedTimeoutPolicy</span><span class="sxs-lookup"><span data-stu-id="0092c-103">Create activityBasedTimeoutPolicy</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0092c-104">创建新的[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0092c-104">Create a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="0092c-105">权限</span><span class="sxs-lookup"><span data-stu-id="0092c-105">Permissions</span></span>

<span data-ttu-id="0092c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0092c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="0092c-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0092c-108">Permission type</span></span>                        | <span data-ttu-id="0092c-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0092c-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="0092c-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0092c-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="0092c-111">ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0092c-111">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="0092c-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0092c-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0092c-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0092c-113">Not supported.</span></span> |
| <span data-ttu-id="0092c-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0092c-114">Application</span></span>                            | <span data-ttu-id="0092c-115">ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="0092c-115">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="0092c-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0092c-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/activityBasedTimeoutPolicies
```

## <a name="request-headers"></a><span data-ttu-id="0092c-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0092c-117">Request headers</span></span>

| <span data-ttu-id="0092c-118">名称</span><span class="sxs-lookup"><span data-stu-id="0092c-118">Name</span></span>          | <span data-ttu-id="0092c-119">说明</span><span class="sxs-lookup"><span data-stu-id="0092c-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="0092c-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="0092c-120">Authorization</span></span> | <span data-ttu-id="0092c-121">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="0092c-121">Bearer {token}</span></span> |
| <span data-ttu-id="0092c-122">Content-type</span><span class="sxs-lookup"><span data-stu-id="0092c-122">Content-type</span></span> | <span data-ttu-id="0092c-123">application/json</span><span class="sxs-lookup"><span data-stu-id="0092c-123">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="0092c-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="0092c-124">Request body</span></span>

<span data-ttu-id="0092c-125">在请求正文中，提供[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0092c-125">In the request body, supply a JSON representation of [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="0092c-126">响应</span><span class="sxs-lookup"><span data-stu-id="0092c-126">Response</span></span>

<span data-ttu-id="0092c-127">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0092c-127">If successful, this method returns a `201 Created` response code and a new [activityBasedTimeoutPolicy](../resources/activitybasedtimeoutpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0092c-128">示例</span><span class="sxs-lookup"><span data-stu-id="0092c-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0092c-129">请求</span><span class="sxs-lookup"><span data-stu-id="0092c-129">Request</span></span>

<span data-ttu-id="0092c-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0092c-130">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="0092c-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="0092c-131">HTTP</span></span>](#tab/http)
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
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0092c-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0092c-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="0092c-133">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0092c-133">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-activitybasedtimeoutpolicy-from-activitybasedtimeoutpolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="0092c-134">响应</span><span class="sxs-lookup"><span data-stu-id="0092c-134">Response</span></span>

<span data-ttu-id="0092c-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0092c-135">The following is an example of the response.</span></span>

> <span data-ttu-id="0092c-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0092c-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
