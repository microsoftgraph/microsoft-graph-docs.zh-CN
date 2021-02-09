---
title: 删除权限
description: 删除网站上的权限对象。
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 25d5cb047f43b3cd3d057a76bd898bbb989486ee
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160279"
---
# <a name="delete-permission"></a><span data-ttu-id="a9734-103">删除权限</span><span class="sxs-lookup"><span data-stu-id="a9734-103">Delete permission</span></span>
<span data-ttu-id="a9734-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9734-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="a9734-105">删除 [网站上](../resources/permission.md) 的权限对象。</span><span class="sxs-lookup"><span data-stu-id="a9734-105">Delete a [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="a9734-106">权限</span><span class="sxs-lookup"><span data-stu-id="a9734-106">Permissions</span></span>
<span data-ttu-id="a9734-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9734-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9734-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9734-109">Permission type</span></span>                        | <span data-ttu-id="a9734-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9734-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="a9734-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9734-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="a9734-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9734-112">Not supported.</span></span>
|<span data-ttu-id="a9734-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9734-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a9734-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9734-114">Not supported.</span></span>
|<span data-ttu-id="a9734-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9734-115">Application</span></span>                            | <span data-ttu-id="a9734-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="a9734-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="a9734-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9734-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /sites/{sitesId}/permissions/{permissionId}
```

## <a name="request-headers"></a><span data-ttu-id="a9734-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9734-118">Request headers</span></span>
|<span data-ttu-id="a9734-119">名称</span><span class="sxs-lookup"><span data-stu-id="a9734-119">Name</span></span>|<span data-ttu-id="a9734-120">说明</span><span class="sxs-lookup"><span data-stu-id="a9734-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a9734-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9734-121">Authorization</span></span>|<span data-ttu-id="a9734-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a9734-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9734-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9734-124">Request body</span></span>
<span data-ttu-id="a9734-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a9734-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a9734-126">响应</span><span class="sxs-lookup"><span data-stu-id="a9734-126">Response</span></span>

<span data-ttu-id="a9734-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="a9734-p103">If successful, this method returns `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="a9734-129">示例</span><span class="sxs-lookup"><span data-stu-id="a9734-129">Examples</span></span>

### <a name="request"></a><span data-ttu-id="a9734-130">请求</span><span class="sxs-lookup"><span data-stu-id="a9734-130">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_permission"
}
-->
``` http
DELETE https://graph.microsoft.com/beta/sites/{sitesId}/permissions/{permissionId}
```


### <a name="response"></a><span data-ttu-id="a9734-131">响应</span><span class="sxs-lookup"><span data-stu-id="a9734-131">Response</span></span>
<span data-ttu-id="a9734-132">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="a9734-132">Here is an example of the response.</span></span> 
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
