---
title: 列表用户可传递 memberOf
description: 获取组、 目录角色和管理单元的用户的成员。 此 API 请求是可传递，，，也将返回用户是嵌套的成员的所有组。
localization_priority: Normal
ms.openlocfilehash: eadb9722bc323ea056d015ac15c8aed975306eee
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27887911"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="bf0dd-104">列表用户可传递 memberOf</span><span class="sxs-lookup"><span data-stu-id="bf0dd-104">List user transitive memberOf</span></span>

> <span data-ttu-id="bf0dd-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="bf0dd-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="bf0dd-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="bf0dd-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="bf0dd-107">获取组、 目录角色和管理单元的用户的成员。</span><span class="sxs-lookup"><span data-stu-id="bf0dd-107">Get groups, directory roles and administrative units that the user is a member of.</span></span> <span data-ttu-id="bf0dd-108">此 API 请求是可传递，，，也将返回用户是嵌套的成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="bf0dd-108">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="bf0dd-109">权限</span><span class="sxs-lookup"><span data-stu-id="bf0dd-109">Permissions</span></span>

<span data-ttu-id="bf0dd-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bf0dd-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bf0dd-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="bf0dd-112">Permission type</span></span>      | <span data-ttu-id="bf0dd-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bf0dd-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="bf0dd-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bf0dd-114">Delegated (work or school account)</span></span> | <span data-ttu-id="bf0dd-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="bf0dd-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="bf0dd-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bf0dd-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="bf0dd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="bf0dd-117">Not supported.</span></span>    |
|<span data-ttu-id="bf0dd-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="bf0dd-118">Application</span></span> | <span data-ttu-id="bf0dd-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bf0dd-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="bf0dd-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bf0dd-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="bf0dd-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="bf0dd-121">Optional query parameters</span></span>

<span data-ttu-id="bf0dd-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="bf0dd-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="bf0dd-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="bf0dd-123">Request headers</span></span>

| <span data-ttu-id="bf0dd-124">标头</span><span class="sxs-lookup"><span data-stu-id="bf0dd-124">Header</span></span>       | <span data-ttu-id="bf0dd-125">值</span><span class="sxs-lookup"><span data-stu-id="bf0dd-125">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="bf0dd-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="bf0dd-126">Authorization</span></span>  | <span data-ttu-id="bf0dd-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="bf0dd-p105">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="bf0dd-129">Accept</span><span class="sxs-lookup"><span data-stu-id="bf0dd-129">Accept</span></span>  | <span data-ttu-id="bf0dd-130">application/json</span><span class="sxs-lookup"><span data-stu-id="bf0dd-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bf0dd-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="bf0dd-131">Request body</span></span>

<span data-ttu-id="bf0dd-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bf0dd-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bf0dd-133">响应</span><span class="sxs-lookup"><span data-stu-id="bf0dd-133">Response</span></span>

<span data-ttu-id="bf0dd-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="bf0dd-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bf0dd-135">示例</span><span class="sxs-lookup"><span data-stu-id="bf0dd-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="bf0dd-136">请求</span><span class="sxs-lookup"><span data-stu-id="bf0dd-136">Request</span></span>

<span data-ttu-id="bf0dd-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bf0dd-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/me/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="bf0dd-138">响应</span><span class="sxs-lookup"><span data-stu-id="bf0dd-138">Response</span></span>

<span data-ttu-id="bf0dd-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bf0dd-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
