---
title: 将连接器添加到 connectorGroup
description: 使用此 API 将连接器添加到新的 connectorGroup。
localization_priority: Normal
author: japere
ms.prod: applications
doc_type: apiPageType
ms.openlocfilehash: 2b3f2b5cd8813455d6a072fcdd8fecc05974d548
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52047194"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="71b4a-103">Add connector to connectorGroup</span><span class="sxs-lookup"><span data-stu-id="71b4a-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="71b4a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71b4a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="71b4a-105">将连接器 [添加到](../resources/connector.md) [connectorGroup](../resources/connectorgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="71b4a-105">Add a [connector](../resources/connector.md)  to a [connectorGroup](../resources/connectorgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="71b4a-106">权限</span><span class="sxs-lookup"><span data-stu-id="71b4a-106">Permissions</span></span>
<span data-ttu-id="71b4a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71b4a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71b4a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="71b4a-109">Permission type</span></span>      | <span data-ttu-id="71b4a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71b4a-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="71b4a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71b4a-111">Delegated (work or school account)</span></span> | <span data-ttu-id="71b4a-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="71b4a-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="71b4a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71b4a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="71b4a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="71b4a-114">Not supported.</span></span>    |
|<span data-ttu-id="71b4a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="71b4a-115">Application</span></span> | <span data-ttu-id="71b4a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="71b4a-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="71b4a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71b4a-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf/$ref

```
## <a name="request-headers"></a><span data-ttu-id="71b4a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="71b4a-118">Request headers</span></span>
| <span data-ttu-id="71b4a-119">名称</span><span class="sxs-lookup"><span data-stu-id="71b4a-119">Name</span></span>       | <span data-ttu-id="71b4a-120">说明</span><span class="sxs-lookup"><span data-stu-id="71b4a-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="71b4a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="71b4a-121">Authorization</span></span>  | <span data-ttu-id="71b4a-122">Bearer。</span><span class="sxs-lookup"><span data-stu-id="71b4a-122">Bearer.</span></span> <span data-ttu-id="71b4a-123">必需</span><span class="sxs-lookup"><span data-stu-id="71b4a-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="71b4a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="71b4a-124">Request body</span></span>
<span data-ttu-id="71b4a-125">在请求正文中，提供 [connectorGroup](../resources/connectorgroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71b4a-125">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="71b4a-126">响应</span><span class="sxs-lookup"><span data-stu-id="71b4a-126">Response</span></span>

<span data-ttu-id="71b4a-127">如果成功，此方法在 `201 Created` 响应正文中返回 响应代码和 [connectorGroup](../resources/connectorgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="71b4a-127">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71b4a-128">示例</span><span class="sxs-lookup"><span data-stu-id="71b4a-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="71b4a-129">请求</span><span class="sxs-lookup"><span data-stu-id="71b4a-129">Request</span></span>
<span data-ttu-id="71b4a-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71b4a-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="71b4a-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="71b4a-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_connectorgroup_from_connector"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf/$ref
Content-type: application/json
Content-length: 99

{
  "@odata.id": "https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}"
}
```
# <a name="javascript"></a>[<span data-ttu-id="71b4a-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="71b4a-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connectorgroup-from-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="71b4a-133">C#</span><span class="sxs-lookup"><span data-stu-id="71b4a-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-connectorgroup-from-connector-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="71b4a-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="71b4a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-connectorgroup-from-connector-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="71b4a-135">Java</span><span class="sxs-lookup"><span data-stu-id="71b4a-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-connectorgroup-from-connector-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="71b4a-136">在请求正文中，提供 [connectorGroup](../resources/connectorgroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71b4a-136">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="71b4a-137">响应</span><span class="sxs-lookup"><span data-stu-id="71b4a-137">Response</span></span>
<span data-ttu-id="71b4a-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="71b4a-138">Here is an example of the response.</span></span> <span data-ttu-id="71b4a-139">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="71b4a-139">Note: The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 201 Created
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
  "description": "Create connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->



