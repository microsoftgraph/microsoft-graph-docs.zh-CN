---
title: 列表已分配 tokenIssuancePolicies
description: 列出分配给应用程序的 tokenIssuancePolicies。
localization_priority: Normal
author: sureshja
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 99e6811d3462afd64548063685e20225459d0f3a
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081276"
---
# <a name="list-assigned-tokenissuancepolicies"></a><span data-ttu-id="6a068-103">列表已分配 tokenIssuancePolicies</span><span class="sxs-lookup"><span data-stu-id="6a068-103">List assigned tokenIssuancePolicies</span></span>

<span data-ttu-id="6a068-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6a068-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a068-105">列出分配给[应用程序](../resources/application.md)的[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6a068-105">List the [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects that are assigned to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6a068-106">权限</span><span class="sxs-lookup"><span data-stu-id="6a068-106">Permissions</span></span>

<span data-ttu-id="6a068-107">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="6a068-107">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="6a068-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="6a068-108">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="6a068-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a068-109">Permission type</span></span>                        | <span data-ttu-id="6a068-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6a068-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="6a068-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a068-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="6a068-112">Policy. All 和 ApplicationConfiguration 和应用程序的所有读写全部。</span><span class="sxs-lookup"><span data-stu-id="6a068-112">Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |
| <span data-ttu-id="6a068-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a068-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a068-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a068-114">Not supported.</span></span> |
| <span data-ttu-id="6a068-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a068-115">Application</span></span>                            | <span data-ttu-id="6a068-116">Policy. All 和 Application.readwrite.ownedby、Application.readwrite.ownedby、ApplicationConfiguration 和、、ApplicationConfiguration 和应用程序的、、和和的所有应用程序中的</span><span class="sxs-lookup"><span data-stu-id="6a068-116">Policy.Read.All and Application.ReadWrite.OwnedBy, Policy.Read.All and Application.ReadWrite.All, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.OwnedBy, Policy.ReadWrite.ApplicationConfiguration and Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a068-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a068-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /applications/{id}/tokenIssuancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="6a068-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a068-118">Request headers</span></span>

| <span data-ttu-id="6a068-119">名称</span><span class="sxs-lookup"><span data-stu-id="6a068-119">Name</span></span>          | <span data-ttu-id="6a068-120">说明</span><span class="sxs-lookup"><span data-stu-id="6a068-120">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="6a068-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a068-121">Authorization</span></span> | <span data-ttu-id="6a068-122">Bearer {token}.</span><span class="sxs-lookup"><span data-stu-id="6a068-122">Bearer {token}.</span></span> <span data-ttu-id="6a068-123">Required.</span><span class="sxs-lookup"><span data-stu-id="6a068-123">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a068-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a068-124">Request body</span></span>

<span data-ttu-id="6a068-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6a068-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a068-126">响应</span><span class="sxs-lookup"><span data-stu-id="6a068-126">Response</span></span>

<span data-ttu-id="6a068-127">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[tokenIssuancePolicy](../resources/tokenissuancepolicy.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="6a068-127">If successful, this method returns a `200 OK` response code and a collection of [tokenIssuancePolicy](../resources/tokenissuancepolicy.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="6a068-128">示例</span><span class="sxs-lookup"><span data-stu-id="6a068-128">Examples</span></span>

### <a name="request"></a><span data-ttu-id="6a068-129">请求</span><span class="sxs-lookup"><span data-stu-id="6a068-129">Request</span></span>

<span data-ttu-id="6a068-130">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6a068-130">The following is an example of the request.</span></span>


# <a name="http"></a>[<span data-ttu-id="6a068-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="6a068-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_tokenissuancepolicies_on_application"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/applications/{id}/tokenIssuancePolicies
```

### <a name="response"></a><span data-ttu-id="6a068-132">响应</span><span class="sxs-lookup"><span data-stu-id="6a068-132">Response</span></span>

<span data-ttu-id="6a068-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6a068-133">The following is an example of the response.</span></span>

> <span data-ttu-id="6a068-134">**Note:** The response object shown here might be shortened for readability.</span><span class="sxs-lookup"><span data-stu-id="6a068-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="6a068-135">All the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="6a068-135">All the properties will be returned from an actual call.</span></span>

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
