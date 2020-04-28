---
title: 创建 tokenIssuancePolicy
description: 创建新的 tokenIssuancePolicy。
localization_priority: Normal
author: luleonpla
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 56bb0c89d8194f73498f0847d533b2f2c97532b0
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917423"
---
# <a name="create-tokenissuancepolicy"></a><span data-ttu-id="a6fba-103">创建 tokenIssuancePolicy</span><span class="sxs-lookup"><span data-stu-id="a6fba-103">Create tokenIssuancePolicy</span></span>

<span data-ttu-id="a6fba-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a6fba-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a6fba-105">创建新的[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a6fba-105">Create a new [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="a6fba-106">权限</span><span class="sxs-lookup"><span data-stu-id="a6fba-106">Permissions</span></span>

<span data-ttu-id="a6fba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a6fba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="a6fba-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a6fba-109">Permission type</span></span>                        | <span data-ttu-id="a6fba-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a6fba-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="a6fba-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a6fba-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a6fba-112">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a6fba-112">Policy.ReadWrite.ApplicationConfiguration</span></span> |
| <span data-ttu-id="a6fba-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a6fba-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a6fba-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a6fba-114">Not supported.</span></span> |
| <span data-ttu-id="a6fba-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a6fba-115">Application</span></span>                            | <span data-ttu-id="a6fba-116">Policy.ReadWrite.ApplicationConfiguration</span><span class="sxs-lookup"><span data-stu-id="a6fba-116">Policy.ReadWrite.ApplicationConfiguration</span></span> |

## <a name="http-request"></a><span data-ttu-id="a6fba-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a6fba-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST policies/tokenIssuancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="a6fba-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a6fba-118">Request headers</span></span>

| <span data-ttu-id="a6fba-119">名称</span><span class="sxs-lookup"><span data-stu-id="a6fba-119">Name</span></span>          | <span data-ttu-id="a6fba-120">说明</span><span class="sxs-lookup"><span data-stu-id="a6fba-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="a6fba-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a6fba-121">Authorization</span></span> | <span data-ttu-id="a6fba-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a6fba-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a6fba-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="a6fba-124">Content-type</span></span> | <span data-ttu-id="a6fba-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a6fba-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="a6fba-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a6fba-127">Request body</span></span>

<span data-ttu-id="a6fba-128">在请求正文中，提供[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a6fba-128">In the request body, supply a JSON representation of a [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a6fba-129">响应</span><span class="sxs-lookup"><span data-stu-id="a6fba-129">Response</span></span>

<span data-ttu-id="a6fba-130">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a6fba-130">If successful, this method returns a `201 Created` response code and a new [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a6fba-131">示例</span><span class="sxs-lookup"><span data-stu-id="a6fba-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a6fba-132">请求</span><span class="sxs-lookup"><span data-stu-id="a6fba-132">Request</span></span>

<span data-ttu-id="a6fba-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a6fba-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a6fba-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="a6fba-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_tokenIssuancePolicies_from_tokenIssuancePolicies"
}-->

```http
POST https://graph.microsoft.com/beta/policies/tokenIssuancePolicies
Content-type: application/json

{
  "definition": [
    "definition-value"
  ],
  "displayName": "displayName-value",
  "isOrganizationDefault": true
}
```
# <a name="c"></a>[<span data-ttu-id="a6fba-135">C#</span><span class="sxs-lookup"><span data-stu-id="a6fba-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-tokenissuancepolicies-from-tokenissuancepolicies-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a6fba-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a6fba-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-tokenissuancepolicies-from-tokenissuancepolicies-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a6fba-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a6fba-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-tokenissuancepolicies-from-tokenissuancepolicies-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

---
### <a name="response"></a><span data-ttu-id="a6fba-138">响应</span><span class="sxs-lookup"><span data-stu-id="a6fba-138">Response</span></span>

<span data-ttu-id="a6fba-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a6fba-139">The following is an example of the response.</span></span>

> <span data-ttu-id="a6fba-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a6fba-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy"
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
  "description": "Create tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
