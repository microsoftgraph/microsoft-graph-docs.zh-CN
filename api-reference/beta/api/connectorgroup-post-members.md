---
title: 将连接器添加到 connectorGroup
description: 使用此 API 将连接器添加到 connectorGroup。
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: ad5efa59698d4dcf05365c63eb7f69fa2eb095a6
ms.sourcegitcommit: 1ec5a7be90790aaebdf6d85d93ab0c72b381c9c3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/24/2020
ms.locfileid: "44862925"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="c3d9a-103">将连接器添加到 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="c3d9a-103">Add connector to connectorGroup</span></span>

<span data-ttu-id="c3d9a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3d9a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c3d9a-105">将[连接器](../resources/connector.md)添加到[connectorGroup](../resources/connectorgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="c3d9a-105">Add a [connector](../resources/connector.md) to a [connectorGroup](../resources/connectorgroup.md).</span></span>

<span data-ttu-id="c3d9a-106">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c3d9a-106">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c3d9a-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c3d9a-107">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3d9a-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3d9a-108">Permission type</span></span>      | <span data-ttu-id="c3d9a-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c3d9a-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c3d9a-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3d9a-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c3d9a-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c3d9a-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c3d9a-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3d9a-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c3d9a-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3d9a-113">Not supported.</span></span>    |
|<span data-ttu-id="c3d9a-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c3d9a-114">Application</span></span> | <span data-ttu-id="c3d9a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3d9a-115">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="c3d9a-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3d9a-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/members/$ref

```
## <a name="request-headers"></a><span data-ttu-id="c3d9a-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3d9a-117">Request headers</span></span>
| <span data-ttu-id="c3d9a-118">名称</span><span class="sxs-lookup"><span data-stu-id="c3d9a-118">Name</span></span>       | <span data-ttu-id="c3d9a-119">说明</span><span class="sxs-lookup"><span data-stu-id="c3d9a-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c3d9a-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3d9a-120">Authorization</span></span>  | <span data-ttu-id="c3d9a-121">负载.</span><span class="sxs-lookup"><span data-stu-id="c3d9a-121">Bearer.</span></span> <span data-ttu-id="c3d9a-122">必需。</span><span class="sxs-lookup"><span data-stu-id="c3d9a-122">Required.</span></span>|
| <span data-ttu-id="c3d9a-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="c3d9a-123">Content-type</span></span> | <span data-ttu-id="c3d9a-124">application/json.</span><span class="sxs-lookup"><span data-stu-id="c3d9a-124">application/json.</span></span> <span data-ttu-id="c3d9a-125">Required.</span><span class="sxs-lookup"><span data-stu-id="c3d9a-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c3d9a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3d9a-126">Request body</span></span>
<span data-ttu-id="c3d9a-127">在请求正文中，提供指向[连接器](../resources/connector.md)对象的链接的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3d9a-127">In the request body, supply a JSON representation of a link to a [connector](../resources/connector.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c3d9a-128">响应</span><span class="sxs-lookup"><span data-stu-id="c3d9a-128">Response</span></span>

<span data-ttu-id="c3d9a-129">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[连接器](../resources/connector.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c3d9a-129">If successful, this method returns a `201 Created` response code and a [connector](../resources/connector.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3d9a-130">示例</span><span class="sxs-lookup"><span data-stu-id="c3d9a-130">Example</span></span>
### <a name="request"></a><span data-ttu-id="c3d9a-131">请求</span><span class="sxs-lookup"><span data-stu-id="c3d9a-131">Request</span></span>
<span data-ttu-id="c3d9a-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c3d9a-132">The following is an example of the request.</span></span>
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
### <a name="response"></a><span data-ttu-id="c3d9a-133">响应</span><span class="sxs-lookup"><span data-stu-id="c3d9a-133">Response</span></span>
<span data-ttu-id="c3d9a-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c3d9a-134">The following is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connector"
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
