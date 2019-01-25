---
title: 获取 privilegedRole
description: '检索的属性和 privilegedRole 对象的关系。 '
localization_priority: Normal
ms.openlocfilehash: 54fbf8bab03003a03f607bc540414190573a6158
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29521640"
---
# <a name="get-privilegedrole"></a><span data-ttu-id="6a67e-103">获取 privilegedRole</span><span class="sxs-lookup"><span data-stu-id="6a67e-103">Get privilegedRole</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6a67e-104">检索的属性和[privilegedRole](../resources/privilegedrole.md)对象的关系。</span><span class="sxs-lookup"><span data-stu-id="6a67e-104">Retrieve the properties and relationships of [privilegedRole](../resources/privilegedrole.md) object.</span></span> 

## <a name="permissions"></a><span data-ttu-id="6a67e-105">权限</span><span class="sxs-lookup"><span data-stu-id="6a67e-105">Permissions</span></span>
<span data-ttu-id="6a67e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a67e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="6a67e-108">请求者需要拥有以下角色之一：_具有权限的角色管理员_、_全局管理员_、_安全管理员_或_安全读取器_。</span><span class="sxs-lookup"><span data-stu-id="6a67e-108">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="6a67e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a67e-109">Permission type</span></span>      | <span data-ttu-id="6a67e-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6a67e-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6a67e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a67e-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6a67e-112">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="6a67e-112">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="6a67e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a67e-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6a67e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a67e-114">Not supported.</span></span>    |
|<span data-ttu-id="6a67e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a67e-115">Application</span></span> | <span data-ttu-id="6a67e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a67e-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="6a67e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a67e-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles/{id}
GET /privilegedRoleAssignments/{id}/roleInfo
```
## <a name="optional-query-parameters"></a><span data-ttu-id="6a67e-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6a67e-118">Optional query parameters</span></span>
<span data-ttu-id="6a67e-119">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="6a67e-119">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="6a67e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a67e-120">Request headers</span></span>
| <span data-ttu-id="6a67e-121">名称</span><span class="sxs-lookup"><span data-stu-id="6a67e-121">Name</span></span>      |<span data-ttu-id="6a67e-122">说明</span><span class="sxs-lookup"><span data-stu-id="6a67e-122">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="6a67e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a67e-123">Authorization</span></span>  | <span data-ttu-id="6a67e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6a67e-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="6a67e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a67e-126">Request body</span></span>
<span data-ttu-id="6a67e-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6a67e-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6a67e-128">响应</span><span class="sxs-lookup"><span data-stu-id="6a67e-128">Response</span></span>

<span data-ttu-id="6a67e-129">如果成功，此方法返回`200 OK`响应正文中的响应代码和[privilegedRole](../resources/privilegedrole.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6a67e-129">If successful, this method returns a `200 OK` response code and [privilegedRole](../resources/privilegedrole.md) object in the response body.</span></span>

<span data-ttu-id="6a67e-130">请注意，需要将其注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="6a67e-130">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="6a67e-131">否则，将返回的 HTTP 403 禁止访问状态代码。</span><span class="sxs-lookup"><span data-stu-id="6a67e-131">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="6a67e-132">示例</span><span class="sxs-lookup"><span data-stu-id="6a67e-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="6a67e-133">请求</span><span class="sxs-lookup"><span data-stu-id="6a67e-133">Request</span></span>
<span data-ttu-id="6a67e-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a67e-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedrole"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles/{id}
```
##### <a name="response"></a><span data-ttu-id="6a67e-135">响应</span><span class="sxs-lookup"><span data-stu-id="6a67e-135">Response</span></span>
<span data-ttu-id="6a67e-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6a67e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 46

{
  "id": "id-value",
  "name": "name-value"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Get privilegedRole",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-get.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
