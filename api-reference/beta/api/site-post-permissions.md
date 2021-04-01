---
title: 创建权限
description: 创建新的 permission 对象。
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 34ef9db31610c930c0b516b822b63372cddab0b5
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51474072"
---
# <a name="create-permission"></a><span data-ttu-id="d73aa-103">创建权限</span><span class="sxs-lookup"><span data-stu-id="d73aa-103">Create permission</span></span>
<span data-ttu-id="d73aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d73aa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d73aa-105">在网站 [中](../resources/permission.md) 创建新的 permission 对象。</span><span class="sxs-lookup"><span data-stu-id="d73aa-105">Create a new [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="d73aa-106">权限</span><span class="sxs-lookup"><span data-stu-id="d73aa-106">Permissions</span></span>
<span data-ttu-id="d73aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d73aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d73aa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d73aa-109">Permission type</span></span>                        | <span data-ttu-id="d73aa-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d73aa-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="d73aa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d73aa-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="d73aa-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="d73aa-112">Not supported.</span></span>
|<span data-ttu-id="d73aa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d73aa-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d73aa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d73aa-114">Not supported.</span></span>
|<span data-ttu-id="d73aa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d73aa-115">Application</span></span>                            | <span data-ttu-id="d73aa-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="d73aa-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="d73aa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d73aa-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /sites/{sitesId}/permissions
```

## <a name="request-headers"></a><span data-ttu-id="d73aa-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d73aa-118">Request headers</span></span>
|<span data-ttu-id="d73aa-119">名称</span><span class="sxs-lookup"><span data-stu-id="d73aa-119">Name</span></span>|<span data-ttu-id="d73aa-120">说明</span><span class="sxs-lookup"><span data-stu-id="d73aa-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="d73aa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d73aa-121">Authorization</span></span>|<span data-ttu-id="d73aa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d73aa-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="d73aa-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="d73aa-124">Content-Type</span></span>|<span data-ttu-id="d73aa-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="d73aa-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="d73aa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d73aa-127">Request body</span></span>
<span data-ttu-id="d73aa-128">在请求正文中，提供 permission 对象的 JSON [表示](../resources/permission.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="d73aa-128">In the request body, supply a JSON representation of the [permission](../resources/permission.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="d73aa-129">响应</span><span class="sxs-lookup"><span data-stu-id="d73aa-129">Response</span></span>

<span data-ttu-id="d73aa-130">如果成功，此方法在响应 `201 Created` 正文中返回 [响应](../resources/permission.md) 代码和 permission 对象。</span><span class="sxs-lookup"><span data-stu-id="d73aa-130">If successful, this method returns a `201 Created` response code and a [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="d73aa-131">示例</span><span class="sxs-lookup"><span data-stu-id="d73aa-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="d73aa-132">请求</span><span class="sxs-lookup"><span data-stu-id="d73aa-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="d73aa-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="d73aa-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_permission_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/sites/{sitesId}/permissions
Content-Type: application/json

{
  "roles": ["write"],
  "grantedToIdentities": [{
    "application": {
      "id": "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
      "displayName": "Contoso Time Manager App"
    }
  }]
}
```
# <a name="c"></a>[<span data-ttu-id="d73aa-134">C#</span><span class="sxs-lookup"><span data-stu-id="d73aa-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-permission-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="d73aa-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="d73aa-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-permission-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="d73aa-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="d73aa-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-permission-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="d73aa-137">Java</span><span class="sxs-lookup"><span data-stu-id="d73aa-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-permission-from--java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="d73aa-138">响应</span><span class="sxs-lookup"><span data-stu-id="d73aa-138">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.permission"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
    "id": "1",
    "roles": ["write"],
    "grantedToIdentities": [{
      "application": {
        "id": "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
        "displayName": "Contoso Time Manager App"
      }
    }]
}
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Create site permissions"
} -->
