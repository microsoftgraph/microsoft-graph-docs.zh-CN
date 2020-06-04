---
title: 将连接器添加到 connectorGroup
description: 使用此 API 将连接器添加到 connectorGroup。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: de3f64a0b1efec39497d2b6e4a24bc690539fe75
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44555788"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="91c69-103">将连接器添加到 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="91c69-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="91c69-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="91c69-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="91c69-105">将[连接器](../resources/connector.md)添加到[connectorGroup](../resources/connectorgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="91c69-105">Add a [connector](../resources/connector.md) to a [connectorGroup](../resources/connectorgroup.md).</span></span>

<span data-ttu-id="91c69-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="91c69-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="91c69-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="91c69-108">Permission type</span></span>      | <span data-ttu-id="91c69-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="91c69-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="91c69-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="91c69-110">Delegated (work or school account)</span></span> | <span data-ttu-id="91c69-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="91c69-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="91c69-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="91c69-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="91c69-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="91c69-113">Not supported.</span></span>    |
|<span data-ttu-id="91c69-114">Application</span><span class="sxs-lookup"><span data-stu-id="91c69-114">Application</span></span> | <span data-ttu-id="91c69-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="91c69-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="91c69-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="91c69-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="91c69-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="91c69-117">Request headers</span></span>
| <span data-ttu-id="91c69-118">名称</span><span class="sxs-lookup"><span data-stu-id="91c69-118">Name</span></span>       | <span data-ttu-id="91c69-119">说明</span><span class="sxs-lookup"><span data-stu-id="91c69-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="91c69-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="91c69-120">Authorization</span></span>  | <span data-ttu-id="91c69-121">负载.</span><span class="sxs-lookup"><span data-stu-id="91c69-121">Bearer.</span></span> <span data-ttu-id="91c69-122">必需</span><span class="sxs-lookup"><span data-stu-id="91c69-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="91c69-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="91c69-123">Request body</span></span>
<span data-ttu-id="91c69-124">在请求正文中，提供指向[连接器](../resources/connector.md)对象的链接的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91c69-124">In the request body, supply a JSON representation of a link to a   [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="91c69-125">响应</span><span class="sxs-lookup"><span data-stu-id="91c69-125">Response</span></span>

<span data-ttu-id="91c69-126">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[连接器](../resources/connector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="91c69-126">If successful, this method returns `201 Created` response code and [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="91c69-127">示例</span><span class="sxs-lookup"><span data-stu-id="91c69-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="91c69-128">请求</span><span class="sxs-lookup"><span data-stu-id="91c69-128">Request</span></span>
<span data-ttu-id="91c69-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="91c69-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="91c69-130">在请求正文中，提供指向[连接器](../resources/connector.md)对象的链接的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="91c69-130">In the request body, supply a JSON representation of a link to a  [connector](../resources/connector.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="91c69-131">响应</span><span class="sxs-lookup"><span data-stu-id="91c69-131">Response</span></span>
<span data-ttu-id="91c69-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="91c69-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
