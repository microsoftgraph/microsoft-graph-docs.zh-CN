---
title: 列出 appliesTo
description: 获取已应用 homeRealmDiscoveryPolicy 对象的 directoryObject 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a8166c54c6ad62f2add344e4bd4ffd318b668af4
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234161"
---
# <a name="list-appliesto"></a><span data-ttu-id="49589-103">列出 appliesTo</span><span class="sxs-lookup"><span data-stu-id="49589-103">List appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="49589-104">获取已应用[homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md)对象的[directoryObject](../resources/directoryObject.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="49589-104">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [homeRealmDiscoveryPolicy](../resources/homerealmdiscoverypolicy.md) object has been applied to.</span></span> <span data-ttu-id="49589-105">HomeRealmDiscoveryPolicy 只能应用于[servicePrincipal](../resources/serviceprincipal.md)资源。</span><span class="sxs-lookup"><span data-stu-id="49589-105">The homeRealmDiscoveryPolicy can only be applied to [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="49589-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="49589-106">Permissions</span></span>

<span data-ttu-id="49589-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="49589-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="49589-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="49589-109">Permission type</span></span>                        | <span data-ttu-id="49589-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="49589-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="49589-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="49589-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="49589-112">Read. all 和 Application. all、Directory。 All</span><span class="sxs-lookup"><span data-stu-id="49589-112">Policy.Read.All and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="49589-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="49589-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="49589-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="49589-114">Not supported.</span></span> |
| <span data-ttu-id="49589-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="49589-115">Application</span></span>                            | <span data-ttu-id="49589-116">Read. all 和 Application. all、Directory。 All</span><span class="sxs-lookup"><span data-stu-id="49589-116">Policy.Read.All and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="49589-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="49589-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/homeRealmDiscoveryPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="49589-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="49589-118">Optional query parameters</span></span>

<span data-ttu-id="49589-119">此方法支持`$select`和`$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="49589-119">This method supports the `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="49589-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="49589-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="49589-121">请求头</span><span class="sxs-lookup"><span data-stu-id="49589-121">Request headers</span></span>

| <span data-ttu-id="49589-122">名称</span><span class="sxs-lookup"><span data-stu-id="49589-122">Name</span></span>      |<span data-ttu-id="49589-123">说明</span><span class="sxs-lookup"><span data-stu-id="49589-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="49589-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="49589-124">Authorization</span></span> | <span data-ttu-id="49589-125">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="49589-125">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="49589-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="49589-126">Request body</span></span>

<span data-ttu-id="49589-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="49589-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="49589-128">响应</span><span class="sxs-lookup"><span data-stu-id="49589-128">Response</span></span>

<span data-ttu-id="49589-129">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="49589-129">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="49589-130">示例</span><span class="sxs-lookup"><span data-stu-id="49589-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="49589-131">请求</span><span class="sxs-lookup"><span data-stu-id="49589-131">Request</span></span>

<span data-ttu-id="49589-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="49589-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/beta/homeRealmDiscoveryPolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="49589-133">响应</span><span class="sxs-lookup"><span data-stu-id="49589-133">Response</span></span>

<span data-ttu-id="49589-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="49589-134">The following is an example of the response.</span></span>

> <span data-ttu-id="49589-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="49589-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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