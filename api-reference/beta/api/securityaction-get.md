---
title: 获取 securityAction
description: 检索 securityAction 对象的属性和关系。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: apiPageType
ms.openlocfilehash: 206f0384fe3c592ca1daf67c0d401eb16b7aed16
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42453574"
---
# <a name="get-securityaction"></a><span data-ttu-id="c951b-103">获取 securityAction</span><span class="sxs-lookup"><span data-stu-id="c951b-103">Get securityAction</span></span>

<span data-ttu-id="c951b-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c951b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c951b-105">检索[securityAction](../resources/securityaction.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c951b-105">Retrieve the properties and relationships of a [securityAction](../resources/securityaction.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="c951b-106">权限</span><span class="sxs-lookup"><span data-stu-id="c951b-106">Permissions</span></span>

<span data-ttu-id="c951b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c951b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="c951b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c951b-109">Permission type</span></span>                        | <span data-ttu-id="c951b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c951b-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="c951b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c951b-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="c951b-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="c951b-112">Not supported.</span></span> |
| <span data-ttu-id="c951b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c951b-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c951b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c951b-114">Not supported.</span></span> |
| <span data-ttu-id="c951b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c951b-115">Application</span></span>                            | <span data-ttu-id="c951b-116">SecurityActions、SecurityActions 和所有</span><span class="sxs-lookup"><span data-stu-id="c951b-116">SecurityActions.Read.All, SecurityActions.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c951b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c951b-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /security/securityActions/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c951b-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c951b-118">Optional query parameters</span></span>

<span data-ttu-id="c951b-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c951b-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="c951b-120">有关一般信息，请参阅[OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="c951b-120">For general information, see [OData Query Parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="c951b-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c951b-121">Request headers</span></span>

| <span data-ttu-id="c951b-122">名称</span><span class="sxs-lookup"><span data-stu-id="c951b-122">Name</span></span>      |<span data-ttu-id="c951b-123">说明</span><span class="sxs-lookup"><span data-stu-id="c951b-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c951b-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c951b-124">Authorization</span></span> | <span data-ttu-id="c951b-125">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="c951b-125">Bearer {code}</span></span> |

## <a name="request-body"></a><span data-ttu-id="c951b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c951b-126">Request body</span></span>

<span data-ttu-id="c951b-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c951b-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c951b-128">响应</span><span class="sxs-lookup"><span data-stu-id="c951b-128">Response</span></span>

<span data-ttu-id="c951b-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和[securityAction](../resources/securityaction.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c951b-129">If successful, this method returns a `200 OK` response code and a [securityAction](../resources/securityaction.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c951b-130">示例</span><span class="sxs-lookup"><span data-stu-id="c951b-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c951b-131">请求</span><span class="sxs-lookup"><span data-stu-id="c951b-131">Request</span></span>

<span data-ttu-id="c951b-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c951b-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c951b-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c951b-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_securityaction"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/beta/security/securityActions/{id}
```
# <a name="c"></a>[<span data-ttu-id="c951b-134">C#</span><span class="sxs-lookup"><span data-stu-id="c951b-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-securityaction-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c951b-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c951b-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-securityaction-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c951b-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c951b-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-securityaction-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c951b-137">响应</span><span class="sxs-lookup"><span data-stu-id="c951b-137">Response</span></span>

<span data-ttu-id="c951b-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c951b-138">The following is an example of the response.</span></span>

> [!NOTE]
> <span data-ttu-id="c951b-139">为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c951b-139">The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c951b-140">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c951b-140">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.securityAction"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "actionReason": "actionReason-value",
  "appId": "appId-value",
  "azureTenantId": "azureTenantId-value",
  "clientContext": "clientContext-value",
  "completedDateTime": "datetime-value",
  "createdDateTime": "datetime-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Get securityAction",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
