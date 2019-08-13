---
title: 创建 privilegedApproval
description: 使用此 API 创建新的 privilegedApproval。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 4b902bd05779a9dd6bb7cb771c2b91b14303e099
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36361250"
---
# <a name="create-privilegedapproval"></a><span data-ttu-id="cde70-103">创建 privilegedApproval</span><span class="sxs-lookup"><span data-stu-id="cde70-103">Create privilegedApproval</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cde70-104">使用此 API 创建新的 privilegedApproval。</span><span class="sxs-lookup"><span data-stu-id="cde70-104">Use this API to create a new privilegedApproval.</span></span>
## <a name="permissions"></a><span data-ttu-id="cde70-105">权限</span><span class="sxs-lookup"><span data-stu-id="cde70-105">Permissions</span></span>
<span data-ttu-id="cde70-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cde70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="cde70-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="cde70-108">Permission type</span></span>      | <span data-ttu-id="cde70-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cde70-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cde70-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cde70-110">Delegated (work or school account)</span></span> | <span data-ttu-id="cde70-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cde70-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cde70-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cde70-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cde70-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="cde70-113">Not supported.</span></span>    |
|<span data-ttu-id="cde70-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="cde70-114">Application</span></span> | <span data-ttu-id="cde70-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cde70-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="cde70-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cde70-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /privilegedApproval

```
## <a name="request-headers"></a><span data-ttu-id="cde70-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="cde70-117">Request headers</span></span>
| <span data-ttu-id="cde70-118">名称</span><span class="sxs-lookup"><span data-stu-id="cde70-118">Name</span></span>       | <span data-ttu-id="cde70-119">说明</span><span class="sxs-lookup"><span data-stu-id="cde70-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="cde70-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="cde70-120">Authorization</span></span>  | <span data-ttu-id="cde70-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cde70-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cde70-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="cde70-123">Request body</span></span>
<span data-ttu-id="cde70-124">在请求正文中, 提供[privilegedApproval](../resources/privilegedapproval.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cde70-124">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="cde70-125">响应</span><span class="sxs-lookup"><span data-stu-id="cde70-125">Response</span></span>

<span data-ttu-id="cde70-126">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[privilegedApproval](../resources/privilegedapproval.md)对象。</span><span class="sxs-lookup"><span data-stu-id="cde70-126">If successful, this method returns `201 Created` response code and [privilegedApproval](../resources/privilegedapproval.md) object in the response body.</span></span>

<span data-ttu-id="cde70-127">请注意, 需要将租户注册到 PIM。</span><span class="sxs-lookup"><span data-stu-id="cde70-127">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="cde70-128">否则, 将返回 HTTP 403 禁止的状态代码。</span><span class="sxs-lookup"><span data-stu-id="cde70-128">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>

## <a name="example"></a><span data-ttu-id="cde70-129">示例</span><span class="sxs-lookup"><span data-stu-id="cde70-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="cde70-130">请求</span><span class="sxs-lookup"><span data-stu-id="cde70-130">Request</span></span>
<span data-ttu-id="cde70-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cde70-131">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="cde70-132">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="cde70-132">HTTP</span></span>](#tab/http)
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
# <a name="ctabcsharp"></a>[<span data-ttu-id="cde70-133">C#</span><span class="sxs-lookup"><span data-stu-id="cde70-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-privilegedapproval-from-privilegedapproval-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cde70-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="cde70-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-privilegedapproval-from-privilegedapproval-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="cde70-135">目标-C</span><span class="sxs-lookup"><span data-stu-id="cde70-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-privilegedapproval-from-privilegedapproval-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="cde70-136">Java</span><span class="sxs-lookup"><span data-stu-id="cde70-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-privilegedapproval-from-privilegedapproval-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

<span data-ttu-id="cde70-137">在请求正文中, 提供[privilegedApproval](../resources/privilegedapproval.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cde70-137">In the request body, supply a JSON representation of [privilegedApproval](../resources/privilegedapproval.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="cde70-138">响应</span><span class="sxs-lookup"><span data-stu-id="cde70-138">Response</span></span>
<span data-ttu-id="cde70-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cde70-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
