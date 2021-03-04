---
title: 创建 privilegedApproval
description: 使用此 API 创建新的 privilegedApproval。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: ef3581fef523f14d5f84bb0f1859795860624c45
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50442241"
---
# <a name="create-privilegedapproval"></a><span data-ttu-id="fc3d0-103">创建 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="fc3d0-103">Create privilegedApproval</span></span>

<span data-ttu-id="fc3d0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fc3d0-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fc3d0-105">使用此 API 创建新的 privilegedApproval。</span><span class="sxs-lookup"><span data-stu-id="fc3d0-105">Use this API to create a new privilegedApproval.</span></span>
## <a name="permissions"></a><span data-ttu-id="fc3d0-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="fc3d0-106">Permissions</span></span>
<span data-ttu-id="fc3d0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc3d0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="fc3d0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc3d0-109">Permission type</span></span>      | <span data-ttu-id="fc3d0-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc3d0-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc3d0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc3d0-111">Delegated (work or school account)</span></span> | <span data-ttu-id="fc3d0-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fc3d0-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fc3d0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc3d0-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc3d0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc3d0-114">Not supported.</span></span>    |
|<span data-ttu-id="fc3d0-115">Application</span><span class="sxs-lookup"><span data-stu-id="fc3d0-115">Application</span></span> | <span data-ttu-id="fc3d0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc3d0-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc3d0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc3d0-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedApproval

```
## <a name="request-headers"></a><span data-ttu-id="fc3d0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc3d0-118">Request headers</span></span>
| <span data-ttu-id="fc3d0-119">名称</span><span class="sxs-lookup"><span data-stu-id="fc3d0-119">Name</span></span>       | <span data-ttu-id="fc3d0-120">说明</span><span class="sxs-lookup"><span data-stu-id="fc3d0-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="fc3d0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc3d0-121">Authorization</span></span>  | <span data-ttu-id="fc3d0-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fc3d0-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="fc3d0-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc3d0-124">Request body</span></span>
<span data-ttu-id="fc3d0-125">在请求正文中，提供 [privilegedApproval](../resources/privilegedapproval.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc3d0-125">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="fc3d0-126">响应</span><span class="sxs-lookup"><span data-stu-id="fc3d0-126">Response</span></span>

<span data-ttu-id="fc3d0-127">如果成功，此方法在响应正文中返回响应 `201 Created` 代码和 [privilegedApproval](../resources/privilegedapproval.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fc3d0-127">If successful, this method returns `201 Created` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="fc3d0-128">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="fc3d0-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="fc3d0-129">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="fc3d0-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="fc3d0-130">示例</span><span class="sxs-lookup"><span data-stu-id="fc3d0-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc3d0-131">请求</span><span class="sxs-lookup"><span data-stu-id="fc3d0-131">Request</span></span>
<span data-ttu-id="fc3d0-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc3d0-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="fc3d0-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="fc3d0-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_privilegedapproval_from_privilegedapproval"
}-->
```http
POST https://graph.microsoft.com/beta/privilegedApproval
Content-type: application/json
Content-length: 180

{
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```
# <a name="c"></a>[<span data-ttu-id="fc3d0-134">C#</span><span class="sxs-lookup"><span data-stu-id="fc3d0-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedapproval-from-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fc3d0-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fc3d0-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedapproval-from-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fc3d0-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fc3d0-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedapproval-from-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fc3d0-137">Java</span><span class="sxs-lookup"><span data-stu-id="fc3d0-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-privilegedapproval-from-privilegedapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="fc3d0-138">在请求正文中，提供 [privilegedApproval](../resources/privilegedapproval.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc3d0-138">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="fc3d0-139">响应</span><span class="sxs-lookup"><span data-stu-id="fc3d0-139">Response</span></span>
<span data-ttu-id="fc3d0-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fc3d0-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedApproval"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 200

{
  "id": "id-value",
  "userId": "userId-value",
  "roleId": "roleId-value",
  "approvalType": "approvalType-value",
  "approvalState": "approvalState-value",
  "approvalDuration": "datetime-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create privilegedApproval",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


