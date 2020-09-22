---
title: 删除 programControl
description: 在 "Azure AD access 评论" 功能中，删除 programControl 对象。  这会断开某个程序的访问评审。
localization_priority: Normal
doc_type: apiPageType
ms.prod: microsoft-identity-platform
author: markwahl-msft
ms.openlocfilehash: fd9254deb969a860b14268057421e4e1547c7a08
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48087934"
---
# <a name="delete-programcontrol"></a><span data-ttu-id="67e37-104">删除 programControl</span><span class="sxs-lookup"><span data-stu-id="67e37-104">Delete programControl</span></span>

<span data-ttu-id="67e37-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="67e37-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="67e37-106">在 "Azure AD [access 评论](../resources/accessreviews-root.md) " 功能中，删除 [programControl](../resources/programcontrol.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="67e37-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, delete a [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="67e37-107">这会断开某个程序的访问评审。</span><span class="sxs-lookup"><span data-stu-id="67e37-107">This unlinks an access review from a program.</span></span>
## <a name="permissions"></a><span data-ttu-id="67e37-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="67e37-108">Permissions</span></span>
<span data-ttu-id="67e37-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67e37-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67e37-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="67e37-111">Permission type</span></span>                        | <span data-ttu-id="67e37-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="67e37-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="67e37-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67e37-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="67e37-114">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67e37-114">ProgramControl.ReadWrite.All</span></span>   |
|<span data-ttu-id="67e37-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67e37-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="67e37-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="67e37-116">Not supported.</span></span> |
|<span data-ttu-id="67e37-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="67e37-117">Application</span></span>                            | <span data-ttu-id="67e37-118">ProgramControl.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67e37-118">ProgramControl.ReadWrite.All</span></span>  |

<span data-ttu-id="67e37-119">登录用户还必须位于允许他们删除的目录角色中 `programControl` 。</span><span class="sxs-lookup"><span data-stu-id="67e37-119">The signed in user must also be in a directory role that permits them to delete a `programControl`.</span></span>

## <a name="http-request"></a><span data-ttu-id="67e37-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67e37-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /programControls/{id}
```
## <a name="request-headers"></a><span data-ttu-id="67e37-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="67e37-121">Request headers</span></span>
| <span data-ttu-id="67e37-122">名称</span><span class="sxs-lookup"><span data-stu-id="67e37-122">Name</span></span>         | <span data-ttu-id="67e37-123">类型</span><span class="sxs-lookup"><span data-stu-id="67e37-123">Type</span></span>        | <span data-ttu-id="67e37-124">说明</span><span class="sxs-lookup"><span data-stu-id="67e37-124">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="67e37-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="67e37-125">Authorization</span></span> | <span data-ttu-id="67e37-126">string</span><span class="sxs-lookup"><span data-stu-id="67e37-126">string</span></span> | <span data-ttu-id="67e37-p104">持有者 \{token\}。必需。</span><span class="sxs-lookup"><span data-stu-id="67e37-p104">Bearer \{token\}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="67e37-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="67e37-129">Request body</span></span>
<span data-ttu-id="67e37-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="67e37-130">Do not supply a request body for this method.</span></span>


## <a name="response"></a><span data-ttu-id="67e37-131">响应</span><span class="sxs-lookup"><span data-stu-id="67e37-131">Response</span></span>
<span data-ttu-id="67e37-p105">如果成功，此方法返回 `204, No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="67e37-p105">If successful, this method returns a `204, No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67e37-134">示例</span><span class="sxs-lookup"><span data-stu-id="67e37-134">Example</span></span>
##### <a name="request"></a><span data-ttu-id="67e37-135">请求</span><span class="sxs-lookup"><span data-stu-id="67e37-135">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="67e37-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="67e37-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_programControl"
}-->
```http
DELETE https://graph.microsoft.com/beta/programControls/7e59d237-2fb0-4e5d-b7bb-d4f9f9129213
```
# <a name="c"></a>[<span data-ttu-id="67e37-137">C#</span><span class="sxs-lookup"><span data-stu-id="67e37-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-programcontrol-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="67e37-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="67e37-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-programcontrol-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="67e37-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="67e37-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-programcontrol-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="67e37-140">响应</span><span class="sxs-lookup"><span data-stu-id="67e37-140">Response</span></span>
><span data-ttu-id="67e37-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="67e37-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2017-06-25 00:00:01 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Delete programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->


