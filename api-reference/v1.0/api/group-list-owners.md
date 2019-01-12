---
title: 列出所有者
description: '检索组的所有者列表。所有者是一组具有 group 对象修改权限的非管理员用户。 '
localization_priority: Priority
author: dkershaw10
ms.prod: groups
ms.openlocfilehash: 5c8cf1c82ceab0a7fa2a7f78b6c229165448d46e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972206"
---
# <a name="list-owners"></a><span data-ttu-id="59f1c-104">列出所有者</span><span class="sxs-lookup"><span data-stu-id="59f1c-104">List owners</span></span>
<span data-ttu-id="59f1c-p102">检索组的所有者列表。所有者是一组具有 group 对象修改权限的非管理员用户。</span><span class="sxs-lookup"><span data-stu-id="59f1c-p102">Retrieve a list of the group's owners. The owners are a set of non-admin users who are allowed to modify the group object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="59f1c-107">权限</span><span class="sxs-lookup"><span data-stu-id="59f1c-107">Permissions</span></span>
<span data-ttu-id="59f1c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="59f1c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="59f1c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="59f1c-110">Permission type</span></span>      | <span data-ttu-id="59f1c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="59f1c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="59f1c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="59f1c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="59f1c-113">Group.Read.All 和 User.ReadBasic.All、Group.Read.All 和 User.Read.All、Group.Read.All 和 User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59f1c-113">Group.Read.All and User.ReadBasic.All, Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span>   |
|<span data-ttu-id="59f1c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="59f1c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="59f1c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="59f1c-115">Not supported.</span></span>    |
|<span data-ttu-id="59f1c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="59f1c-116">Application</span></span> | <span data-ttu-id="59f1c-117">Group.Read.All 和 User.Read.All、Group.Read.All 和User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="59f1c-117">Group.Read.All and User.Read.All, Group.Read.All and User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="59f1c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="59f1c-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/owners
```

## <a name="optional-query-parameters"></a><span data-ttu-id="59f1c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="59f1c-119">Optional query parameters</span></span>
<span data-ttu-id="59f1c-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="59f1c-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="59f1c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="59f1c-121">Request headers</span></span>
| <span data-ttu-id="59f1c-122">名称</span><span class="sxs-lookup"><span data-stu-id="59f1c-122">Name</span></span>       | <span data-ttu-id="59f1c-123">类型</span><span class="sxs-lookup"><span data-stu-id="59f1c-123">Type</span></span> | <span data-ttu-id="59f1c-124">说明</span><span class="sxs-lookup"><span data-stu-id="59f1c-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="59f1c-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="59f1c-125">Authorization</span></span>  | <span data-ttu-id="59f1c-126">string</span><span class="sxs-lookup"><span data-stu-id="59f1c-126">string</span></span>  | <span data-ttu-id="59f1c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="59f1c-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="59f1c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="59f1c-129">Request body</span></span>
<span data-ttu-id="59f1c-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="59f1c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="59f1c-131">响应</span><span class="sxs-lookup"><span data-stu-id="59f1c-131">Response</span></span>
<span data-ttu-id="59f1c-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [user](../resources/user.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="59f1c-132">If successful, this method returns a `200 OK` response code and collection of [user](../resources/user.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="59f1c-133">示例</span><span class="sxs-lookup"><span data-stu-id="59f1c-133">Example</span></span>
#### <a name="request"></a><span data-ttu-id="59f1c-134">请求</span><span class="sxs-lookup"><span data-stu-id="59f1c-134">Request</span></span>
<span data-ttu-id="59f1c-135">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="59f1c-135">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_owners"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/owners
```

#### <a name="response"></a><span data-ttu-id="59f1c-136">响应</span><span class="sxs-lookup"><span data-stu-id="59f1c-136">Response</span></span>
<span data-ttu-id="59f1c-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="59f1c-137">The following is an example of the response.</span></span>
><span data-ttu-id="59f1c-138">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="59f1c-138">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="59f1c-139">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="59f1c-139">All the properties will be returned from an actual call.</span></span>
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
      "@odata.type": "#microsoft.graph.user"
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
