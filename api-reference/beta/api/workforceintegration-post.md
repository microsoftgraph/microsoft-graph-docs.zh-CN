---
title: 创建 workforceIntegration
description: 创建新的 workforceIntegration 对象。
localization_priority: Normal
author: akumar39
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 6066005ff12e2cfa3513f1548b4e3895eb38f993
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40870574"
---
# <a name="create-workforceintegration"></a><span data-ttu-id="5b105-103">创建 workforceIntegration</span><span class="sxs-lookup"><span data-stu-id="5b105-103">Create workforceIntegration</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5b105-104">创建新的[workforceIntegration](../resources/workforceintegration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5b105-104">Create a new [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="5b105-105">权限</span><span class="sxs-lookup"><span data-stu-id="5b105-105">Permissions</span></span>

<span data-ttu-id="5b105-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5b105-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5b105-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b105-108">Permission type</span></span>                        | <span data-ttu-id="5b105-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5b105-109">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5b105-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b105-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="5b105-111">WorkforceIntegration</span><span class="sxs-lookup"><span data-stu-id="5b105-111">WorkforceIntegration.ReadWrite.All</span></span> |
| <span data-ttu-id="5b105-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b105-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5b105-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b105-113">Not supported.</span></span> |
| <span data-ttu-id="5b105-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b105-114">Application</span></span>                            | <span data-ttu-id="5b105-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b105-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="5b105-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b105-116">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
POST /teamwork/workforceIntegrations
```

## <a name="request-headers"></a><span data-ttu-id="5b105-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b105-117">Request headers</span></span>

| <span data-ttu-id="5b105-118">名称</span><span class="sxs-lookup"><span data-stu-id="5b105-118">Name</span></span>          | <span data-ttu-id="5b105-119">说明</span><span class="sxs-lookup"><span data-stu-id="5b105-119">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="5b105-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b105-120">Authorization</span></span> | <span data-ttu-id="5b105-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5b105-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5b105-123">Content-type</span><span class="sxs-lookup"><span data-stu-id="5b105-123">Content-type</span></span> | <span data-ttu-id="5b105-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5b105-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5b105-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b105-126">Request body</span></span>

<span data-ttu-id="5b105-127">在请求正文中，提供[workforceIntegration](../resources/workforceintegration.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b105-127">In the request body, supply a JSON representation of a [workforceIntegration](../resources/workforceintegration.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="5b105-128">响应</span><span class="sxs-lookup"><span data-stu-id="5b105-128">Response</span></span>

<span data-ttu-id="5b105-129">如果成功，此方法在响应`201 Created`正文中返回响应代码和新的[workforceIntegration](../resources/workforceintegration.md)对象。</span><span class="sxs-lookup"><span data-stu-id="5b105-129">If successful, this method returns a `201 Created` response code and a new [workforceIntegration](../resources/workforceintegration.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5b105-130">示例</span><span class="sxs-lookup"><span data-stu-id="5b105-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5b105-131">请求</span><span class="sxs-lookup"><span data-stu-id="5b105-131">Request</span></span>

<span data-ttu-id="5b105-132">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="5b105-132">The following is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="5b105-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="5b105-133">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="5b105-134">C#</span><span class="sxs-lookup"><span data-stu-id="5b105-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-workforceintegration-from-teamwork-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="5b105-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5b105-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-workforceintegration-from-teamwork-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="5b105-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5b105-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-workforceintegration-from-teamwork-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5b105-137">响应</span><span class="sxs-lookup"><span data-stu-id="5b105-137">Response</span></span>

<span data-ttu-id="5b105-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5b105-138">The following is an example of the response.</span></span>

> <span data-ttu-id="5b105-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5b105-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
