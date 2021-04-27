---
title: 创建 privilegedApproval
description: 使用此 API 创建新的 privilegedApproval。
localization_priority: Normal
doc_type: apiPageType
ms.prod: governance
author: shauliu
ms.openlocfilehash: 3b85324bc8468f0fd6c3c5963ab417ba8c6a9acb
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52055286"
---
# <a name="create-privilegedapproval"></a><span data-ttu-id="1a756-103">创建 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="1a756-103">Create privilegedApproval</span></span>

<span data-ttu-id="1a756-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a756-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a756-105">使用此 API 创建新的 privilegedApproval。</span><span class="sxs-lookup"><span data-stu-id="1a756-105">Use this API to create a new privilegedApproval.</span></span>
## <a name="permissions"></a><span data-ttu-id="1a756-106">权限</span><span class="sxs-lookup"><span data-stu-id="1a756-106">Permissions</span></span>
<span data-ttu-id="1a756-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a756-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="1a756-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a756-109">Permission type</span></span>      | <span data-ttu-id="1a756-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a756-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a756-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a756-111">Delegated (work or school account)</span></span> | <span data-ttu-id="1a756-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1a756-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1a756-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a756-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a756-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a756-114">Not supported.</span></span>    |
|<span data-ttu-id="1a756-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a756-115">Application</span></span> | <span data-ttu-id="1a756-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a756-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a756-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a756-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedApproval

```
## <a name="request-headers"></a><span data-ttu-id="1a756-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a756-118">Request headers</span></span>
| <span data-ttu-id="1a756-119">名称</span><span class="sxs-lookup"><span data-stu-id="1a756-119">Name</span></span>       | <span data-ttu-id="1a756-120">说明</span><span class="sxs-lookup"><span data-stu-id="1a756-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="1a756-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a756-121">Authorization</span></span>  | <span data-ttu-id="1a756-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a756-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1a756-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a756-124">Request body</span></span>
<span data-ttu-id="1a756-125">在请求正文中，提供 [privilegedApproval 对象的](../resources/privilegedapproval.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a756-125">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="1a756-126">响应</span><span class="sxs-lookup"><span data-stu-id="1a756-126">Response</span></span>

<span data-ttu-id="1a756-127">如果成功，此方法在 `201 Created` 响应正文中返回 响应代码和 [privilegedApproval](../resources/privilegedapproval.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a756-127">If successful, this method returns `201 Created` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="1a756-128">请注意，租户需要注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="1a756-128">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="1a756-129">否则，将返回 HTTP 403 禁止状态代码。</span><span class="sxs-lookup"><span data-stu-id="1a756-129">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="1a756-130">示例</span><span class="sxs-lookup"><span data-stu-id="1a756-130">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a756-131">请求</span><span class="sxs-lookup"><span data-stu-id="1a756-131">Request</span></span>
<span data-ttu-id="1a756-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a756-132">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="1a756-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1a756-133">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1a756-134">C#</span><span class="sxs-lookup"><span data-stu-id="1a756-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedapproval-from-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1a756-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1a756-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedapproval-from-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1a756-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1a756-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedapproval-from-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1a756-137">Java</span><span class="sxs-lookup"><span data-stu-id="1a756-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-privilegedapproval-from-privilegedapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="1a756-138">在请求正文中，提供 [privilegedApproval 对象的](../resources/privilegedapproval.md) JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a756-138">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="1a756-139">响应</span><span class="sxs-lookup"><span data-stu-id="1a756-139">Response</span></span>
<span data-ttu-id="1a756-140">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1a756-140">Here is an example of the response.</span></span> <span data-ttu-id="1a756-141">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1a756-141">Note: The response object shown here might be shortened for readability.</span></span>
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


