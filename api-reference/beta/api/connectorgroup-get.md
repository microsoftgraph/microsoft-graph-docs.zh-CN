---
title: Get connectorGroup
description: 检索 connectorGroup 对象的属性。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 9207236c7470fe4bdc7d7c638f573dd17bd3d992
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047180"
---
# <a name="get-connectorgroup"></a><span data-ttu-id="0af50-103">Get connectorGroup</span><span class="sxs-lookup"><span data-stu-id="0af50-103">Get connectorGroup</span></span>

<span data-ttu-id="0af50-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0af50-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0af50-105">检索 [connectorGroup 的属性](../resources/connectorgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="0af50-105">Retrieve the properties of a [connectorGroup](../resources/connectorgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="0af50-106">权限</span><span class="sxs-lookup"><span data-stu-id="0af50-106">Permissions</span></span>
<span data-ttu-id="0af50-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0af50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0af50-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="0af50-109">Permission type</span></span>      | <span data-ttu-id="0af50-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0af50-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0af50-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0af50-111">Delegated (work or school account)</span></span> | <span data-ttu-id="0af50-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0af50-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0af50-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0af50-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0af50-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="0af50-114">Not supported.</span></span>    |
|<span data-ttu-id="0af50-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="0af50-115">Application</span></span> | <span data-ttu-id="0af50-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0af50-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="0af50-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0af50-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="optional-query-parameters"></a><span data-ttu-id="0af50-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0af50-118">Optional query parameters</span></span>
<span data-ttu-id="0af50-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0af50-119">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0af50-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0af50-120">Request headers</span></span>
| <span data-ttu-id="0af50-121">名称</span><span class="sxs-lookup"><span data-stu-id="0af50-121">Name</span></span>      |<span data-ttu-id="0af50-122">说明</span><span class="sxs-lookup"><span data-stu-id="0af50-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0af50-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0af50-123">Authorization</span></span>  | <span data-ttu-id="0af50-124">Bearer。</span><span class="sxs-lookup"><span data-stu-id="0af50-124">Bearer.</span></span> <span data-ttu-id="0af50-125">必需</span><span class="sxs-lookup"><span data-stu-id="0af50-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="0af50-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0af50-126">Request body</span></span>
<span data-ttu-id="0af50-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0af50-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0af50-128">响应</span><span class="sxs-lookup"><span data-stu-id="0af50-128">Response</span></span>

<span data-ttu-id="0af50-129">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [connectorGroup](../resources/connectorgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0af50-129">If successful, this method returns a `200 OK` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0af50-130">示例</span><span class="sxs-lookup"><span data-stu-id="0af50-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="0af50-131">请求</span><span class="sxs-lookup"><span data-stu-id="0af50-131">Request</span></span>
<span data-ttu-id="0af50-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="0af50-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="0af50-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="0af50-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectorgroup"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="0af50-134">C#</span><span class="sxs-lookup"><span data-stu-id="0af50-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="0af50-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="0af50-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="0af50-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="0af50-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="0af50-137">Java</span><span class="sxs-lookup"><span data-stu-id="0af50-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-connectorgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="0af50-138">响应</span><span class="sxs-lookup"><span data-stu-id="0af50-138">Response</span></span>
<span data-ttu-id="0af50-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="0af50-139">The following is an example of the response.</span></span> <span data-ttu-id="0af50-140">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0af50-140">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false,
  "region": "region-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->

