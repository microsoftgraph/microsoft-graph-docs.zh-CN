---
title: 列出成员
description: 检索分配给目录角色的用户列表。只能将用户分配给目录角色。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 4365408309a8d87387da76695257207f03bf5ce5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519575"
---
# <a name="list-members"></a><span data-ttu-id="19ee2-104">列出成员</span><span class="sxs-lookup"><span data-stu-id="19ee2-104">List members</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="19ee2-p102">检索分配给目录角色的用户列表。只能将用户分配给目录角色。</span><span class="sxs-lookup"><span data-stu-id="19ee2-p102">Retrieve a list of the users that are assigned to the directory role.  Only users can be assigned to a directory role.</span></span>
## <a name="permissions"></a><span data-ttu-id="19ee2-107">权限</span><span class="sxs-lookup"><span data-stu-id="19ee2-107">Permissions</span></span>
<span data-ttu-id="19ee2-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19ee2-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="19ee2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="19ee2-110">Permission type</span></span>      | <span data-ttu-id="19ee2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="19ee2-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="19ee2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19ee2-112">Delegated (work or school account)</span></span> | <span data-ttu-id="19ee2-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="19ee2-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="19ee2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19ee2-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="19ee2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="19ee2-115">Not supported.</span></span>    |
|<span data-ttu-id="19ee2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="19ee2-116">Application</span></span> | <span data-ttu-id="19ee2-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19ee2-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="19ee2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19ee2-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /directoryRoles/{id}/members
```
## <a name="optional-query-parameters"></a><span data-ttu-id="19ee2-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="19ee2-119">Optional query parameters</span></span>
<span data-ttu-id="19ee2-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="19ee2-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="19ee2-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="19ee2-121">Request headers</span></span>
| <span data-ttu-id="19ee2-122">名称</span><span class="sxs-lookup"><span data-stu-id="19ee2-122">Name</span></span>       | <span data-ttu-id="19ee2-123">类型</span><span class="sxs-lookup"><span data-stu-id="19ee2-123">Type</span></span> | <span data-ttu-id="19ee2-124">说明</span><span class="sxs-lookup"><span data-stu-id="19ee2-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="19ee2-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="19ee2-125">Authorization</span></span>  | <span data-ttu-id="19ee2-126">string</span><span class="sxs-lookup"><span data-stu-id="19ee2-126">string</span></span>  | <span data-ttu-id="19ee2-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="19ee2-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="19ee2-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="19ee2-129">Request body</span></span>
<span data-ttu-id="19ee2-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="19ee2-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="19ee2-131">响应</span><span class="sxs-lookup"><span data-stu-id="19ee2-131">Response</span></span>

<span data-ttu-id="19ee2-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="19ee2-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="19ee2-133">示例</span><span class="sxs-lookup"><span data-stu-id="19ee2-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="19ee2-134">请求</span><span class="sxs-lookup"><span data-stu-id="19ee2-134">Request</span></span>
<span data-ttu-id="19ee2-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="19ee2-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_members"
}-->
```http
GET https://graph.microsoft.com/beta/directoryRoles/{id}/members
```
##### <a name="response"></a><span data-ttu-id="19ee2-136">响应</span><span class="sxs-lookup"><span data-stu-id="19ee2-136">Response</span></span>
<span data-ttu-id="19ee2-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19ee2-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List members",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/directoryrole-list-members.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
