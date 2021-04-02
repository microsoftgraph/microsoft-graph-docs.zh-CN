---
title: 获取权限
description: 检索网站上 permission 对象的属性和关系。
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: 9a9c03b81292f18ee9af220e97072ce1952b5d47
ms.sourcegitcommit: 08d47a31c48fd69ae4fcee26e34fdd65ad1ba69f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/02/2021
ms.locfileid: "51508125"
---
# <a name="get-permission"></a><span data-ttu-id="e71f3-103">获取权限</span><span class="sxs-lookup"><span data-stu-id="e71f3-103">Get permission</span></span>
<span data-ttu-id="e71f3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e71f3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e71f3-105">检索网站上 [permission](../resources/permission.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="e71f3-105">Retrieve the properties and relationships of a [permission](../resources/permission.md) object on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="e71f3-106">权限</span><span class="sxs-lookup"><span data-stu-id="e71f3-106">Permissions</span></span>
<span data-ttu-id="e71f3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e71f3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e71f3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="e71f3-109">Permission type</span></span>                        | <span data-ttu-id="e71f3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e71f3-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="e71f3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e71f3-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="e71f3-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="e71f3-112">Not supported.</span></span>
|<span data-ttu-id="e71f3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e71f3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e71f3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="e71f3-114">Not supported.</span></span>
|<span data-ttu-id="e71f3-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="e71f3-115">Application</span></span>                            | <span data-ttu-id="e71f3-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="e71f3-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="e71f3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e71f3-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /sites/{sitesId}/permissions/{permissionId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="e71f3-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e71f3-118">Optional query parameters</span></span>
<span data-ttu-id="e71f3-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e71f3-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="e71f3-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="e71f3-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="e71f3-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e71f3-121">Request headers</span></span>
|<span data-ttu-id="e71f3-122">名称</span><span class="sxs-lookup"><span data-stu-id="e71f3-122">Name</span></span>|<span data-ttu-id="e71f3-123">说明</span><span class="sxs-lookup"><span data-stu-id="e71f3-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e71f3-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="e71f3-124">Authorization</span></span>|<span data-ttu-id="e71f3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e71f3-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e71f3-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e71f3-127">Request body</span></span>
<span data-ttu-id="e71f3-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e71f3-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e71f3-129">响应</span><span class="sxs-lookup"><span data-stu-id="e71f3-129">Response</span></span>

<span data-ttu-id="e71f3-130">如果成功，此方法在响应 `200 OK` 正文中返回 [响应](../resources/permission.md) 代码和 permission 对象。</span><span class="sxs-lookup"><span data-stu-id="e71f3-130">If successful, this method returns a `200 OK` response code and the [permission](../resources/permission.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e71f3-131">示例</span><span class="sxs-lookup"><span data-stu-id="e71f3-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e71f3-132">请求</span><span class="sxs-lookup"><span data-stu-id="e71f3-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="e71f3-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="e71f3-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_permission"
}
-->
``` http
GET https://graph.microsoft.com/beta/sites/{sitesId}/permissions/{permissionId}
```
# <a name="c"></a>[<span data-ttu-id="e71f3-134">C#</span><span class="sxs-lookup"><span data-stu-id="e71f3-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="e71f3-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="e71f3-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="e71f3-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="e71f3-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="e71f3-137">Java</span><span class="sxs-lookup"><span data-stu-id="e71f3-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="e71f3-138">响应</span><span class="sxs-lookup"><span data-stu-id="e71f3-138">Response</span></span>
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
   "id":"1",
   "roles":[
      "read"
   ],
   "grantedToIdentities":[
      {
         "application":{
            "id":"89ea5c94-7736-4e25-95ad-3fa95f62b66e",
            "displayName":"Contoso Time Manager App"
         }
      }
   ]
}
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/Get site permission"
} -->
