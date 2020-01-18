---
title: 列出 appliesTo
description: 获取已应用 tokenLifetimePolicy 对象的 directoryObject 对象的列表。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ec486f79c1f9c61c606c5630aa7810480a1d2b81
ms.sourcegitcommit: 0536ab327c8b8bf215b726e0d4c25e8f6e8996f9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/18/2020
ms.locfileid: "41234193"
---
# <a name="list-appliesto"></a><span data-ttu-id="18baa-103">列出 appliesTo</span><span class="sxs-lookup"><span data-stu-id="18baa-103">List appliesTo</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="18baa-104">获取已应用[tokenLifetimePolicy](../resources/tokenlifetimepolicy.md)对象的[directoryObject](../resources/directoryObject.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="18baa-104">Get a list of [directoryObject](../resources/directoryObject.md) objects that a [tokenLifetimePolicy](../resources/tokenlifetimepolicy.md) object has been applied to.</span></span> <span data-ttu-id="18baa-105">TokenLifetimePolicy 只能应用于[application](../resources/application.md)和[servicePrincipal](../resources/serviceprincipal.md)资源。</span><span class="sxs-lookup"><span data-stu-id="18baa-105">The tokenLifetimePolicy can only be applied to [application](../resources/application.md) and [servicePrincipal](../resources/serviceprincipal.md) resources.</span></span>

## <a name="permissions"></a><span data-ttu-id="18baa-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="18baa-106">Permissions</span></span>

<span data-ttu-id="18baa-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18baa-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="18baa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="18baa-109">Permission type</span></span>                        | <span data-ttu-id="18baa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="18baa-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="18baa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18baa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="18baa-112">Read. all 和 Application. all、Directory。 All</span><span class="sxs-lookup"><span data-stu-id="18baa-112">Policy.Read.All and Application.Read.All, Directory.Read.All</span></span> |
| <span data-ttu-id="18baa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18baa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="18baa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="18baa-114">Not supported.</span></span> |
| <span data-ttu-id="18baa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="18baa-115">Application</span></span>                            | <span data-ttu-id="18baa-116">Read. all 和 Application. all、Directory。 All</span><span class="sxs-lookup"><span data-stu-id="18baa-116">Policy.Read.All and Application.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="18baa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18baa-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /policies/tokenLifetimePolicies/{id}/appliesTo
```

## <a name="optional-query-parameters"></a><span data-ttu-id="18baa-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="18baa-118">Optional query parameters</span></span>

<span data-ttu-id="18baa-119">此方法支持`$expand` `$select`和`$top` OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="18baa-119">This method supports the `$expand`, `$select` and `$top` OData query parameters to help customize the response.</span></span> <span data-ttu-id="18baa-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="18baa-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span> <span data-ttu-id="18baa-121">使用`$expand`时，请确保您的应用程序请求读取扩展的对象的权限。</span><span class="sxs-lookup"><span data-stu-id="18baa-121">When using `$expand` make sure your app requests permissions to read the expanded objects.</span></span>

## <a name="request-headers"></a><span data-ttu-id="18baa-122">请求头</span><span class="sxs-lookup"><span data-stu-id="18baa-122">Request headers</span></span>

| <span data-ttu-id="18baa-123">名称</span><span class="sxs-lookup"><span data-stu-id="18baa-123">Name</span></span>      |<span data-ttu-id="18baa-124">说明</span><span class="sxs-lookup"><span data-stu-id="18baa-124">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="18baa-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="18baa-125">Authorization</span></span> | <span data-ttu-id="18baa-126">持有者 {token}</span><span class="sxs-lookup"><span data-stu-id="18baa-126">Bearer {token}</span></span> |

## <a name="request-body"></a><span data-ttu-id="18baa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="18baa-127">Request body</span></span>

<span data-ttu-id="18baa-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="18baa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18baa-129">响应</span><span class="sxs-lookup"><span data-stu-id="18baa-129">Response</span></span>

<span data-ttu-id="18baa-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="18baa-130">If successful, this method returns a `200 OK` response code and a collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="18baa-131">示例</span><span class="sxs-lookup"><span data-stu-id="18baa-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="18baa-132">请求</span><span class="sxs-lookup"><span data-stu-id="18baa-132">Request</span></span>

<span data-ttu-id="18baa-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="18baa-133">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_appliesto"
}-->

```http
GET https://graph.microsoft.com/beta/tokenLifetimePolicies/{id}/appliesTo
```

### <a name="response"></a><span data-ttu-id="18baa-134">响应</span><span class="sxs-lookup"><span data-stu-id="18baa-134">Response</span></span>

<span data-ttu-id="18baa-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="18baa-135">The following is an example of the response.</span></span>

> <span data-ttu-id="18baa-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="18baa-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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