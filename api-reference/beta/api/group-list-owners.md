---
title: 列出所有者
description: 检索组的所有者列表。所有者是一组具有 group 对象修改权限的非管理员用户。
localization_priority: Normal
ms.openlocfilehash: d173b7a350d4aedbf1ec96b0b5e37da70e87d078
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27878972"
---
# <a name="list-owners"></a><span data-ttu-id="89942-104">列出所有者</span><span class="sxs-lookup"><span data-stu-id="89942-104">List owners</span></span>

> <span data-ttu-id="89942-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="89942-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89942-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="89942-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="89942-p103">检索组的所有者列表。所有者是一组具有 group 对象修改权限的非管理员用户。</span><span class="sxs-lookup"><span data-stu-id="89942-p103">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span>

## <a name="permissions"></a><span data-ttu-id="89942-109">权限</span><span class="sxs-lookup"><span data-stu-id="89942-109">Permissions</span></span>
<span data-ttu-id="89942-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89942-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="89942-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="89942-112">Permission type</span></span>      | <span data-ttu-id="89942-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89942-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="89942-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89942-114">Delegated (work or school account)</span></span> | <span data-ttu-id="89942-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="89942-115">Not supported.</span></span>    |
|<span data-ttu-id="89942-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89942-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89942-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="89942-117">Not supported.</span></span>    |
|<span data-ttu-id="89942-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="89942-118">Application</span></span> | <span data-ttu-id="89942-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="89942-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="89942-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89942-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="89942-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="89942-121">Optional query parameters</span></span>
<span data-ttu-id="89942-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="89942-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="89942-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="89942-123">Request headers</span></span>
| <span data-ttu-id="89942-124">名称</span><span class="sxs-lookup"><span data-stu-id="89942-124">Name</span></span>       | <span data-ttu-id="89942-125">类型</span><span class="sxs-lookup"><span data-stu-id="89942-125">Type</span></span> | <span data-ttu-id="89942-126">说明</span><span class="sxs-lookup"><span data-stu-id="89942-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="89942-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="89942-127">Authorization</span></span>  | <span data-ttu-id="89942-128">string</span><span class="sxs-lookup"><span data-stu-id="89942-128">string</span></span>  | <span data-ttu-id="89942-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="89942-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89942-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="89942-131">Request body</span></span>
<span data-ttu-id="89942-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="89942-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="89942-133">响应</span><span class="sxs-lookup"><span data-stu-id="89942-133">Response</span></span>
<span data-ttu-id="89942-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="89942-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="89942-135">示例</span><span class="sxs-lookup"><span data-stu-id="89942-135">Example</span></span>
#### <a name="request"></a><span data-ttu-id="89942-136">请求</span><span class="sxs-lookup"><span data-stu-id="89942-136">Request</span></span>
<span data-ttu-id="89942-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="89942-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="89942-138">响应</span><span class="sxs-lookup"><span data-stu-id="89942-138">Response</span></span>
<span data-ttu-id="89942-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="89942-139">The following is an example of the response.</span></span>
><span data-ttu-id="89942-140">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="89942-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="89942-141">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="89942-141">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 55

{
  "value": [
    {
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List owners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
