---
title: 创建 workforceIntegration
description: 创建新的 workforceIntegration 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: e6da06c27296009bcf337171af6e77d5cc55eeb0
ms.sourcegitcommit: 2ddc63c889fc2f4666aa55bca7ce0221ab899abf
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/07/2019
ms.locfileid: "39895574"
---
# <a name="create-workforceintegration"></a><span data-ttu-id="de7ea-103">创建 workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="de7ea-103">Create workforceIntegration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="de7ea-104">创建新的[workforceIntegration](../resources/workforceintegration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="de7ea-104">Create a new [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="de7ea-105">权限</span><span class="sxs-lookup"><span data-stu-id="de7ea-105">Permissions</span></span>

<span data-ttu-id="de7ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="de7ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="de7ea-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="de7ea-108">Permission type</span></span>                        | <span data-ttu-id="de7ea-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="de7ea-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="de7ea-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de7ea-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="de7ea-111">WorkforceIntegration</span><span class="sxs-lookup"><span data-stu-id="de7ea-111">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="de7ea-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de7ea-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="de7ea-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="de7ea-113">Not supported.</span></span> |
| <span data-ttu-id="de7ea-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="de7ea-114">Application</span></span>                            | <span data-ttu-id="de7ea-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="de7ea-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="de7ea-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de7ea-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="de7ea-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="de7ea-117">Request headers</span></span>

| <span data-ttu-id="de7ea-118">名称</span><span class="sxs-lookup"><span data-stu-id="de7ea-118">Name</span></span>          | <span data-ttu-id="de7ea-119">说明</span><span class="sxs-lookup"><span data-stu-id="de7ea-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="de7ea-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="de7ea-120">Authorization</span></span> | <span data-ttu-id="de7ea-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="de7ea-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="de7ea-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="de7ea-123">Content-type</span></span> | <span data-ttu-id="de7ea-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="de7ea-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="de7ea-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="de7ea-126">Request body</span></span>

<span data-ttu-id="de7ea-127">在请求正文中，提供[workforceIntegration](../resources/workforceintegration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de7ea-127">In the request body, supply a JSON representation of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="de7ea-128">响应</span><span class="sxs-lookup"><span data-stu-id="de7ea-128">Response</span></span>

<span data-ttu-id="de7ea-129">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[workforceIntegration](../resources/workforceintegration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="de7ea-129">If successful, this method returns a `201 Created` response code and a new [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="de7ea-130">示例</span><span class="sxs-lookup"><span data-stu-id="de7ea-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="de7ea-131">请求</span><span class="sxs-lookup"><span data-stu-id="de7ea-131">Request</span></span>

<span data-ttu-id="de7ea-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="de7ea-132">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_workforceintegration_from_teamwork"
}-->

```http
POST https://graph.microsoft.com/beta/teamwork/workforceIntegrations
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```

### <a name="response"></a><span data-ttu-id="de7ea-133">响应</span><span class="sxs-lookup"><span data-stu-id="de7ea-133">Response</span></span>

<span data-ttu-id="de7ea-134">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="de7ea-134">The following is an example of the response.</span></span>

> <span data-ttu-id="de7ea-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="de7ea-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.workforceIntegration"
} -->

```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "displayName": "displayName-value",
  "apiVersion": 99,
  "encryption": {
    "protocol": "protocol-value",
    "secret": "secret-value"
  },
  "isActive": true,
  "url": "url-value",
  "supports": "supports-value"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create workforceIntegration",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
