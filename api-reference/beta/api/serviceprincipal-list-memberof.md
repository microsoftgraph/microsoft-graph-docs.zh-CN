---
title: 列表 servicePrincipal memberOf
description: 获取主体此服务是直接成员的组和目录角色。 此操作是不可传递的。
localization_priority: Normal
ms.openlocfilehash: 84f82f632ef9c8f7e933d024f4d7df958415f140
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29524203"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="8bda4-104">列表 servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="8bda4-104">List servicePrincipal memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="8bda4-105">获取主体此服务是直接成员的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="8bda4-105">Get the groups and directory roles that this service principal is a direct member of.</span></span> <span data-ttu-id="8bda4-106">此操作是不可传递的。</span><span class="sxs-lookup"><span data-stu-id="8bda4-106">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="8bda4-107">权限</span><span class="sxs-lookup"><span data-stu-id="8bda4-107">Permissions</span></span>

<span data-ttu-id="8bda4-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8bda4-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8bda4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8bda4-110">Permission type</span></span>      | <span data-ttu-id="8bda4-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="8bda4-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="8bda4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8bda4-112">Delegated (work or school account)</span></span> | <span data-ttu-id="8bda4-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="8bda4-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="8bda4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8bda4-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="8bda4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8bda4-115">Not supported.</span></span>    |
|<span data-ttu-id="8bda4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8bda4-116">Application</span></span> | <span data-ttu-id="8bda4-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8bda4-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="8bda4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8bda4-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="8bda4-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="8bda4-119">Optional query parameters</span></span>

<span data-ttu-id="8bda4-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="8bda4-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="8bda4-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="8bda4-121">Request headers</span></span>
| <span data-ttu-id="8bda4-122">名称</span><span class="sxs-lookup"><span data-stu-id="8bda4-122">Name</span></span>       | <span data-ttu-id="8bda4-123">类型</span><span class="sxs-lookup"><span data-stu-id="8bda4-123">Type</span></span> | <span data-ttu-id="8bda4-124">说明</span><span class="sxs-lookup"><span data-stu-id="8bda4-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="8bda4-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="8bda4-125">Authorization</span></span>  | <span data-ttu-id="8bda4-126">string</span><span class="sxs-lookup"><span data-stu-id="8bda4-126">string</span></span>  | <span data-ttu-id="8bda4-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="8bda4-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="8bda4-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="8bda4-129">Request body</span></span>
<span data-ttu-id="8bda4-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="8bda4-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="8bda4-131">响应</span><span class="sxs-lookup"><span data-stu-id="8bda4-131">Response</span></span>

<span data-ttu-id="8bda4-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="8bda4-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8bda4-133">示例</span><span class="sxs-lookup"><span data-stu-id="8bda4-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="8bda4-134">请求</span><span class="sxs-lookup"><span data-stu-id="8bda4-134">Request</span></span>

<span data-ttu-id="8bda4-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8bda4-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="8bda4-136">响应</span><span class="sxs-lookup"><span data-stu-id="8bda4-136">Response</span></span>

<span data-ttu-id="8bda4-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8bda4-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List servicePrincipal memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/serviceprincipal-list-memberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
