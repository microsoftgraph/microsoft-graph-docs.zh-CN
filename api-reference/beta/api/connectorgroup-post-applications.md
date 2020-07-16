---
title: 将 connectorGroup 分配给应用程序
description: 使用此 API 将 connectorGroup 分配给应用程序
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: a45037dc22298482001bb3f010aca538e4939ecd
ms.sourcegitcommit: e20c113409836115f338dcfe3162342ef3bd6a4a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/01/2020
ms.locfileid: "45006857"
---
# <a name="assign-a-connectorgroup-to-an-application"></a><span data-ttu-id="cc0ea-103">将 connectorGroup 分配给应用程序</span><span class="sxs-lookup"><span data-stu-id="cc0ea-103">Assign a connectorGroup to an application</span></span>

<span data-ttu-id="cc0ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cc0ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cc0ea-105">将[connectorGroup](../resources/connectorgroup.md)分配给[应用程序](../resources/application.md)。</span><span class="sxs-lookup"><span data-stu-id="cc0ea-105">Assign a [connectorGroup](../resources/connectorgroup.md) to an [application](../resources/application.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="cc0ea-106">权限</span><span class="sxs-lookup"><span data-stu-id="cc0ea-106">Permissions</span></span>
<span data-ttu-id="cc0ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cc0ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cc0ea-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cc0ea-109">Permission type</span></span>      | <span data-ttu-id="cc0ea-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cc0ea-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cc0ea-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cc0ea-111">Delegated (work or school account)</span></span> | <span data-ttu-id="cc0ea-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cc0ea-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cc0ea-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cc0ea-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cc0ea-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc0ea-114">Not supported.</span></span>    |
|<span data-ttu-id="cc0ea-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cc0ea-115">Application</span></span> | <span data-ttu-id="cc0ea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cc0ea-116">Not supported.</span></span>  |

## <a name="http-request"></a><span data-ttu-id="cc0ea-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cc0ea-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PUT /applications/{id}/connectorGroup/$ref

```
## <a name="request-headers"></a><span data-ttu-id="cc0ea-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cc0ea-118">Request headers</span></span>
| <span data-ttu-id="cc0ea-119">名称</span><span class="sxs-lookup"><span data-stu-id="cc0ea-119">Name</span></span>       | <span data-ttu-id="cc0ea-120">说明</span><span class="sxs-lookup"><span data-stu-id="cc0ea-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cc0ea-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cc0ea-121">Authorization</span></span>  | <span data-ttu-id="cc0ea-122">负载.</span><span class="sxs-lookup"><span data-stu-id="cc0ea-122">Bearer.</span></span> <span data-ttu-id="cc0ea-123">必需。</span><span class="sxs-lookup"><span data-stu-id="cc0ea-123">Required.</span></span>|
| <span data-ttu-id="cc0ea-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="cc0ea-124">Content-type</span></span> | <span data-ttu-id="cc0ea-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cc0ea-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cc0ea-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cc0ea-127">Request body</span></span>
<span data-ttu-id="cc0ea-128">在请求正文中，提供[connectorGroup](../resources/connectorgroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cc0ea-128">In the request body, supply a JSON representation of a [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cc0ea-129">响应</span><span class="sxs-lookup"><span data-stu-id="cc0ea-129">Response</span></span>

<span data-ttu-id="cc0ea-130">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [application](../resources/application.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cc0ea-130">If successful, this method returns `201 Created` response code and an [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cc0ea-131">示例</span><span class="sxs-lookup"><span data-stu-id="cc0ea-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="cc0ea-132">请求</span><span class="sxs-lookup"><span data-stu-id="cc0ea-132">Request</span></span>
<span data-ttu-id="cc0ea-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cc0ea-133">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="cc0ea-134">HTTP</span><span class="sxs-lookup"><span data-stu-id="cc0ea-134">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="cc0ea-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cc0ea-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-application-from-connectorgroup-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="cc0ea-136">响应</span><span class="sxs-lookup"><span data-stu-id="cc0ea-136">Response</span></span>
<span data-ttu-id="cc0ea-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cc0ea-137">The following is an example of the response.</span></span> 

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
