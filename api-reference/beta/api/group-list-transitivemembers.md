---
title: 可传递列表组的成员
description: 获取组的成员的列表。 一组可将用户、 联系人、 设备、 服务主体和其他组作为成员。 此操作可传递，也将返回所有嵌套成员一个平面列表。
localization_priority: Normal
ms.openlocfilehash: a89894bf17d12f7cd23350f466e9e1272fa0cb6a
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27892216"
---
# <a name="list-group-transitive-members"></a><span data-ttu-id="cf657-105">可传递列表组的成员</span><span class="sxs-lookup"><span data-stu-id="cf657-105">List group transitive members</span></span>

> <span data-ttu-id="cf657-106">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cf657-106">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cf657-107">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cf657-107">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="cf657-108">获取组的成员的列表。</span><span class="sxs-lookup"><span data-stu-id="cf657-108">Get a list of the group's members.</span></span> <span data-ttu-id="cf657-109">一组可将用户、 联系人、 设备、 服务主体和其他组作为成员。</span><span class="sxs-lookup"><span data-stu-id="cf657-109">A group can have users, contacts, devices, service principals and other groups as members.</span></span> <span data-ttu-id="cf657-110">此操作可传递，也将返回所有嵌套成员一个平面列表。</span><span class="sxs-lookup"><span data-stu-id="cf657-110">This operation is transitive and will also return a flat list of all nested members.</span></span>

## <a name="permissions"></a><span data-ttu-id="cf657-111">权限</span><span class="sxs-lookup"><span data-stu-id="cf657-111">Permissions</span></span>

<span data-ttu-id="cf657-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cf657-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf657-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf657-114">Permission type</span></span>      | <span data-ttu-id="cf657-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cf657-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cf657-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf657-116">Delegated (work or school account)</span></span> | <span data-ttu-id="cf657-117">Directory.Read.All，Directory.AccessAsUser.All，User.ReadBasic.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf657-117">Directory.Read.All, Directory.AccessAsUser.All, User.ReadBasic.All, User.Read.All</span></span>    |
|<span data-ttu-id="cf657-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf657-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cf657-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf657-119">Not supported.</span></span>    |
|<span data-ttu-id="cf657-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf657-120">Application</span></span> | <span data-ttu-id="cf657-121">Directory.Read.All User.Read.All</span><span class="sxs-lookup"><span data-stu-id="cf657-121">Directory.Read.All, User.Read.All</span></span> |

> <span data-ttu-id="cf657-122">注意： 列表中隐藏成员资格组的成员，则 Member.Read.Hidden 权限是必需。</span><span class="sxs-lookup"><span data-stu-id="cf657-122">Note: To list the members of a hidden membership group, the Member.Read.Hidden permission is required.</span></span>

## <a name="http-request"></a><span data-ttu-id="cf657-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf657-123">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /groups/{id}/transitiveMembers
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cf657-124">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cf657-124">Optional query parameters</span></span>

<span data-ttu-id="cf657-125">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cf657-125">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cf657-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf657-126">Request headers</span></span>

| <span data-ttu-id="cf657-127">名称</span><span class="sxs-lookup"><span data-stu-id="cf657-127">Name</span></span>       | <span data-ttu-id="cf657-128">类型</span><span class="sxs-lookup"><span data-stu-id="cf657-128">Type</span></span> | <span data-ttu-id="cf657-129">说明</span><span class="sxs-lookup"><span data-stu-id="cf657-129">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="cf657-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf657-130">Authorization</span></span>  | <span data-ttu-id="cf657-131">string</span><span class="sxs-lookup"><span data-stu-id="cf657-131">string</span></span>  | <span data-ttu-id="cf657-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cf657-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="cf657-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf657-134">Request body</span></span>

<span data-ttu-id="cf657-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cf657-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf657-136">响应</span><span class="sxs-lookup"><span data-stu-id="cf657-136">Response</span></span>

<span data-ttu-id="cf657-137">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cf657-137">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cf657-138">示例</span><span class="sxs-lookup"><span data-stu-id="cf657-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="cf657-139">请求</span><span class="sxs-lookup"><span data-stu-id="cf657-139">Request</span></span>

<span data-ttu-id="cf657-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="cf657-140">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_group_transitivemembers"
}-->

```http
GET https://graph.microsoft.com/beta/groups/{id}/transitiveMembers
```

### <a name="response"></a><span data-ttu-id="cf657-141">响应</span><span class="sxs-lookup"><span data-stu-id="cf657-141">Response</span></span>

<span data-ttu-id="cf657-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="cf657-142">The following is an example of the response.</span></span>
><span data-ttu-id="cf657-143">**注意：** 可能为便于阅读缩短如下所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cf657-143">**Note:** The response object shown here might be shortened for readability.</span></span> <span data-ttu-id="cf657-144">所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="cf657-144">All the properties will be returned from an actual call.</span></span>
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
    "@odata.type": "#microsoft.graph.user",
    {
      "businessPhones": [
        "businessPhones-value"
      ],
      "displayName": "displayName-value",
      "givenName": "givenName-value",
      "jobTitle": "jobTitle-value",
      "mail": "mail-value",
      "mobilePhone": "mobilePhone-value",
      "officeLocation": "officeLocation-value",
      "preferredLanguage": "preferredLanguage-value",
      "surname": "surname-value",
      "userPrincipalName": "userPrincipalName-value",
      "id": "id-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List transitive group members",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
