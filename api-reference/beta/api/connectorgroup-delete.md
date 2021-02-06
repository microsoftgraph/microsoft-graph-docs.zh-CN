---
title: Delete connectorGroup
description: 删除 connectorGroup。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: d5ad43b789dff0abdc7cf938746e3b75dc5f4ad4
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50130134"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="51d6a-103">Delete connectorGroup</span><span class="sxs-lookup"><span data-stu-id="51d6a-103">Delete connectorGroup</span></span>

<span data-ttu-id="51d6a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="51d6a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="51d6a-105">删除 [connectorGroup](../resources/connectorgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="51d6a-105">Delete a [connectorGroup](../resources/connectorgroup.md).</span></span> <span data-ttu-id="51d6a-106">必须先 [从连接器](../resources/connector.md) 组中删除所有连接器和应用程序，然后才能删除连接器组。</span><span class="sxs-lookup"><span data-stu-id="51d6a-106">All [connectors](../resources/connector.md) and applications must be removed from the connector group before a connector group can be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="51d6a-107">权限</span><span class="sxs-lookup"><span data-stu-id="51d6a-107">Permissions</span></span>
<span data-ttu-id="51d6a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="51d6a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="51d6a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="51d6a-110">Permission type</span></span>      | <span data-ttu-id="51d6a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="51d6a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="51d6a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="51d6a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="51d6a-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="51d6a-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="51d6a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="51d6a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="51d6a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="51d6a-115">Not supported.</span></span>    |
|<span data-ttu-id="51d6a-116">Application</span><span class="sxs-lookup"><span data-stu-id="51d6a-116">Application</span></span> | <span data-ttu-id="51d6a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="51d6a-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="51d6a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="51d6a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="51d6a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="51d6a-119">Request headers</span></span>
| <span data-ttu-id="51d6a-120">名称</span><span class="sxs-lookup"><span data-stu-id="51d6a-120">Name</span></span>       | <span data-ttu-id="51d6a-121">说明</span><span class="sxs-lookup"><span data-stu-id="51d6a-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="51d6a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="51d6a-122">Authorization</span></span>  | <span data-ttu-id="51d6a-123">Bearer。</span><span class="sxs-lookup"><span data-stu-id="51d6a-123">Bearer.</span></span> <span data-ttu-id="51d6a-124">必需</span><span class="sxs-lookup"><span data-stu-id="51d6a-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="51d6a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="51d6a-125">Request body</span></span>
<span data-ttu-id="51d6a-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="51d6a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="51d6a-127">响应</span><span class="sxs-lookup"><span data-stu-id="51d6a-127">Response</span></span>

<span data-ttu-id="51d6a-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="51d6a-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51d6a-130">示例</span><span class="sxs-lookup"><span data-stu-id="51d6a-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="51d6a-131">请求</span><span class="sxs-lookup"><span data-stu-id="51d6a-131">Request</span></span>
<span data-ttu-id="51d6a-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="51d6a-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="51d6a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="51d6a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="51d6a-134">C#</span><span class="sxs-lookup"><span data-stu-id="51d6a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="51d6a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="51d6a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="51d6a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="51d6a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="51d6a-137">Java</span><span class="sxs-lookup"><span data-stu-id="51d6a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-connectorgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="51d6a-138">响应</span><span class="sxs-lookup"><span data-stu-id="51d6a-138">Response</span></span>
<span data-ttu-id="51d6a-139">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="51d6a-139">The following is an example of the response.</span></span> <span data-ttu-id="51d6a-140">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="51d6a-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="51d6a-141">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="51d6a-141">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



