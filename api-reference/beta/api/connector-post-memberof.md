---
title: 将连接器添加到 connectorGroup
description: 使用此 API 将连接器添加到新的 connectorGroup。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 00f2ada7d46831b6b0bfbae0db4174e3ca2e9c90
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48009077"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="fd440-103">Add connector to connectorGroup</span><span class="sxs-lookup"><span data-stu-id="fd440-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="fd440-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fd440-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fd440-105">将 [连接器](../resources/connector.md)  添加到 [connectorGroup](../resources/connectorgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="fd440-105">Add a [connector](../resources/connector.md)  to a [connectorGroup](../resources/connectorgroup.md).</span></span>
## <a name="permissions"></a><span data-ttu-id="fd440-106">权限</span><span class="sxs-lookup"><span data-stu-id="fd440-106">Permissions</span></span>
<span data-ttu-id="fd440-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fd440-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd440-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd440-109">Permission type</span></span>      | <span data-ttu-id="fd440-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fd440-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fd440-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd440-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fd440-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fd440-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fd440-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd440-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fd440-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd440-114">Not supported.</span></span>    |
|<span data-ttu-id="fd440-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd440-115">Application</span></span> | <span data-ttu-id="fd440-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd440-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="fd440-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd440-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectors/{id}/memberOf/$ref

```
## <a name="request-headers"></a><span data-ttu-id="fd440-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd440-118">Request headers</span></span>
| <span data-ttu-id="fd440-119">名称</span><span class="sxs-lookup"><span data-stu-id="fd440-119">Name</span></span>       | <span data-ttu-id="fd440-120">说明</span><span class="sxs-lookup"><span data-stu-id="fd440-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fd440-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd440-121">Authorization</span></span>  | <span data-ttu-id="fd440-122">负载.</span><span class="sxs-lookup"><span data-stu-id="fd440-122">Bearer.</span></span> <span data-ttu-id="fd440-123">必填</span><span class="sxs-lookup"><span data-stu-id="fd440-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd440-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd440-124">Request body</span></span>
<span data-ttu-id="fd440-125">在请求正文中，提供 [connectorGroup](../resources/connectorgroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd440-125">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fd440-126">响应</span><span class="sxs-lookup"><span data-stu-id="fd440-126">Response</span></span>

<span data-ttu-id="fd440-127">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [connectorGroup](../resources/connectorgroup.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fd440-127">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd440-128">示例</span><span class="sxs-lookup"><span data-stu-id="fd440-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fd440-129">请求</span><span class="sxs-lookup"><span data-stu-id="fd440-129">Request</span></span>
<span data-ttu-id="fd440-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fd440-130">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fd440-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="fd440-131">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="fd440-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fd440-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-connectorgroup-from-connector-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="fd440-133">在请求正文中，提供 [connectorGroup](../resources/connectorgroup.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fd440-133">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fd440-134">响应</span><span class="sxs-lookup"><span data-stu-id="fd440-134">Response</span></span>
<span data-ttu-id="fd440-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fd440-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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


