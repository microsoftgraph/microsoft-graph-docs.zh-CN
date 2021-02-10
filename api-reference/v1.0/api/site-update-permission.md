---
title: 更新权限
description: 更新网站上的权限对象。
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: c2942645dd2f4faa905f1ccfc87a6aa44132ecef
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162088"
---
# <a name="update-permission"></a><span data-ttu-id="24d7e-103">更新权限</span><span class="sxs-lookup"><span data-stu-id="24d7e-103">Update permission</span></span>
<span data-ttu-id="24d7e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24d7e-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="24d7e-105">更新 [网站上](../resources/permission.md) 的权限对象。</span><span class="sxs-lookup"><span data-stu-id="24d7e-105">Update the [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="24d7e-106">权限</span><span class="sxs-lookup"><span data-stu-id="24d7e-106">Permissions</span></span>
<span data-ttu-id="24d7e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24d7e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24d7e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="24d7e-109">Permission type</span></span>                        | <span data-ttu-id="24d7e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="24d7e-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="24d7e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24d7e-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="24d7e-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="24d7e-112">Not supported.</span></span>
|<span data-ttu-id="24d7e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24d7e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="24d7e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="24d7e-114">Not supported.</span></span>
|<span data-ttu-id="24d7e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="24d7e-115">Application</span></span>                            | <span data-ttu-id="24d7e-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="24d7e-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="24d7e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24d7e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /sites/{sitesId}/permissions/{permissionId}
```

## <a name="request-headers"></a><span data-ttu-id="24d7e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="24d7e-118">Request headers</span></span>
|<span data-ttu-id="24d7e-119">名称</span><span class="sxs-lookup"><span data-stu-id="24d7e-119">Name</span></span>|<span data-ttu-id="24d7e-120">说明</span><span class="sxs-lookup"><span data-stu-id="24d7e-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="24d7e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="24d7e-121">Authorization</span></span>|<span data-ttu-id="24d7e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="24d7e-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="24d7e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="24d7e-124">Content-Type</span></span>|<span data-ttu-id="24d7e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="24d7e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="24d7e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="24d7e-127">Request body</span></span>
<span data-ttu-id="24d7e-128">在请求正文中，提供权限对象的 JSON [表示](../resources/permission.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="24d7e-128">In the request body, supply a JSON representation of the [permission](../resources/permission.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="24d7e-129">响应</span><span class="sxs-lookup"><span data-stu-id="24d7e-129">Response</span></span>

<span data-ttu-id="24d7e-130">如果成功，此方法在响应 `200 OK` 正文中返回响应代码[](../resources/permission.md)和权限对象。</span><span class="sxs-lookup"><span data-stu-id="24d7e-130">If successful, this method returns a `200 OK` response code and a [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="24d7e-131">示例</span><span class="sxs-lookup"><span data-stu-id="24d7e-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="24d7e-132">请求</span><span class="sxs-lookup"><span data-stu-id="24d7e-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_permission_from_"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/sites/{sitesId}/permissions/{permissionId}
Content-Type: application/json

{
  "roles": ["read"]
}
```


### <a name="response"></a><span data-ttu-id="24d7e-133">响应</span><span class="sxs-lookup"><span data-stu-id="24d7e-133">Response</span></span>

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
    "id": "2",
    "roles": ["read"],
    "grantedToIdentities": [{
      "application": {
        "id": "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
        "displayName": "Bar App"
      }
    }]
}
```

<!-- {
  "type": "#page.annotation",
  "description": "",
  "keywords": "",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Update site permission",
  "suppressions": [
  ]
} -->
