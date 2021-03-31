---
title: 列出权限
description: 从网站上的权限导航属性获取权限资源。
author: BarrySh
localization_priority: Normal
ms.prod: sharepoint
doc_type: apiPageType
ms.openlocfilehash: b4c950aec7b58eb6583e8b7a0a209a64f022368e
ms.sourcegitcommit: 17f1c9cff2e59049b894db32435af02e4ae32a70
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/31/2021
ms.locfileid: "51473211"
---
# <a name="list-permissions"></a><span data-ttu-id="1e28a-103">列出权限</span><span class="sxs-lookup"><span data-stu-id="1e28a-103">List permissions</span></span>
<span data-ttu-id="1e28a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e28a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e28a-105">从 [网站上](../resources/permission.md) 的权限导航属性获取权限资源。</span><span class="sxs-lookup"><span data-stu-id="1e28a-105">Get the [permission](../resources/permission.md) resources from the permissions navigation property on a site.</span></span>

## <a name="permissions"></a><span data-ttu-id="1e28a-106">权限</span><span class="sxs-lookup"><span data-stu-id="1e28a-106">Permissions</span></span>
<span data-ttu-id="1e28a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e28a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e28a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e28a-109">Permission type</span></span>                        | <span data-ttu-id="1e28a-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e28a-110">Permissions (from least to most privileged)</span></span>
|:--------------------------------------|:-------------------------------------
|<span data-ttu-id="1e28a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e28a-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="1e28a-112">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e28a-112">Not supported.</span></span>
|<span data-ttu-id="1e28a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e28a-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1e28a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e28a-114">Not supported.</span></span>
|<span data-ttu-id="1e28a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e28a-115">Application</span></span>                            | <span data-ttu-id="1e28a-116">Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="1e28a-116">Sites.FullControl.All</span></span>

## <a name="http-request"></a><span data-ttu-id="1e28a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e28a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /sites/{sitesId}/permissions
```

## <a name="optional-query-parameters"></a><span data-ttu-id="1e28a-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="1e28a-118">Optional query parameters</span></span>
<span data-ttu-id="1e28a-119">此方法支持一些 OData 查询参数来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="1e28a-119">This method supports some of the OData query parameters to help customize the response.</span></span> <span data-ttu-id="1e28a-120">若要了解一般信息，请参阅 [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="1e28a-120">For general information, see [OData query parameters](/graph/query-parameters).</span></span>

## <a name="request-headers"></a><span data-ttu-id="1e28a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e28a-121">Request headers</span></span>
|<span data-ttu-id="1e28a-122">名称</span><span class="sxs-lookup"><span data-stu-id="1e28a-122">Name</span></span>|<span data-ttu-id="1e28a-123">说明</span><span class="sxs-lookup"><span data-stu-id="1e28a-123">Description</span></span>|
|:---|:---|
|<span data-ttu-id="1e28a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e28a-124">Authorization</span></span>|<span data-ttu-id="1e28a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1e28a-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e28a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e28a-127">Request body</span></span>
<span data-ttu-id="1e28a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1e28a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1e28a-129">响应</span><span class="sxs-lookup"><span data-stu-id="1e28a-129">Response</span></span>

<span data-ttu-id="1e28a-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [permission](../resources/permission.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1e28a-130">If successful, this method returns a `200 OK` response code and a collection of [permission](../resources/permission.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1e28a-131">示例</span><span class="sxs-lookup"><span data-stu-id="1e28a-131">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1e28a-132">请求</span><span class="sxs-lookup"><span data-stu-id="1e28a-132">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="1e28a-133">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e28a-133">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_permission"
}
-->
``` http
GET https://graph.microsoft.com/beta/sites/{sitesId}/permissions
```
# <a name="c"></a>[<span data-ttu-id="1e28a-134">C#</span><span class="sxs-lookup"><span data-stu-id="1e28a-134">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-permission-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1e28a-135">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e28a-135">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-permission-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1e28a-136">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1e28a-136">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-permission-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1e28a-137">Java</span><span class="sxs-lookup"><span data-stu-id="1e28a-137">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-permission-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="1e28a-138">响应</span><span class="sxs-lookup"><span data-stu-id="1e28a-138">Response</span></span>
<span data-ttu-id="1e28a-139">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1e28a-139">**Note:** The response object shown here might be shortened for readability.</span></span>
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
   "value":[
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
      },
      {
         "id":"2",
         "roles":[
            "write"
         ],
         "grantedToIdentities":[
            {
               "application":{
                  "id":"22f09bb7-dd29-403e-bec2-ab5cde52c2b3",
                  "displayName":"Fabrikam Dashboard App"
               }
            }
         ]
      }
   ]
}
```

<!-- {
  "type": "#page.annotation",
  "section": "documentation",
  "tocPath": "Sites/Permissions/List site permissions"
} -->
