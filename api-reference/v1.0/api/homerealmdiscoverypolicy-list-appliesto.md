---
title: 列出 appliesTo
description: 获取已应用 homeRealmDiscoveryPolicy 对象的 directoryObject 对象的列表。
localization_priority: Normal
author: hpsin
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 6a2c9ab763f5fa494a8be66a05ab32b31b0f4348
ms.sourcegitcommit: 79988a42d91cc25bdd1c531b5f3261901d720a9a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/28/2020
ms.locfileid: "43917339"
---
# <a name="list-appliesto"></a><span data-ttu-id="2a91b-103">列出 appliesTo</span><span class="sxs-lookup"><span data-stu-id="2a91b-103">List appliesTo</span></span>

<span data-ttu-id="2a91b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a91b-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2a91b-105">获取已应用[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)对象的[directoryObject](../resources/directoryObject.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="2a91b-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object has been applied to.</span></span>

## <a name="permissions"></a><span data-ttu-id="2a91b-106">权限</span><span class="sxs-lookup"><span data-stu-id="2a91b-106">Permissions</span></span>

<span data-ttu-id="2a91b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a91b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="2a91b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a91b-109">Permission type</span></span>                        | <span data-ttu-id="2a91b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2a91b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="2a91b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a91b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="2a91b-112">Policy. all 和 application. all、ApplicationConfiguration 和 Application。 all，All，Read. All</span><span class="sxs-lookup"><span data-stu-id="2a91b-112">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="2a91b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a91b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2a91b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a91b-114">Not supported.</span></span> |
| <span data-ttu-id="2a91b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a91b-115">Application</span></span>                            | <span data-ttu-id="2a91b-116">Policy. all 和 application. all、ApplicationConfiguration 和 Application。 all，All，Read. All</span><span class="sxs-lookup"><span data-stu-id="2a91b-116">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2a91b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a91b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="2a91b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="2a91b-118">Optional query parameters</span></span>

<span data-ttu-id="2a91b-119">此方法支持`$select`和`$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="2a91b-119">This method supports the `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="2a91b-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="2a91b-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="2a91b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a91b-121">Request headers</span></span>

| <span data-ttu-id="2a91b-122">名称</span><span class="sxs-lookup"><span data-stu-id="2a91b-122">Name</span></span>      |<span data-ttu-id="2a91b-123">说明</span><span class="sxs-lookup"><span data-stu-id="2a91b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="2a91b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a91b-124">Authorization</span></span> | <span data-ttu-id="2a91b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2a91b-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="2a91b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a91b-127">Request body</span></span>

<span data-ttu-id="2a91b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2a91b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2a91b-129">响应</span><span class="sxs-lookup"><span data-stu-id="2a91b-129">Response</span></span>

<span data-ttu-id="2a91b-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2a91b-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2a91b-131">示例</span><span class="sxs-lookup"><span data-stu-id="2a91b-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2a91b-132">请求</span><span class="sxs-lookup"><span data-stu-id="2a91b-132">Request</span></span>

<span data-ttu-id="2a91b-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2a91b-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/v1.0/homeRealmDiscoveryPolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="2a91b-134">响应</span><span class="sxs-lookup"><span data-stu-id="2a91b-134">Response</span></span>

<span data-ttu-id="2a91b-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2a91b-135">The following is an example of the response.</span></span>

> <span data-ttu-id="2a91b-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="2a91b-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "id": "id-value",
      "deletedDateTime": "datetime-value"
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List appliesTo",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->