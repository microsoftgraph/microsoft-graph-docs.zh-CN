---
title: 创建 tokenLifetimePolicy
description: 创建新的 tokenLifetimePolicy。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0774e2fb497f94da56cd95130585cebfa86c9814
ms.sourcegitcommit: c4d6ccd343a6b298a2aa844f1bad66c736487251
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2020
ms.locfileid: "42589286"
---
# <a name="create-tokenlifetimepolicy"></a><span data-ttu-id="8cada-103">创建 tokenLifetimePolicy</span><span class="sxs-lookup"><span data-stu-id="8cada-103">Create tokenLifetimePolicy</span></span>

<span data-ttu-id="8cada-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cada-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8cada-105">创建新的[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8cada-105">Create a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="8cada-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="8cada-106">Permissions</span></span>

<span data-ttu-id="8cada-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8cada-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8cada-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8cada-109">Permission type</span></span>                        | <span data-ttu-id="8cada-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8cada-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8cada-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8cada-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8cada-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8cada-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="8cada-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8cada-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8cada-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8cada-114">Not supported.</span></span> |
| <span data-ttu-id="8cada-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8cada-115">Application</span></span>                            | <span data-ttu-id="8cada-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="8cada-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="8cada-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8cada-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenLifetimePolicies
```

## <a name="request-headers"></a><span data-ttu-id="8cada-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8cada-118">Request headers</span></span>

| <span data-ttu-id="8cada-119">名称</span><span class="sxs-lookup"><span data-stu-id="8cada-119">Name</span></span>          | <span data-ttu-id="8cada-120">说明</span><span class="sxs-lookup"><span data-stu-id="8cada-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8cada-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8cada-121">Authorization</span></span> | <span data-ttu-id="8cada-122">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="8cada-122">Bearer {token}</span></span> |
| <span data-ttu-id="8cada-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="8cada-123">Content-type</span></span> | <span data-ttu-id="8cada-124">application/json</span><span class="sxs-lookup"><span data-stu-id="8cada-124">application/json</span></span> |

## <a name="request-body"></a><span data-ttu-id="8cada-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="8cada-125">Request body</span></span>

<span data-ttu-id="8cada-126">在请求正文中，提供[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8cada-126">In the request body, supply a JSON representation of [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="8cada-127">响应</span><span class="sxs-lookup"><span data-stu-id="8cada-127">Response</span></span>

<span data-ttu-id="8cada-128">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8cada-128">If successful, this method returns a `201 Created` response code and a new [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8cada-129">示例</span><span class="sxs-lookup"><span data-stu-id="8cada-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8cada-130">请求</span><span class="sxs-lookup"><span data-stu-id="8cada-130">Request</span></span>

<span data-ttu-id="8cada-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8cada-131">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="8cada-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="8cada-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenlifetimepolicy_from_tokenlifetimepolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/tokenLifetimePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="javascript"></a>[<span data-ttu-id="8cada-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8cada-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenlifetimepolicy-from-tokenlifetimepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8cada-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8cada-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenlifetimepolicy-from-tokenlifetimepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="8cada-135">C#</span><span class="sxs-lookup"><span data-stu-id="8cada-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenlifetimepolicy-from-tokenlifetimepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8cada-136">响应</span><span class="sxs-lookup"><span data-stu-id="8cada-136">Response</span></span>

<span data-ttu-id="8cada-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8cada-137">The following is an example of the response.</span></span>

> <span data-ttu-id="8cada-p102">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="8cada-p102">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenLifetimePolicy"
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
  "description": "Create tokenLifetimePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
