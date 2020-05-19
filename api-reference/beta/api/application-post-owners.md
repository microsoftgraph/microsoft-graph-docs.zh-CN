---
title: 添加所有者
description: 使用此 API 将所有者添加到应用程序。
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 0d22addf96dfa3b900b4d195b8fb0611548fced5
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289136"
---
# <a name="add-owner"></a><span data-ttu-id="ff763-103">添加所有者</span><span class="sxs-lookup"><span data-stu-id="ff763-103">Add owner</span></span>

<span data-ttu-id="ff763-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ff763-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ff763-105">使用此 API 将所有者添加到应用程序，方法是发布到所有者集合。</span><span class="sxs-lookup"><span data-stu-id="ff763-105">Use this API to add an owner to an application by posting to the owners collection.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff763-106">权限</span><span class="sxs-lookup"><span data-stu-id="ff763-106">Permissions</span></span>
<span data-ttu-id="ff763-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff763-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff763-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff763-109">Permission type</span></span>      | <span data-ttu-id="ff763-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ff763-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff763-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff763-111">Delegated (work or school account)</span></span> |  <span data-ttu-id="ff763-112">"ReadWrite"、"全部" 和 "Directory.accessasuser.all"、"全部"、"全部"、"所有"</span><span class="sxs-lookup"><span data-stu-id="ff763-112">Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ff763-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff763-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff763-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff763-114">Not supported.</span></span>    |
|<span data-ttu-id="ff763-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff763-115">Application</span></span> | <span data-ttu-id="ff763-116">Application.readwrite.ownedby 和目录。全部，全部读取全部，全部为。所有读写全部。 all</span><span class="sxs-lookup"><span data-stu-id="ff763-116">Application.ReadWrite.OwnedBy and Directory.Read.All, Application.ReadWrite.All and Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff763-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff763-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/owners/$ref

```
## <a name="request-headers"></a><span data-ttu-id="ff763-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff763-118">Request headers</span></span>
| <span data-ttu-id="ff763-119">名称</span><span class="sxs-lookup"><span data-stu-id="ff763-119">Name</span></span> | <span data-ttu-id="ff763-120">说明</span><span class="sxs-lookup"><span data-stu-id="ff763-120">Description</span></span>|
|:---- |:---------- |
| <span data-ttu-id="ff763-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff763-121">Authorization</span></span> | <span data-ttu-id="ff763-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ff763-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ff763-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff763-124">Request body</span></span>
<span data-ttu-id="ff763-125">在请求正文中，提供要作为所有者分配的目录对象的标识符。</span><span class="sxs-lookup"><span data-stu-id="ff763-125">In the request body, supply the identifier of the directory object to be assigned as owner.</span></span>

## <a name="response"></a><span data-ttu-id="ff763-126">响应</span><span class="sxs-lookup"><span data-stu-id="ff763-126">Response</span></span>

<span data-ttu-id="ff763-127">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ff763-127">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ff763-128">示例</span><span class="sxs-lookup"><span data-stu-id="ff763-128">Example</span></span>
### <a name="request"></a><span data-ttu-id="ff763-129">请求</span><span class="sxs-lookup"><span data-stu-id="ff763-129">Request</span></span>
<span data-ttu-id="ff763-130">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="ff763-130">The following example shows the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="ff763-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ff763-131">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="ff763-132">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff763-132">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-directoryobject-from-application-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="ff763-133">C#</span><span class="sxs-lookup"><span data-stu-id="ff763-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-directoryobject-from-application-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ff763-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ff763-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-directoryobject-from-application-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="ff763-135">响应</span><span class="sxs-lookup"><span data-stu-id="ff763-135">Response</span></span>

<span data-ttu-id="ff763-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ff763-136">The following is an example of the response.</span></span>

><span data-ttu-id="ff763-137">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ff763-137">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="ff763-138">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ff763-138">All the properties will be returned from an actual call.</span></span>

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
