---
title: 添加到 connectorGroup 连接器
description: 使用此 API 向 connectorGroup 添加一个连接符。
ms.openlocfilehash: f5e7330dd5476daacda47a78400181ad3ebc0e2b
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043939"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="66cb0-103">添加到 connectorGroup 连接器</span><span class="sxs-lookup"><span data-stu-id="66cb0-103">Add connector to connectorGroup</span></span>

> <span data-ttu-id="66cb0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="66cb0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="66cb0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="66cb0-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="66cb0-106">使用此 API 向 connectorGroup 添加一个连接符。</span><span class="sxs-lookup"><span data-stu-id="66cb0-106">Use this API to add a connector to a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="66cb0-107">权限</span><span class="sxs-lookup"><span data-stu-id="66cb0-107">Permissions</span></span>
<span data-ttu-id="66cb0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="66cb0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="66cb0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="66cb0-110">Permission type</span></span>      | <span data-ttu-id="66cb0-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="66cb0-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="66cb0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="66cb0-112">Delegated (work or school account)</span></span> | <span data-ttu-id="66cb0-113">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="66cb0-113">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="66cb0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="66cb0-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="66cb0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="66cb0-115">Not supported.</span></span>    |
|<span data-ttu-id="66cb0-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="66cb0-116">Application</span></span> | <span data-ttu-id="66cb0-117">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="66cb0-117">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="66cb0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="66cb0-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="66cb0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="66cb0-119">Request headers</span></span>
| <span data-ttu-id="66cb0-120">名称</span><span class="sxs-lookup"><span data-stu-id="66cb0-120">Name</span></span>       | <span data-ttu-id="66cb0-121">说明</span><span class="sxs-lookup"><span data-stu-id="66cb0-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="66cb0-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="66cb0-122">Authorization</span></span>  | <span data-ttu-id="66cb0-123">持有者。</span><span class="sxs-lookup"><span data-stu-id="66cb0-123">Bearer.</span></span> <span data-ttu-id="66cb0-124">必需</span><span class="sxs-lookup"><span data-stu-id="66cb0-124">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="66cb0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="66cb0-125">Request body</span></span>
<span data-ttu-id="66cb0-126">在请求正文中，提供指向[连接器](../resources/connector.md)对象的链接的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66cb0-126">In the request body, supply a JSON representation of a link to a   [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="66cb0-127">响应</span><span class="sxs-lookup"><span data-stu-id="66cb0-127">Response</span></span>

<span data-ttu-id="66cb0-128">如果成功，此方法返回`201 Created`响应正文中的响应代码和[连接器](../resources/connector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="66cb0-128">If successful, this method returns `201 Created` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="66cb0-129">示例</span><span class="sxs-lookup"><span data-stu-id="66cb0-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="66cb0-130">请求</span><span class="sxs-lookup"><span data-stu-id="66cb0-130">Request</span></span>
<span data-ttu-id="66cb0-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="66cb0-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connector_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups/{id}/members/$ref
Content-type: application/json
Content-length: 104

{
  "@odata.id": "https://graph.microsoft.com/{ver}/connector/{id}"
}
```
<span data-ttu-id="66cb0-132">在请求正文中，提供指向[连接器](../resources/connector.md)对象的链接的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="66cb0-132">In the request body, supply a JSON representation of a link to a  [connector](../resources/connector.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="66cb0-133">响应</span><span class="sxs-lookup"><span data-stu-id="66cb0-133">Response</span></span>
<span data-ttu-id="66cb0-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="66cb0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
} -->
```http
HTTP/1.1 201 Created
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
<!-- {
  "type": "#page.annotation",
  "description": "Create connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
