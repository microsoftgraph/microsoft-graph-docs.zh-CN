---
title: 将 connectorGroup 分配给应用程序
description: 使用此 API 将 connectorGroup 分配给应用程序
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 467320f0118743a29415a035421c4a92496aaf38
ms.sourcegitcommit: a1675c7b8dfc7d7c3c7923d06cda2b0127f9c3e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/05/2021
ms.locfileid: "49752840"
---
# <a name="assign-a-connectorgroup-to-an-application"></a><span data-ttu-id="6ec18-103">将 connectorGroup 分配给应用程序</span><span class="sxs-lookup"><span data-stu-id="6ec18-103">Assign a connectorGroup to an application</span></span>

<span data-ttu-id="6ec18-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6ec18-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6ec18-105">将 [connectorGroup](../resources/connectorgroup.md) 分配给 [应用程序](../resources/application.md)。</span><span class="sxs-lookup"><span data-stu-id="6ec18-105">Assign a [connectorGroup](../resources/connectorgroup.md) to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="6ec18-106">权限</span><span class="sxs-lookup"><span data-stu-id="6ec18-106">Permissions</span></span>
<span data-ttu-id="6ec18-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6ec18-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6ec18-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6ec18-109">Permission type</span></span>      | <span data-ttu-id="6ec18-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6ec18-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6ec18-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6ec18-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6ec18-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6ec18-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6ec18-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6ec18-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6ec18-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ec18-114">Not supported.</span></span>    |
|<span data-ttu-id="6ec18-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6ec18-115">Application</span></span> | <span data-ttu-id="6ec18-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6ec18-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="6ec18-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6ec18-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /applications/{id}/connectorGroup/$ref

```
## <a name="request-headers"></a><span data-ttu-id="6ec18-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6ec18-118">Request headers</span></span>
| <span data-ttu-id="6ec18-119">名称</span><span class="sxs-lookup"><span data-stu-id="6ec18-119">Name</span></span>       | <span data-ttu-id="6ec18-120">说明</span><span class="sxs-lookup"><span data-stu-id="6ec18-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="6ec18-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6ec18-121">Authorization</span></span>  | <span data-ttu-id="6ec18-122">Bearer。</span><span class="sxs-lookup"><span data-stu-id="6ec18-122">Bearer.</span></span> <span data-ttu-id="6ec18-123">必需。</span><span class="sxs-lookup"><span data-stu-id="6ec18-123">Required.</span></span>|
| <span data-ttu-id="6ec18-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="6ec18-124">Content-type</span></span> | <span data-ttu-id="6ec18-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="6ec18-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6ec18-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6ec18-127">Request body</span></span>
<span data-ttu-id="6ec18-128">在请求正文中，提供 [connectorGroup](../resources/connectorgroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6ec18-128">In the request body, supply a JSON representation of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="6ec18-129">响应</span><span class="sxs-lookup"><span data-stu-id="6ec18-129">Response</span></span>

<span data-ttu-id="6ec18-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [application](../resources/application.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6ec18-130">If successful, this method returns `201 Created` response code and an [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6ec18-131">示例</span><span class="sxs-lookup"><span data-stu-id="6ec18-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="6ec18-132">请求</span><span class="sxs-lookup"><span data-stu-id="6ec18-132">Request</span></span>
<span data-ttu-id="6ec18-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="6ec18-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="6ec18-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="6ec18-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_application_from_connectorgroup"
}-->
```http
PUT https://graph.microsoft.com/beta/applications/{id}/connectorGroup/$ref
Content-type: application/json
Content-length: 30

{
  "@odata.id": "https://graph.microsoft.com/onPremisesPublishingProfiles/applicationproxy/connectorGroups/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="6ec18-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="6ec18-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="6ec18-136">C#</span><span class="sxs-lookup"><span data-stu-id="6ec18-136">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-application-from-connectorgroup-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="6ec18-137">Objective-C</span><span class="sxs-lookup"><span data-stu-id="6ec18-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-application-from-connectorgroup-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="6ec18-138">Java</span><span class="sxs-lookup"><span data-stu-id="6ec18-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-application-from-connectorgroup-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="6ec18-139">响应</span><span class="sxs-lookup"><span data-stu-id="6ec18-139">Response</span></span>
<span data-ttu-id="6ec18-140">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="6ec18-140">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 204 No content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Assign a connectorGroup to an application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


