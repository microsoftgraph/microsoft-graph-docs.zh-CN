---
title: 列表 servicePrincipal memberOf
description: 获取主体此服务是直接成员的组和目录角色。 此操作是不可传递的。
ms.openlocfilehash: 54376d80fdb3cc5084ac19aa331b94d40ac3103f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27049539"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="ca270-104">列表 servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="ca270-104">List servicePrincipal memberOf</span></span>

> <span data-ttu-id="ca270-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ca270-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca270-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ca270-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca270-107">获取主体此服务是直接成员的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="ca270-107">Get the groups and directory roles that this service principal is a direct member of.</span></span> <span data-ttu-id="ca270-108">此操作是不可传递的。</span><span class="sxs-lookup"><span data-stu-id="ca270-108">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="ca270-109">权限</span><span class="sxs-lookup"><span data-stu-id="ca270-109">Permissions</span></span>

<span data-ttu-id="ca270-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ca270-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca270-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca270-112">Permission type</span></span>      | <span data-ttu-id="ca270-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ca270-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ca270-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca270-114">Delegated (work or school account)</span></span> | <span data-ttu-id="ca270-115">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ca270-115">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ca270-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca270-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ca270-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca270-117">Not supported.</span></span>    |
|<span data-ttu-id="ca270-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca270-118">Application</span></span> | <span data-ttu-id="ca270-119">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca270-119">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ca270-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca270-120">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ca270-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ca270-121">Optional query parameters</span></span>

<span data-ttu-id="ca270-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ca270-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ca270-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca270-123">Request headers</span></span>
| <span data-ttu-id="ca270-124">名称</span><span class="sxs-lookup"><span data-stu-id="ca270-124">Name</span></span>       | <span data-ttu-id="ca270-125">类型</span><span class="sxs-lookup"><span data-stu-id="ca270-125">Type</span></span> | <span data-ttu-id="ca270-126">说明</span><span class="sxs-lookup"><span data-stu-id="ca270-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ca270-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca270-127">Authorization</span></span>  | <span data-ttu-id="ca270-128">string</span><span class="sxs-lookup"><span data-stu-id="ca270-128">string</span></span>  | <span data-ttu-id="ca270-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ca270-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ca270-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca270-131">Request body</span></span>
<span data-ttu-id="ca270-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ca270-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ca270-133">响应</span><span class="sxs-lookup"><span data-stu-id="ca270-133">Response</span></span>

<span data-ttu-id="ca270-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ca270-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca270-135">示例</span><span class="sxs-lookup"><span data-stu-id="ca270-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="ca270-136">请求</span><span class="sxs-lookup"><span data-stu-id="ca270-136">Request</span></span>

<span data-ttu-id="ca270-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca270-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="ca270-138">响应</span><span class="sxs-lookup"><span data-stu-id="ca270-138">Response</span></span>

<span data-ttu-id="ca270-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca270-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->