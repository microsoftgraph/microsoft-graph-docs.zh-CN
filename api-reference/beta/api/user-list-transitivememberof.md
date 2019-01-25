---
title: 列表用户可传递 memberOf
description: 获取组、 目录角色和管理单元的用户的成员。 此 API 请求是可传递，，，也将返回用户是嵌套的成员的所有组。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b0681196b994e9a0c88a2b2d05e25e3166a5242f
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528863"
---
# <a name="list-user-transitive-memberof"></a><span data-ttu-id="0ce58-104">列表用户可传递 memberOf</span><span class="sxs-lookup"><span data-stu-id="0ce58-104">List user transitive memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ce58-105">获取组、 目录角色和管理单元的用户的成员。</span><span class="sxs-lookup"><span data-stu-id="0ce58-105">Get groups, directory roles and administrative units that the user is a member of.</span></span> <span data-ttu-id="0ce58-106">此 API 请求是可传递，，，也将返回用户是嵌套的成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="0ce58-106">This API request is transitive, and will also return all groups the user is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ce58-107">权限</span><span class="sxs-lookup"><span data-stu-id="0ce58-107">Permissions</span></span>

<span data-ttu-id="0ce58-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ce58-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ce58-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ce58-110">Permission type</span></span>      | <span data-ttu-id="0ce58-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ce58-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ce58-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ce58-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0ce58-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0ce58-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0ce58-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ce58-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ce58-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ce58-115">Not supported.</span></span>    |
|<span data-ttu-id="0ce58-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ce58-116">Application</span></span> | <span data-ttu-id="0ce58-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0ce58-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ce58-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ce58-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /users/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0ce58-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0ce58-119">Optional query parameters</span></span>

<span data-ttu-id="0ce58-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0ce58-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0ce58-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ce58-121">Request headers</span></span>

| <span data-ttu-id="0ce58-122">标头</span><span class="sxs-lookup"><span data-stu-id="0ce58-122">Header</span></span>       | <span data-ttu-id="0ce58-123">值</span><span class="sxs-lookup"><span data-stu-id="0ce58-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0ce58-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ce58-124">Authorization</span></span>  | <span data-ttu-id="0ce58-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ce58-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0ce58-127">Accept</span><span class="sxs-lookup"><span data-stu-id="0ce58-127">Accept</span></span>  | <span data-ttu-id="0ce58-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0ce58-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0ce58-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ce58-129">Request body</span></span>

<span data-ttu-id="0ce58-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0ce58-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ce58-131">响应</span><span class="sxs-lookup"><span data-stu-id="0ce58-131">Response</span></span>

<span data-ttu-id="0ce58-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0ce58-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0ce58-133">示例</span><span class="sxs-lookup"><span data-stu-id="0ce58-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0ce58-134">请求</span><span class="sxs-lookup"><span data-stu-id="0ce58-134">Request</span></span>

<span data-ttu-id="0ce58-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ce58-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/me/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="0ce58-136">响应</span><span class="sxs-lookup"><span data-stu-id="0ce58-136">Response</span></span>

<span data-ttu-id="0ce58-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0ce58-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "List transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/user-list-transitivememberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
