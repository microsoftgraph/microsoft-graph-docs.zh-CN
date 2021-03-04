---
title: List appliesTo
description: 获取已应用 tokenLifetimePolicy 对象的 directoryObject 对象的列表。
localization_priority: Normal
author: lujiangfeng666
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: ac3df91789bb0be148ace7b5e26d94f8c34fae75
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50443340"
---
# <a name="list-appliesto"></a><span data-ttu-id="586c0-103">List appliesTo</span><span class="sxs-lookup"><span data-stu-id="586c0-103">List appliesTo</span></span>

<span data-ttu-id="586c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="586c0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="586c0-105">获取已应用[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象的[directoryObject](../resources/directoryObject.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="586c0-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object has been applied to.</span></span> <span data-ttu-id="586c0-106">tokenLifetimePolicy 只能应用于 [应用程序和](../resources/application.md) [servicePrincipal](../resources/serviceprincipal.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="586c0-106">The tokenLifetimePolicy can only be applied to [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="586c0-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="586c0-107">Permissions</span></span>

<span data-ttu-id="586c0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="586c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="586c0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="586c0-110">Permission type</span></span>                        | <span data-ttu-id="586c0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="586c0-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="586c0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="586c0-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="586c0-113">Policy.Read.All 和 Application.Read.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="586c0-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="586c0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="586c0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="586c0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="586c0-115">Not supported.</span></span> |
| <span data-ttu-id="586c0-116">Application</span><span class="sxs-lookup"><span data-stu-id="586c0-116">Application</span></span>                            | <span data-ttu-id="586c0-117">Policy.Read.All 和 Application.Read.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="586c0-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="586c0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="586c0-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenLifetimePolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="586c0-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="586c0-119">Optional query parameters</span></span>

<span data-ttu-id="586c0-120">此方法支持和 `$expand` `$select` `$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="586c0-120">This method supports the `$expand`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="586c0-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="586c0-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="586c0-122">使用 `$expand` 时，请确保你的应用请求读取扩展对象的权限。</span><span class="sxs-lookup"><span data-stu-id="586c0-122">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="586c0-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="586c0-123">Request headers</span></span>

| <span data-ttu-id="586c0-124">名称</span><span class="sxs-lookup"><span data-stu-id="586c0-124">Name</span></span>      |<span data-ttu-id="586c0-125">说明</span><span class="sxs-lookup"><span data-stu-id="586c0-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="586c0-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="586c0-126">Authorization</span></span> | <span data-ttu-id="586c0-127">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="586c0-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="586c0-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="586c0-128">Request body</span></span>

<span data-ttu-id="586c0-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="586c0-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="586c0-130">响应</span><span class="sxs-lookup"><span data-stu-id="586c0-130">Response</span></span>

<span data-ttu-id="586c0-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="586c0-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="586c0-132">示例</span><span class="sxs-lookup"><span data-stu-id="586c0-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="586c0-133">请求</span><span class="sxs-lookup"><span data-stu-id="586c0-133">Request</span></span>

<span data-ttu-id="586c0-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="586c0-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/beta/tokenLifetimePolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="586c0-135">响应</span><span class="sxs-lookup"><span data-stu-id="586c0-135">Response</span></span>

<span data-ttu-id="586c0-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="586c0-136">The following is an example of the response.</span></span>

> <span data-ttu-id="586c0-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="586c0-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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

