---
title: 列表组 memberOf
description: 获取组和管理组是直接成员的单位。
ms.openlocfilehash: 5c189571095676d0c52b8bb93a8d27136d4aaa3c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044488"
---
# <a name="list-group-memberof"></a><span data-ttu-id="b955f-103">列表组 memberOf</span><span class="sxs-lookup"><span data-stu-id="b955f-103">List group memberOf</span></span>

> <span data-ttu-id="b955f-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b955f-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b955f-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b955f-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b955f-106">获取组和管理组是直接成员的单位。</span><span class="sxs-lookup"><span data-stu-id="b955f-106">Get groups and administrative units that the group is a direct member of.</span></span>

<span data-ttu-id="b955f-107">此操作是不可传递的。</span><span class="sxs-lookup"><span data-stu-id="b955f-107">This operation is not transitive.</span></span> <span data-ttu-id="b955f-108">与不同获取用户的 Office 365 组，这将返回所有类型的组，而不仅仅是 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="b955f-108">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span> 

## <a name="permissions"></a><span data-ttu-id="b955f-109">权限</span><span class="sxs-lookup"><span data-stu-id="b955f-109">Permissions</span></span>

<span data-ttu-id="b955f-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b955f-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b955f-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="b955f-112">Permission type</span></span>      | <span data-ttu-id="b955f-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b955f-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b955f-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b955f-114">Delegated (work or school account)</span></span> | <span data-ttu-id="b955f-115">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="b955f-115">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="b955f-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b955f-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b955f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="b955f-117">Not supported.</span></span>    |
|<span data-ttu-id="b955f-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="b955f-118">Application</span></span> | <span data-ttu-id="b955f-119">Group.Read.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b955f-119">Group.Read.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b955f-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b955f-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="b955f-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="b955f-121">Optional query parameters</span></span>
<span data-ttu-id="b955f-122">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="b955f-122">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="b955f-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="b955f-123">Request headers</span></span>
| <span data-ttu-id="b955f-124">名称</span><span class="sxs-lookup"><span data-stu-id="b955f-124">Name</span></span>       | <span data-ttu-id="b955f-125">类型</span><span class="sxs-lookup"><span data-stu-id="b955f-125">Type</span></span> | <span data-ttu-id="b955f-126">说明</span><span class="sxs-lookup"><span data-stu-id="b955f-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="b955f-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="b955f-127">Authorization</span></span>  | <span data-ttu-id="b955f-128">string</span><span class="sxs-lookup"><span data-stu-id="b955f-128">string</span></span>  | <span data-ttu-id="b955f-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b955f-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b955f-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="b955f-131">Request body</span></span>
<span data-ttu-id="b955f-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b955f-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b955f-133">响应</span><span class="sxs-lookup"><span data-stu-id="b955f-133">Response</span></span>
<span data-ttu-id="b955f-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b955f-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b955f-135">示例</span><span class="sxs-lookup"><span data-stu-id="b955f-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="b955f-136">请求</span><span class="sxs-lookup"><span data-stu-id="b955f-136">Request</span></span>

<span data-ttu-id="b955f-137">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b955f-137">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/groups/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="b955f-138">响应</span><span class="sxs-lookup"><span data-stu-id="b955f-138">Response</span></span>

<span data-ttu-id="b955f-139">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b955f-139">The following is an example of the response.</span></span>
><span data-ttu-id="b955f-140">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="b955f-140">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="b955f-141">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b955f-141">All the properties will be returned from an actual call.</span></span>
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->