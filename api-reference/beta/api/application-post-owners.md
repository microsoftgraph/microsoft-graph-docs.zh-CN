---
title: 创建所有者
description: 使用此 API 创建新的所有者。
author: VinodRavichandran
localization_priority: Normal
ms.prod: microsoft-teams
doc_type: apiPageType
ms.openlocfilehash: 7c7ace73e1d6a2db3bac4502f9ddae6f4f0c0e1f
ms.sourcegitcommit: b18f978808fef800bff9e587464a5f3e18eb7687
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/25/2019
ms.locfileid: "35856769"
---
# <a name="create-owner"></a><span data-ttu-id="c8fda-103">创建所有者</span><span class="sxs-lookup"><span data-stu-id="c8fda-103">Create owner</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c8fda-104">使用此 API 创建新的所有者。</span><span class="sxs-lookup"><span data-stu-id="c8fda-104">Use this API to create a new owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="c8fda-105">权限</span><span class="sxs-lookup"><span data-stu-id="c8fda-105">Permissions</span></span>
<span data-ttu-id="c8fda-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c8fda-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c8fda-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c8fda-108">Permission type</span></span>      | <span data-ttu-id="c8fda-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c8fda-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c8fda-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c8fda-110">Delegated (work or school account)</span></span> |  <span data-ttu-id="c8fda-111">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c8fda-111">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c8fda-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c8fda-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c8fda-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c8fda-113">Not supported.</span></span>    |
|<span data-ttu-id="c8fda-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c8fda-114">Application</span></span> | <span data-ttu-id="c8fda-115">Application.readwrite.ownedby 和 "全部读取"。全部、全部读取全部和全部读取全部。</span><span class="sxs-lookup"><span data-stu-id="c8fda-115">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c8fda-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c8fda-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="c8fda-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c8fda-117">Request headers</span></span>
| <span data-ttu-id="c8fda-118">名称</span><span class="sxs-lookup"><span data-stu-id="c8fda-118">Name</span></span> | <span data-ttu-id="c8fda-119">说明</span><span class="sxs-lookup"><span data-stu-id="c8fda-119">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="c8fda-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c8fda-120">Authorization</span></span> | <span data-ttu-id="c8fda-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c8fda-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="c8fda-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="c8fda-123">Request body</span></span>
<span data-ttu-id="c8fda-124">在请求正文中, 提供要作为所有者分配的目录对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="c8fda-124">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="c8fda-125">响应</span><span class="sxs-lookup"><span data-stu-id="c8fda-125">Response</span></span>

<span data-ttu-id="c8fda-126">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c8fda-126">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c8fda-127">示例</span><span class="sxs-lookup"><span data-stu-id="c8fda-127">Example</span></span>
### <a name="request"></a><span data-ttu-id="c8fda-128">请求</span><span class="sxs-lookup"><span data-stu-id="c8fda-128">Request</span></span>
<span data-ttu-id="c8fda-129">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="c8fda-129">The following example shows the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="c8fda-130">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="c8fda-130">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_directoryobject_from_application"
}-->
```http
POST https://graph.microsoft.com/beta/applications/{id}/owners/$ref
Content-type: application/json
Content-length: 30

{
"@odata.id": "https://graph.microsoft.com/beta/directoryObjects/{id}"
}

```
# <a name="javascripttabjavascript"></a>[<span data-ttu-id="c8fda-131">Javascript</span><span class="sxs-lookup"><span data-stu-id="c8fda-131">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="c8fda-132">响应</span><span class="sxs-lookup"><span data-stu-id="c8fda-132">Response</span></span>

<span data-ttu-id="c8fda-133">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="c8fda-133">The following is an example of the response.</span></span>

><span data-ttu-id="c8fda-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c8fda-134">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="c8fda-135">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="c8fda-135">All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create owner",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
