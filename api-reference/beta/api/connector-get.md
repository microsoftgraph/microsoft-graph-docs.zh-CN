---
title: 获取连接器
description: 检索连接器对象的属性。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a93e5c4cbafc541136ea91204b4c279ff612caf1
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681569"
---
# <a name="get-connector"></a><span data-ttu-id="99deb-103">获取连接器</span><span class="sxs-lookup"><span data-stu-id="99deb-103">Get connector</span></span>

<span data-ttu-id="99deb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99deb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="99deb-105">检索[连接器](../resources/connector.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="99deb-105">Retrieve the properties and relationships of a [connector](../resources/connector.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="99deb-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="99deb-106">Permissions</span></span>
<span data-ttu-id="99deb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99deb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99deb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="99deb-109">Permission type</span></span>      | <span data-ttu-id="99deb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99deb-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="99deb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99deb-111">Delegated (work or school account)</span></span> | <span data-ttu-id="99deb-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="99deb-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="99deb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99deb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="99deb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="99deb-114">Not supported.</span></span>    |
|<span data-ttu-id="99deb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="99deb-115">Application</span></span> | <span data-ttu-id="99deb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="99deb-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="99deb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99deb-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectors/{id}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="99deb-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="99deb-118">Optional query parameters</span></span>
<span data-ttu-id="99deb-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="99deb-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="99deb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="99deb-120">Request headers</span></span>
| <span data-ttu-id="99deb-121">名称</span><span class="sxs-lookup"><span data-stu-id="99deb-121">Name</span></span>      |<span data-ttu-id="99deb-122">说明</span><span class="sxs-lookup"><span data-stu-id="99deb-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="99deb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="99deb-123">Authorization</span></span>  | <span data-ttu-id="99deb-124">负载.</span><span class="sxs-lookup"><span data-stu-id="99deb-124">Bearer.</span></span> <span data-ttu-id="99deb-125">必需</span><span class="sxs-lookup"><span data-stu-id="99deb-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="99deb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="99deb-126">Request body</span></span>
<span data-ttu-id="99deb-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="99deb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="99deb-128">响应</span><span class="sxs-lookup"><span data-stu-id="99deb-128">Response</span></span>

<span data-ttu-id="99deb-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[连接器](../resources/connector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="99deb-129">If successful, this method returns a `200 OK` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99deb-130">示例</span><span class="sxs-lookup"><span data-stu-id="99deb-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="99deb-131">请求</span><span class="sxs-lookup"><span data-stu-id="99deb-131">Request</span></span>

<span data-ttu-id="99deb-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="99deb-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="99deb-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="99deb-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connector"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}
```
# <a name="c"></a>[<span data-ttu-id="99deb-134">C#</span><span class="sxs-lookup"><span data-stu-id="99deb-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="99deb-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="99deb-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="99deb-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="99deb-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="99deb-137">响应</span><span class="sxs-lookup"><span data-stu-id="99deb-137">Response</span></span>
<span data-ttu-id="99deb-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="99deb-138">The following is an example of the response.</span></span> <span data-ttu-id="99deb-139">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="99deb-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="99deb-140">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="99deb-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 124

{
  "id": "id-value",
  "machineName": "machineName-value",
  "externalIp": "externalIp-value",
  "status": "status-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
