---
title: 列出权限
description: 从网站上的权限导航属性获取权限资源。
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: bcaa0cd18268bbfbc079883eb91cc74a88d87d96
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160277"
---
# <a name="list-permissions"></a><span data-ttu-id="3171c-103">列出权限</span><span class="sxs-lookup"><span data-stu-id="3171c-103">List permissions</span></span>
<span data-ttu-id="3171c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3171c-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3171c-105">从 [网站上](../resources/permission.md) 的权限导航属性获取权限资源。</span><span class="sxs-lookup"><span data-stu-id="3171c-105">Get the [permission](../resources/permission.md) resources from the permissions navigation property on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="3171c-106">权限</span><span class="sxs-lookup"><span data-stu-id="3171c-106">Permissions</span></span>
<span data-ttu-id="3171c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3171c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3171c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3171c-109">Permission type</span></span>                        | <span data-ttu-id="3171c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3171c-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="3171c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3171c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="3171c-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="3171c-112">Not supported.</span></span>
|<span data-ttu-id="3171c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3171c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3171c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3171c-114">Not supported.</span></span>
|<span data-ttu-id="3171c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3171c-115">Application</span></span>                            | <span data-ttu-id="3171c-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="3171c-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="3171c-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3171c-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /sites/{sitesId}/permissions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="3171c-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3171c-118">Optional query parameters</span></span>
<span data-ttu-id="3171c-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3171c-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="3171c-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="3171c-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="3171c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3171c-121">Request headers</span></span>
|<span data-ttu-id="3171c-122">名称</span><span class="sxs-lookup"><span data-stu-id="3171c-122">Name</span></span>|<span data-ttu-id="3171c-123">说明</span><span class="sxs-lookup"><span data-stu-id="3171c-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="3171c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3171c-124">Authorization</span></span>|<span data-ttu-id="3171c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3171c-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3171c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3171c-127">Request body</span></span>
<span data-ttu-id="3171c-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3171c-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3171c-129">响应</span><span class="sxs-lookup"><span data-stu-id="3171c-129">Response</span></span>

<span data-ttu-id="3171c-130">如果成功，此方法在响应 `200 OK` 正文中返回响应代码 [和权限](../resources/permission.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3171c-130">If successful, this method returns a `200 OK` response code and a collection of [permission](../resources/permission.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3171c-131">示例</span><span class="sxs-lookup"><span data-stu-id="3171c-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3171c-132">请求</span><span class="sxs-lookup"><span data-stu-id="3171c-132">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_permission"
}
-->
``` http
GET https://graph.microsoft.com/beta/sites/{sitesId}/permissions
```


### <a name="response"></a><span data-ttu-id="3171c-133">响应</span><span class="sxs-lookup"><span data-stu-id="3171c-133">Response</span></span>
<span data-ttu-id="3171c-134">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3171c-134">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.permission)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "id": "1",
      "roles": ["read"],
      "grantedToIdentities": [{
        "application": {
          "id": "89ea5c94-7736-4e25-95ad-3fa95f62b66e",
          "displayName": "Foo App"
        }
      }]
    },
    {
      "id": "2",
      "roles": ["write"],
      "grantedToIdentities": [{
        "application": {
          "id": "22f09bb7-dd29-403e-bec2-ab5cde52c2b3",
          "displayName": "Bar App"
        }
      }]
    }
  ]
}
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/List site permissions"
} -->