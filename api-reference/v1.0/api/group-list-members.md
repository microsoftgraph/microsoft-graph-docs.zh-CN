---
title: 列出成员
description: 获取组的直接成员的列表。 一组可将用户、 联系人和其他组作为成员。
localization_priority: Priority
ms.openlocfilehash: d7dfaede0e9deae6806499b504c6a58da2381ef5
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27833283"
---
# <a name="list-members"></a><span data-ttu-id="7dce7-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="7dce7-104">List members</span></span>
<span data-ttu-id="7dce7-p102">获取组的直接成员列表。组可将用户、联系人和其他组作为成员。此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="7dce7-p102">Get a list of the group's direct members. A group can have users, contacts, and other groups as members. This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="7dce7-108">权限</span><span class="sxs-lookup"><span data-stu-id="7dce7-108">Permissions</span></span>
<span data-ttu-id="7dce7-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7dce7-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dce7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7dce7-111">Permission type</span></span>      | <span data-ttu-id="7dce7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7dce7-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7dce7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7dce7-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7dce7-114">User.ReadBasic.All、User.Read.All、Directory.Read.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7dce7-114">User.ReadBasic.All, User.Read.All, Directory.Read.All, Directory.AccessAsUser.All</span></span>   |
|<span data-ttu-id="7dce7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7dce7-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7dce7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7dce7-116">Not supported.</span></span>    |
|<span data-ttu-id="7dce7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7dce7-117">Application</span></span> | <span data-ttu-id="7dce7-118">User.Read.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="7dce7-118">User.Read.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7dce7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7dce7-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/members
```

## <a name="optional-query-parameters"></a><span data-ttu-id="7dce7-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7dce7-120">Optional query parameters</span></span>
<span data-ttu-id="7dce7-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7dce7-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7dce7-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7dce7-122">Request headers</span></span>
| <span data-ttu-id="7dce7-123">名称</span><span class="sxs-lookup"><span data-stu-id="7dce7-123">Name</span></span>       | <span data-ttu-id="7dce7-124">类型</span><span class="sxs-lookup"><span data-stu-id="7dce7-124">Type</span></span> | <span data-ttu-id="7dce7-125">说明</span><span class="sxs-lookup"><span data-stu-id="7dce7-125">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="7dce7-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dce7-126">Authorization</span></span>  | <span data-ttu-id="7dce7-127">string</span><span class="sxs-lookup"><span data-stu-id="7dce7-127">string</span></span>  | <span data-ttu-id="7dce7-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7dce7-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7dce7-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="7dce7-130">Request body</span></span>
<span data-ttu-id="7dce7-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7dce7-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7dce7-132">响应</span><span class="sxs-lookup"><span data-stu-id="7dce7-132">Response</span></span>
<span data-ttu-id="7dce7-133">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="7dce7-133">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dce7-134">示例</span><span class="sxs-lookup"><span data-stu-id="7dce7-134">Example</span></span>
#### <a name="request"></a><span data-ttu-id="7dce7-135">请求</span><span class="sxs-lookup"><span data-stu-id="7dce7-135">Request</span></span>
<span data-ttu-id="7dce7-136">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7dce7-136">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/v1.0/groups/{id}/members
```

#### <a name="response"></a><span data-ttu-id="7dce7-137">响应</span><span class="sxs-lookup"><span data-stu-id="7dce7-137">Response</span></span>
<span data-ttu-id="7dce7-138">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7dce7-138">The following is an example of the response.</span></span>
><span data-ttu-id="7dce7-139">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="7dce7-139">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="7dce7-140">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7dce7-140">All the properties will be returned from an actual call.</span></span>
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
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
