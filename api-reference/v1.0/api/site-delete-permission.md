---
title: 删除权限
description: 删除网站上的权限对象。
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 53649ddaccb9094f222a0aff6e07b2e52144cbe8
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50952708"
---
# <a name="delete-permission"></a><span data-ttu-id="ddd8a-103">删除权限</span><span class="sxs-lookup"><span data-stu-id="ddd8a-103">Delete permission</span></span>
<span data-ttu-id="ddd8a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ddd8a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="ddd8a-105">删除 [网站上](../resources/permission.md) 的权限对象。</span><span class="sxs-lookup"><span data-stu-id="ddd8a-105">Delete a [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddd8a-106">权限</span><span class="sxs-lookup"><span data-stu-id="ddd8a-106">Permissions</span></span>
<span data-ttu-id="ddd8a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ddd8a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddd8a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ddd8a-109">Permission type</span></span>                        | <span data-ttu-id="ddd8a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ddd8a-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="ddd8a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ddd8a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="ddd8a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddd8a-112">Not supported.</span></span>
|<span data-ttu-id="ddd8a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ddd8a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddd8a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddd8a-114">Not supported.</span></span>
|<span data-ttu-id="ddd8a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ddd8a-115">Application</span></span>                            | <span data-ttu-id="ddd8a-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="ddd8a-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="ddd8a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ddd8a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /sites/{sitesId}/permissions/{permissionId}
```

## <a name="request-headers"></a><span data-ttu-id="ddd8a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ddd8a-118">Request headers</span></span>
|<span data-ttu-id="ddd8a-119">名称</span><span class="sxs-lookup"><span data-stu-id="ddd8a-119">Name</span></span>|<span data-ttu-id="ddd8a-120">说明</span><span class="sxs-lookup"><span data-stu-id="ddd8a-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ddd8a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddd8a-121">Authorization</span></span>|<span data-ttu-id="ddd8a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ddd8a-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddd8a-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ddd8a-124">Request body</span></span>
<span data-ttu-id="ddd8a-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ddd8a-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddd8a-126">响应</span><span class="sxs-lookup"><span data-stu-id="ddd8a-126">Response</span></span>

<span data-ttu-id="ddd8a-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ddd8a-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ddd8a-129">示例</span><span class="sxs-lookup"><span data-stu-id="ddd8a-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ddd8a-130">请求</span><span class="sxs-lookup"><span data-stu-id="ddd8a-130">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="ddd8a-131">HTTP</span><span class="sxs-lookup"><span data-stu-id="ddd8a-131">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "delete_permission_2"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/sites/{sitesId}/permissions/{permissionId}
```
# <a name="c"></a>[<span data-ttu-id="ddd8a-132">C#</span><span class="sxs-lookup"><span data-stu-id="ddd8a-132">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/delete-permission-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="ddd8a-133">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ddd8a-133">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/delete-permission-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ddd8a-134">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ddd8a-134">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/delete-permission-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="ddd8a-135">Java</span><span class="sxs-lookup"><span data-stu-id="ddd8a-135">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/delete-permission-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="ddd8a-136">响应</span><span class="sxs-lookup"><span data-stu-id="ddd8a-136">Response</span></span>
<span data-ttu-id="ddd8a-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ddd8a-137">Here is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Delete site permission"
} -->
