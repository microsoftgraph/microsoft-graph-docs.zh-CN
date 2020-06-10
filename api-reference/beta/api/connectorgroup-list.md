---
title: 列出 connectorGroups
description: 检索 connectorgroup 对象的列表。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: bdbf86c846bfc3277b3ce96198239d86e0c90408
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681321"
---
# <a name="list-connectorgroups"></a><span data-ttu-id="c273c-103">列出 connectorGroups</span><span class="sxs-lookup"><span data-stu-id="c273c-103">List connectorGroups</span></span>

<span data-ttu-id="c273c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c273c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c273c-105">检索[connectorGroup](../resources/connectorgroup.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="c273c-105">Retrieve a list of [connectorGroup](../resources/connectorgroup.md) objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="c273c-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="c273c-106">Permissions</span></span>
<span data-ttu-id="c273c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c273c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c273c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c273c-109">Permission type</span></span>      | <span data-ttu-id="c273c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c273c-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c273c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c273c-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c273c-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c273c-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c273c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c273c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c273c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c273c-114">Not supported.</span></span>    |
|<span data-ttu-id="c273c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c273c-115">Application</span></span> | <span data-ttu-id="c273c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c273c-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="c273c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c273c-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /onPremisesPublishingProfiles/applicationProxy/connectorGroups
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c273c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c273c-118">Optional query parameters</span></span>
<span data-ttu-id="c273c-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c273c-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c273c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c273c-120">Request headers</span></span>
| <span data-ttu-id="c273c-121">名称</span><span class="sxs-lookup"><span data-stu-id="c273c-121">Name</span></span>      |<span data-ttu-id="c273c-122">说明</span><span class="sxs-lookup"><span data-stu-id="c273c-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="c273c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c273c-123">Authorization</span></span>  | <span data-ttu-id="c273c-124">负载.</span><span class="sxs-lookup"><span data-stu-id="c273c-124">Bearer.</span></span> <span data-ttu-id="c273c-125">必需</span><span class="sxs-lookup"><span data-stu-id="c273c-125">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="c273c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c273c-126">Request body</span></span>
<span data-ttu-id="c273c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c273c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c273c-128">响应</span><span class="sxs-lookup"><span data-stu-id="c273c-128">Response</span></span>

<span data-ttu-id="c273c-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[connectorGroup](../resources/connectorgroup.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="c273c-129">If successful, this method returns a `200 OK` response code and collection of [connectorGroup](../resources/connectorgroup.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c273c-130">示例</span><span class="sxs-lookup"><span data-stu-id="c273c-130">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c273c-131">请求</span><span class="sxs-lookup"><span data-stu-id="c273c-131">Request</span></span>

<span data-ttu-id="c273c-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c273c-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="c273c-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="c273c-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_connectorgroups"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups
```
# <a name="c"></a>[<span data-ttu-id="c273c-134">C#</span><span class="sxs-lookup"><span data-stu-id="c273c-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-connectorgroups-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c273c-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c273c-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-connectorgroups-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c273c-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c273c-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-connectorgroups-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="c273c-137">响应</span><span class="sxs-lookup"><span data-stu-id="c273c-137">Response</span></span>
<span data-ttu-id="c273c-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c273c-138">The following is an example of the response.</span></span> <span data-ttu-id="c273c-139">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c273c-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c273c-140">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c273c-140">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 164

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value",
      "connectorGroupType": "connectorGroupType-value",
      "isDefault": true,
      "region": "region-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List connectorGroups",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
