---
title: List appliesTo
description: 获取 claimsMappingPolicy 对象已应用到的 directoryObject 对象的列表。
localization_priority: Normal
author: paulgarn
ms.prod: identity-and-sign-in
doc_type: apiPageType
ms.openlocfilehash: 710c0094a1e81d026f0933fe6fd4185c5af39616
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047270"
---
# <a name="list-appliesto"></a><span data-ttu-id="956b8-103">List appliesTo</span><span class="sxs-lookup"><span data-stu-id="956b8-103">List appliesTo</span></span>

<span data-ttu-id="956b8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="956b8-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="956b8-105">获取[claimsMappingPolicy](../resources/claimsmappingpolicy.md)对象已应用到的[directoryObject](../resources/directoryObject.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="956b8-105">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [claimsMappingPolicy](../resources/claimsmappingpolicy.md) object has been applied to.</span></span> <span data-ttu-id="956b8-106">claimsMappingPolicy 只能应用于 [application](../resources/application.md) 和 [servicePrincipal](../resources/serviceprincipal.md) 资源。</span><span class="sxs-lookup"><span data-stu-id="956b8-106">The claimsMappingPolicy can only be applied to [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="956b8-107">权限</span><span class="sxs-lookup"><span data-stu-id="956b8-107">Permissions</span></span>

<span data-ttu-id="956b8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="956b8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="956b8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="956b8-110">Permission type</span></span>                        | <span data-ttu-id="956b8-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="956b8-111">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="956b8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="956b8-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="956b8-113">Policy.Read.All 和 Application.Read.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="956b8-113">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="956b8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="956b8-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="956b8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="956b8-115">Not supported.</span></span> |
| <span data-ttu-id="956b8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="956b8-116">Application</span></span>                            | <span data-ttu-id="956b8-117">Policy.Read.All 和 Application.Read.All、Policy.ReadWrite.ApplicationConfiguration 和 Application.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="956b8-117">Policy.Read.All and Application.Read.All, Policy.ReadWrite.ApplicationConfiguration and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="956b8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="956b8-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/claimsMappingPolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="956b8-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="956b8-119">Optional query parameters</span></span>

<span data-ttu-id="956b8-120">此方法支持 `$expand` 、 `$select` 和 `$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="956b8-120">This method supports the `$expand`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="956b8-121">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="956b8-121">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="956b8-122">使用 `$expand` 时，请确保你的应用请求读取扩展对象的权限。</span><span class="sxs-lookup"><span data-stu-id="956b8-122">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="956b8-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="956b8-123">Request headers</span></span>

| <span data-ttu-id="956b8-124">名称</span><span class="sxs-lookup"><span data-stu-id="956b8-124">Name</span></span>      |<span data-ttu-id="956b8-125">说明</span><span class="sxs-lookup"><span data-stu-id="956b8-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="956b8-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="956b8-126">Authorization</span></span> | <span data-ttu-id="956b8-127">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="956b8-127">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="956b8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="956b8-128">Request body</span></span>

<span data-ttu-id="956b8-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="956b8-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="956b8-130">响应</span><span class="sxs-lookup"><span data-stu-id="956b8-130">Response</span></span>

<span data-ttu-id="956b8-131">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="956b8-131">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="956b8-132">示例</span><span class="sxs-lookup"><span data-stu-id="956b8-132">Examples</span></span>

### <a name="request"></a><span data-ttu-id="956b8-133">请求</span><span class="sxs-lookup"><span data-stu-id="956b8-133">Request</span></span>

<span data-ttu-id="956b8-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="956b8-134">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="956b8-135">HTTP</span><span class="sxs-lookup"><span data-stu-id="956b8-135">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_appliesto_1"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/policies/claimsMappingPolicies/{id}/appliesTo
```
# <a name="c"></a>[<span data-ttu-id="956b8-136">C#</span><span class="sxs-lookup"><span data-stu-id="956b8-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-appliesto-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="956b8-137">JavaScript</span><span class="sxs-lookup"><span data-stu-id="956b8-137">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-appliesto-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="956b8-138">Objective-C</span><span class="sxs-lookup"><span data-stu-id="956b8-138">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-appliesto-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="956b8-139">Java</span><span class="sxs-lookup"><span data-stu-id="956b8-139">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-appliesto-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="956b8-140">响应</span><span class="sxs-lookup"><span data-stu-id="956b8-140">Response</span></span>

<span data-ttu-id="956b8-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="956b8-141">The following is an example of the response.</span></span>

> <span data-ttu-id="956b8-142">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="956b8-142">**Note:** The response object shown here might be shortened for readability.</span></span>

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

