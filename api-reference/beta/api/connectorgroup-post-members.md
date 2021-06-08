---
title: Add connector to connectorGroup
description: 使用此 API 将连接器添加到 connectorGroup。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 83829bdcfc3c3bfafe92971c42420f2fb9cf62d8
ms.sourcegitcommit: 94c4acf8bd03c10a44b12952b6cb4827df55b978
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/06/2021
ms.locfileid: "52786143"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="28f46-103">Add connector to connectorGroup</span><span class="sxs-lookup"><span data-stu-id="28f46-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="28f46-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="28f46-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="28f46-105">将连接器 [添加到](../resources/connector.md) [connectorGroup](../resources/connectorgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="28f46-105">Add a [connector](../resources/connector.md) to a [connectorGroup](../resources/connectorgroup.md).</span></span>

<span data-ttu-id="28f46-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="28f46-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="28f46-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="28f46-108">Permission type</span></span>      | <span data-ttu-id="28f46-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="28f46-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="28f46-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="28f46-110">Delegated (work or school account)</span></span> | <span data-ttu-id="28f46-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="28f46-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="28f46-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="28f46-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="28f46-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="28f46-113">Not supported.</span></span>    |
|<span data-ttu-id="28f46-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="28f46-114">Application</span></span> | <span data-ttu-id="28f46-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="28f46-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="28f46-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="28f46-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="28f46-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="28f46-117">Request headers</span></span>
| <span data-ttu-id="28f46-118">名称</span><span class="sxs-lookup"><span data-stu-id="28f46-118">Name</span></span>       | <span data-ttu-id="28f46-119">说明</span><span class="sxs-lookup"><span data-stu-id="28f46-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="28f46-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="28f46-120">Authorization</span></span>  | <span data-ttu-id="28f46-121">Bearer。</span><span class="sxs-lookup"><span data-stu-id="28f46-121">Bearer.</span></span> <span data-ttu-id="28f46-122">必需。</span><span class="sxs-lookup"><span data-stu-id="28f46-122">Required.</span></span>|
| <span data-ttu-id="28f46-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="28f46-123">Content-type</span></span> | <span data-ttu-id="28f46-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="28f46-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="28f46-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="28f46-126">Request body</span></span>
<span data-ttu-id="28f46-127">在请求正文中，提供指向连接器对象的链接的 JSON [表示](../resources/connector.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="28f46-127">In the request body, supply a JSON representation of a link to a [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="28f46-128">响应</span><span class="sxs-lookup"><span data-stu-id="28f46-128">Response</span></span>

<span data-ttu-id="28f46-129">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [connector](../resources/connector.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="28f46-129">If successful, this method returns a `201 Created` response code and a [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="28f46-130">示例</span><span class="sxs-lookup"><span data-stu-id="28f46-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="28f46-131">请求</span><span class="sxs-lookup"><span data-stu-id="28f46-131">Request</span></span>
<span data-ttu-id="28f46-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="28f46-132">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="28f46-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="28f46-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_connector_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref
Content-type: application/json
Content-length: 104

{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="28f46-134">C#</span><span class="sxs-lookup"><span data-stu-id="28f46-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connector-from-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="28f46-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="28f46-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connector-from-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="28f46-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="28f46-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connector-from-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="28f46-137">Java</span><span class="sxs-lookup"><span data-stu-id="28f46-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-connector-from-connectorgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="28f46-138">响应</span><span class="sxs-lookup"><span data-stu-id="28f46-138">Response</span></span>
<span data-ttu-id="28f46-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="28f46-139">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Add connector to connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



