---
title: 更新权限
description: 更新网站上的权限对象。
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 27f006e5a2059662903f710ac994e176e1d51a22
ms.sourcegitcommit: 16ee16e7fddd662ca42dc5c9352cfb109e31ed1a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/03/2021
ms.locfileid: "51582597"
---
# <a name="update-permission"></a><span data-ttu-id="45732-103">更新权限</span><span class="sxs-lookup"><span data-stu-id="45732-103">Update permission</span></span>
<span data-ttu-id="45732-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="45732-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45732-105">更新 [网站上](../resources/permission.md) 的权限对象。</span><span class="sxs-lookup"><span data-stu-id="45732-105">Update the [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="45732-106">权限</span><span class="sxs-lookup"><span data-stu-id="45732-106">Permissions</span></span>
<span data-ttu-id="45732-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45732-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45732-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="45732-109">Permission type</span></span>                        | <span data-ttu-id="45732-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45732-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="45732-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45732-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="45732-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="45732-112">Not supported.</span></span>
|<span data-ttu-id="45732-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45732-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45732-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="45732-114">Not supported.</span></span>
|<span data-ttu-id="45732-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="45732-115">Application</span></span>                            | <span data-ttu-id="45732-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="45732-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="45732-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45732-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /sites/{sitesId}/permissions/{permissionId}
```

## <a name="request-headers"></a><span data-ttu-id="45732-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="45732-118">Request headers</span></span>
|<span data-ttu-id="45732-119">名称</span><span class="sxs-lookup"><span data-stu-id="45732-119">Name</span></span>|<span data-ttu-id="45732-120">说明</span><span class="sxs-lookup"><span data-stu-id="45732-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="45732-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="45732-121">Authorization</span></span>|<span data-ttu-id="45732-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="45732-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="45732-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="45732-124">Content-Type</span></span>|<span data-ttu-id="45732-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="45732-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="45732-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="45732-127">Request body</span></span>
<span data-ttu-id="45732-128">在请求正文中，提供 permission 对象的 JSON [表示](../resources/permission.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="45732-128">In the request body, supply a JSON representation of the [permission](../resources/permission.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="45732-129">响应</span><span class="sxs-lookup"><span data-stu-id="45732-129">Response</span></span>

<span data-ttu-id="45732-130">如果成功，此方法在响应 `200 OK` 正文中返回 [响应](../resources/permission.md) 代码和 permission 对象。</span><span class="sxs-lookup"><span data-stu-id="45732-130">If successful, this method returns a `200 OK` response code and a [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="45732-131">示例</span><span class="sxs-lookup"><span data-stu-id="45732-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="45732-132">请求</span><span class="sxs-lookup"><span data-stu-id="45732-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="45732-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="45732-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_permission_from_"
}
-->
``` http
PATCH https://graph.microsoft.com/beta/sites/{sitesId}/permissions/{permissionId}
Content-Type: application/json

{
  "roles": ["read"]
}
```
# <a name="c"></a>[<span data-ttu-id="45732-134">C#</span><span class="sxs-lookup"><span data-stu-id="45732-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-permission-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="45732-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="45732-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-permission-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="45732-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="45732-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-permission-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="45732-137">Java</span><span class="sxs-lookup"><span data-stu-id="45732-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-permission-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="45732-138">响应</span><span class="sxs-lookup"><span data-stu-id="45732-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
   "id":"2",
   "roles":[
      "read"
   ],
   "grantedToIdentities":[
      {
         "application":{
            "id":"89ea5c94-7736-4e25-95ad-3fa95f62b66e",
            "displayName":"Fabrikam Dashboard App"
         }
      }
   ]
}
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Update site permission"
} -->
