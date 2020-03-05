---
title: 将连接器添加到 connectorGroup
description: 使用此 API 将连接器添加到 connectorGroup。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: dce30f90f35bb373be845aaa9390c9da8c54d02f
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437180"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="a08ab-103">将连接器添加到 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="a08ab-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="a08ab-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="a08ab-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a08ab-105">使用此 API 将连接器添加到 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="a08ab-105">Use this API to add a connector to a connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="a08ab-106">权限</span><span class="sxs-lookup"><span data-stu-id="a08ab-106">Permissions</span></span>
<span data-ttu-id="a08ab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a08ab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a08ab-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a08ab-109">Permission type</span></span>      | <span data-ttu-id="a08ab-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a08ab-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a08ab-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a08ab-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a08ab-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="a08ab-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="a08ab-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a08ab-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a08ab-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a08ab-114">Not supported.</span></span>    |
|<span data-ttu-id="a08ab-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a08ab-115">Application</span></span> | <span data-ttu-id="a08ab-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a08ab-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a08ab-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a08ab-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/members/$ref
```
## <a name="request-headers"></a><span data-ttu-id="a08ab-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a08ab-118">Request headers</span></span>
| <span data-ttu-id="a08ab-119">名称</span><span class="sxs-lookup"><span data-stu-id="a08ab-119">Name</span></span>       | <span data-ttu-id="a08ab-120">说明</span><span class="sxs-lookup"><span data-stu-id="a08ab-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="a08ab-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a08ab-121">Authorization</span></span>  | <span data-ttu-id="a08ab-122">负载.</span><span class="sxs-lookup"><span data-stu-id="a08ab-122">Bearer.</span></span> <span data-ttu-id="a08ab-123">必需</span><span class="sxs-lookup"><span data-stu-id="a08ab-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="a08ab-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="a08ab-124">Request body</span></span>
<span data-ttu-id="a08ab-125">在请求正文中，提供指向[连接器](../resources/connector.md)对象的链接的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a08ab-125">In the request body, supply a JSON representation of a link to a   [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="a08ab-126">响应</span><span class="sxs-lookup"><span data-stu-id="a08ab-126">Response</span></span>

<span data-ttu-id="a08ab-127">如果成功，此方法在`201 Created`响应正文中返回响应代码和[连接器](../resources/connector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a08ab-127">If successful, this method returns `201 Created` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a08ab-128">示例</span><span class="sxs-lookup"><span data-stu-id="a08ab-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a08ab-129">请求</span><span class="sxs-lookup"><span data-stu-id="a08ab-129">Request</span></span>
<span data-ttu-id="a08ab-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a08ab-130">Here is an example of the request.</span></span>
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
<span data-ttu-id="a08ab-131">在请求正文中，提供指向[连接器](../resources/connector.md)对象的链接的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a08ab-131">In the request body, supply a JSON representation of a link to a  [connector](../resources/connector.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="a08ab-132">响应</span><span class="sxs-lookup"><span data-stu-id="a08ab-132">Response</span></span>
<span data-ttu-id="a08ab-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a08ab-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "Create connector",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
