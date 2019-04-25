---
title: 列出 servicePrincipal memberOf
description: 获取此服务主体是其直接成员的组和目录角色。 此操作不可传递。
localization_priority: Normal
ms.openlocfilehash: 84f82f632ef9c8f7e933d024f4d7df958415f140
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32537469"
---
# <a name="list-serviceprincipal-memberof"></a><span data-ttu-id="0306e-104">列出 servicePrincipal memberOf</span><span class="sxs-lookup"><span data-stu-id="0306e-104">List servicePrincipal memberOf</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0306e-105">获取此服务主体是其直接成员的组和目录角色。</span><span class="sxs-lookup"><span data-stu-id="0306e-105">Get the groups and directory roles that this service principal is a direct member of.</span></span> <span data-ttu-id="0306e-106">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="0306e-106">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="0306e-107">权限</span><span class="sxs-lookup"><span data-stu-id="0306e-107">Permissions</span></span>

<span data-ttu-id="0306e-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0306e-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0306e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0306e-110">Permission type</span></span>      | <span data-ttu-id="0306e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0306e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0306e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0306e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0306e-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0306e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0306e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0306e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0306e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0306e-115">Not supported.</span></span>    |
|<span data-ttu-id="0306e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0306e-116">Application</span></span> | <span data-ttu-id="0306e-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0306e-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0306e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0306e-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/memberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0306e-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0306e-119">Optional query parameters</span></span>

<span data-ttu-id="0306e-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0306e-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0306e-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0306e-121">Request headers</span></span>
| <span data-ttu-id="0306e-122">名称</span><span class="sxs-lookup"><span data-stu-id="0306e-122">Name</span></span>       | <span data-ttu-id="0306e-123">类型</span><span class="sxs-lookup"><span data-stu-id="0306e-123">Type</span></span> | <span data-ttu-id="0306e-124">说明</span><span class="sxs-lookup"><span data-stu-id="0306e-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0306e-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="0306e-125">Authorization</span></span>  | <span data-ttu-id="0306e-126">string</span><span class="sxs-lookup"><span data-stu-id="0306e-126">string</span></span>  | <span data-ttu-id="0306e-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0306e-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0306e-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="0306e-129">Request body</span></span>
<span data-ttu-id="0306e-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0306e-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0306e-131">响应</span><span class="sxs-lookup"><span data-stu-id="0306e-131">Response</span></span>

<span data-ttu-id="0306e-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0306e-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0306e-133">示例</span><span class="sxs-lookup"><span data-stu-id="0306e-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0306e-134">请求</span><span class="sxs-lookup"><span data-stu-id="0306e-134">Request</span></span>

<span data-ttu-id="0306e-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0306e-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_serviceprincipal_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="0306e-136">响应</span><span class="sxs-lookup"><span data-stu-id="0306e-136">Response</span></span>

<span data-ttu-id="0306e-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0306e-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
