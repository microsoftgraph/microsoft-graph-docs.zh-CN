---
title: 列表组可传递 memberOf
description: 获取组和管理单元的组的成员。  此操作可传递，也将包括此组是嵌套的成员的所有组。 与不同获取用户的 Office 365 组，这将返回所有类型的组，而不仅仅是 Office 365 组。
ms.openlocfilehash: e622ee484a4070560c38528bccfe7f12e2172d54
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043946"
---
# <a name="list-group-transitive-memberof"></a><span data-ttu-id="68ebf-105">列表组可传递 memberOf</span><span class="sxs-lookup"><span data-stu-id="68ebf-105">List group transitive memberOf</span></span>

> <span data-ttu-id="68ebf-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="68ebf-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="68ebf-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="68ebf-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="68ebf-108">获取组和管理单元的组的成员。</span><span class="sxs-lookup"><span data-stu-id="68ebf-108">Get groups and administrative units that the group is a member of.</span></span>  <span data-ttu-id="68ebf-109">此操作可传递，也将包括此组是嵌套的成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="68ebf-109">This operation is transitive and will also include all groups that this groups is a nested member of.</span></span> <span data-ttu-id="68ebf-110">与不同获取用户的 Office 365 组，这将返回所有类型的组，而不仅仅是 Office 365 组。</span><span class="sxs-lookup"><span data-stu-id="68ebf-110">Unlike getting a user's Office 365 Groups, this returns all types of groups, not just Office 365 Groups.</span></span>

## <a name="permissions"></a><span data-ttu-id="68ebf-111">权限</span><span class="sxs-lookup"><span data-stu-id="68ebf-111">Permissions</span></span>

<span data-ttu-id="68ebf-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="68ebf-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="68ebf-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="68ebf-114">Permission type</span></span>      | <span data-ttu-id="68ebf-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="68ebf-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="68ebf-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="68ebf-116">Delegated (work or school account)</span></span> | <span data-ttu-id="68ebf-117">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="68ebf-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="68ebf-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="68ebf-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="68ebf-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="68ebf-119">Not supported.</span></span>    |
|<span data-ttu-id="68ebf-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="68ebf-120">Application</span></span> | <span data-ttu-id="68ebf-121">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="68ebf-121">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="68ebf-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="68ebf-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /groups/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="68ebf-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="68ebf-123">Optional query parameters</span></span>
<span data-ttu-id="68ebf-124">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="68ebf-124">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="68ebf-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="68ebf-125">Request headers</span></span>
| <span data-ttu-id="68ebf-126">名称</span><span class="sxs-lookup"><span data-stu-id="68ebf-126">Name</span></span>       | <span data-ttu-id="68ebf-127">类型</span><span class="sxs-lookup"><span data-stu-id="68ebf-127">Type</span></span> | <span data-ttu-id="68ebf-128">说明</span><span class="sxs-lookup"><span data-stu-id="68ebf-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="68ebf-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="68ebf-129">Authorization</span></span>  | <span data-ttu-id="68ebf-130">string</span><span class="sxs-lookup"><span data-stu-id="68ebf-130">string</span></span>  | <span data-ttu-id="68ebf-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="68ebf-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="68ebf-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="68ebf-133">Request body</span></span>
<span data-ttu-id="68ebf-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="68ebf-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="68ebf-135">响应</span><span class="sxs-lookup"><span data-stu-id="68ebf-135">Response</span></span>
<span data-ttu-id="68ebf-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="68ebf-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="68ebf-137">示例</span><span class="sxs-lookup"><span data-stu-id="68ebf-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="68ebf-138">请求</span><span class="sxs-lookup"><span data-stu-id="68ebf-138">Request</span></span>
<span data-ttu-id="68ebf-139">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="68ebf-139">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="68ebf-140">响应</span><span class="sxs-lookup"><span data-stu-id="68ebf-140">Response</span></span>

<span data-ttu-id="68ebf-141">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="68ebf-141">The following is an example of the response.</span></span>
><span data-ttu-id="68ebf-142">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="68ebf-142">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="68ebf-143">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="68ebf-143">All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.directoryObject",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.group",
      "id": "id-value",
      "createdDateTime": null,
      "description": "All users at the company",
      "displayName": "All Users",
      "groupTypes": [],
      "mailEnabled": false,
      "securityEnabled": true,
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List group transitive memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->