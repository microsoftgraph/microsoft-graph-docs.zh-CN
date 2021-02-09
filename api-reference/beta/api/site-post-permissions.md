---
title: 创建权限
description: 创建新的权限对象。
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 6952931c2925e0de229d93d47b62d77e702c1873
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160276"
---
# <a name="create-permission"></a><span data-ttu-id="88dac-103">创建权限</span><span class="sxs-lookup"><span data-stu-id="88dac-103">Create permission</span></span>
<span data-ttu-id="88dac-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="88dac-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="88dac-105">在网站上 [创建新的](../resources/permission.md) 权限对象。</span><span class="sxs-lookup"><span data-stu-id="88dac-105">Create a new [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="88dac-106">权限</span><span class="sxs-lookup"><span data-stu-id="88dac-106">Permissions</span></span>
<span data-ttu-id="88dac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88dac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88dac-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="88dac-109">Permission type</span></span>                        | <span data-ttu-id="88dac-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="88dac-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="88dac-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88dac-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="88dac-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="88dac-112">Not supported.</span></span>
|<span data-ttu-id="88dac-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88dac-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="88dac-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="88dac-114">Not supported.</span></span>
|<span data-ttu-id="88dac-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="88dac-115">Application</span></span>                            | <span data-ttu-id="88dac-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="88dac-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="88dac-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88dac-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /sites/{sitesId}/permissions
```

## <a name="request-headers"></a><span data-ttu-id="88dac-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="88dac-118">Request headers</span></span>
|<span data-ttu-id="88dac-119">名称</span><span class="sxs-lookup"><span data-stu-id="88dac-119">Name</span></span>|<span data-ttu-id="88dac-120">说明</span><span class="sxs-lookup"><span data-stu-id="88dac-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="88dac-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="88dac-121">Authorization</span></span>|<span data-ttu-id="88dac-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="88dac-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="88dac-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="88dac-124">Content-Type</span></span>|<span data-ttu-id="88dac-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="88dac-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="88dac-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="88dac-127">Request body</span></span>
<span data-ttu-id="88dac-128">在请求正文中，提供权限对象的 JSON [表示](../resources/permission.md) 形式。</span><span class="sxs-lookup"><span data-stu-id="88dac-128">In the request body, supply a JSON representation of the [permission](../resources/permission.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="88dac-129">响应</span><span class="sxs-lookup"><span data-stu-id="88dac-129">Response</span></span>

<span data-ttu-id="88dac-130">如果成功，此方法在响应 `201 Created` 正文中返回响应代码[](../resources/permission.md)和权限对象。</span><span class="sxs-lookup"><span data-stu-id="88dac-130">If successful, this method returns a `201 Created` response code and a [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="88dac-131">示例</span><span class="sxs-lookup"><span data-stu-id="88dac-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="88dac-132">请求</span><span class="sxs-lookup"><span data-stu-id="88dac-132">Request</span></span>
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
      "displayName": "Foo App"
    }
  }]
}
```


### <a name="response"></a><span data-ttu-id="88dac-133">响应</span><span class="sxs-lookup"><span data-stu-id="88dac-133">Response</span></span>

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
        "displayName": "Foo App"
      }
    }]
}
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Create site permissions"
} -->
