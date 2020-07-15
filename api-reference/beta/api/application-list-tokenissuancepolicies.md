---
title: 列表已分配 tokenIssuancePolicies
description: 列出分配给应用程序的 tokenIssuancePolicies。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 1c39d82332e2ea278afd169f059e642c66c59bdc
ms.sourcegitcommit: 2c8a12389b82ee5101b2bd17eae11b42e65e52c0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2020
ms.locfileid: "45142239"
---
# <a name="list-assigned-tokenissuancepolicies"></a><span data-ttu-id="8c8c8-103">列表已分配 tokenIssuancePolicies</span><span class="sxs-lookup"><span data-stu-id="8c8c8-103">List assigned tokenIssuancePolicies</span></span>

<span data-ttu-id="8c8c8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8c8c8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8c8c8-105">列出分配给[应用程序](../resources/application.md)的[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8c8c8-105">List the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="8c8c8-106">权限</span><span class="sxs-lookup"><span data-stu-id="8c8c8-106">Permissions</span></span>

<span data-ttu-id="8c8c8-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="8c8c8-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="8c8c8-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="8c8c8-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="8c8c8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="8c8c8-109">Permission type</span></span>                        | <span data-ttu-id="8c8c8-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8c8c8-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="8c8c8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8c8c8-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="8c8c8-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="8c8c8-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="8c8c8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8c8c8-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8c8c8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="8c8c8-114">Not supported.</span></span> |
| <span data-ttu-id="8c8c8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="8c8c8-115">Application</span></span>                            | <span data-ttu-id="8c8c8-116">Policy. All 和 Application.readwrite.ownedby、Application.readwrite.ownedby、ApplicationConfiguration 和、、ApplicationConfiguration 和应用程序的、、和和的所有应用程序中的</span><span class="sxs-lookup"><span data-stu-id="8c8c8-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8c8c8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8c8c8-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenIssuancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="8c8c8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="8c8c8-118">Request headers</span></span>

| <span data-ttu-id="8c8c8-119">名称</span><span class="sxs-lookup"><span data-stu-id="8c8c8-119">Name</span></span>          | <span data-ttu-id="8c8c8-120">说明</span><span class="sxs-lookup"><span data-stu-id="8c8c8-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="8c8c8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="8c8c8-121">Authorization</span></span> | <span data-ttu-id="8c8c8-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="8c8c8-122">Bearer {token}.</span></span> <span data-ttu-id="8c8c8-123">Required.</span><span class="sxs-lookup"><span data-stu-id="8c8c8-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8c8c8-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="8c8c8-124">Request body</span></span>

<span data-ttu-id="8c8c8-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8c8c8-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8c8c8-126">响应</span><span class="sxs-lookup"><span data-stu-id="8c8c8-126">Response</span></span>

<span data-ttu-id="8c8c8-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="8c8c8-127">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="8c8c8-128">示例</span><span class="sxs-lookup"><span data-stu-id="8c8c8-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="8c8c8-129">请求</span><span class="sxs-lookup"><span data-stu-id="8c8c8-129">Request</span></span>

<span data-ttu-id="8c8c8-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="8c8c8-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="8c8c8-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="8c8c8-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenissuancepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies
```
# <a name="c"></a>[<span data-ttu-id="8c8c8-132">C#</span><span class="sxs-lookup"><span data-stu-id="8c8c8-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-tokenissuancepolicies-on-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="8c8c8-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="8c8c8-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-tokenissuancepolicies-on-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="8c8c8-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="8c8c8-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-tokenissuancepolicies-on-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="8c8c8-135">响应</span><span class="sxs-lookup"><span data-stu-id="8c8c8-135">Response</span></span>

<span data-ttu-id="8c8c8-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="8c8c8-136">The following is an example of the response.</span></span>

> <span data-ttu-id="8c8c8-137">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="8c8c8-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="8c8c8-138">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="8c8c8-138">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.tokenIssuancePolicy",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "definition": [
        "definition-value"
      ],
      "displayName": "displayName-value",
      "isOrganizationDefault": true,
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List assigned tokenIssuancePolicy",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
