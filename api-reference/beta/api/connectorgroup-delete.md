---
title: 删除 connectorGroup
description: 删除 connectorGroup。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 12fe7ee89d5175b7a0be6721775c42c16a7eb51d
ms.sourcegitcommit: c650b95ef4d0c3e93e2eb36cd6b52ed31200164f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/10/2020
ms.locfileid: "44681467"
---
# <a name="delete-connectorgroup"></a><span data-ttu-id="63eca-103">删除 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="63eca-103">Delete connectorGroup</span></span>

<span data-ttu-id="63eca-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="63eca-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="63eca-105">删除[connectorGroup](../resources/connectorgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="63eca-105">Delete a [connectorGroup](../resources/connectorgroup.md).</span></span> <span data-ttu-id="63eca-106">必须先从连接器组中删除所有[连接器](../resources/connector.md)和应用程序，然后才能删除连接器组。</span><span class="sxs-lookup"><span data-stu-id="63eca-106">All [connectors](../resources/connector.md) and applications must be removed from the connector group before a connector group can be deleted.</span></span>

## <a name="permissions"></a><span data-ttu-id="63eca-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="63eca-107">Permissions</span></span>
<span data-ttu-id="63eca-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="63eca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="63eca-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="63eca-110">Permission type</span></span>      | <span data-ttu-id="63eca-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="63eca-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="63eca-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="63eca-112">Delegated (work or school account)</span></span> | <span data-ttu-id="63eca-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="63eca-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="63eca-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="63eca-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="63eca-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="63eca-115">Not supported.</span></span>    |
|<span data-ttu-id="63eca-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="63eca-116">Application</span></span> | <span data-ttu-id="63eca-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="63eca-117">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="63eca-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="63eca-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
## <a name="request-headers"></a><span data-ttu-id="63eca-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="63eca-119">Request headers</span></span>
| <span data-ttu-id="63eca-120">名称</span><span class="sxs-lookup"><span data-stu-id="63eca-120">Name</span></span>       | <span data-ttu-id="63eca-121">说明</span><span class="sxs-lookup"><span data-stu-id="63eca-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="63eca-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="63eca-122">Authorization</span></span>  | <span data-ttu-id="63eca-123">负载.</span><span class="sxs-lookup"><span data-stu-id="63eca-123">Bearer.</span></span> <span data-ttu-id="63eca-124">必需</span><span class="sxs-lookup"><span data-stu-id="63eca-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="63eca-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="63eca-125">Request body</span></span>
<span data-ttu-id="63eca-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="63eca-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="63eca-127">响应</span><span class="sxs-lookup"><span data-stu-id="63eca-127">Response</span></span>

<span data-ttu-id="63eca-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="63eca-p104">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="63eca-130">示例</span><span class="sxs-lookup"><span data-stu-id="63eca-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="63eca-131">请求</span><span class="sxs-lookup"><span data-stu-id="63eca-131">Request</span></span>
<span data-ttu-id="63eca-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="63eca-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="63eca-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="63eca-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_connectorgroup"
}-->
```http
DELETE https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}
```
# <a name="c"></a>[<span data-ttu-id="63eca-134">C#</span><span class="sxs-lookup"><span data-stu-id="63eca-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="63eca-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="63eca-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="63eca-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="63eca-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="63eca-137">响应</span><span class="sxs-lookup"><span data-stu-id="63eca-137">Response</span></span>
<span data-ttu-id="63eca-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="63eca-138">The following is an example of the response.</span></span> <span data-ttu-id="63eca-139">注意：为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="63eca-139">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="63eca-140">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="63eca-140">All of the properties will be returned from an actual call.</span></span>
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
