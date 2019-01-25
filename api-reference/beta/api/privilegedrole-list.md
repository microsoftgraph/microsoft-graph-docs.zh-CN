---
title: 列表 privilegedRoles
description: 检索 privilegedRole 对象的列表。
localization_priority: Normal
ms.openlocfilehash: d954cedbaf4b164fe0649a3565ea0212d148c322
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29518077"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="7847a-103">列表 privilegedRoles</span><span class="sxs-lookup"><span data-stu-id="7847a-103">List privilegedRoles</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7847a-104">检索[privilegedRole](../resources/privilegedrole.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="7847a-104">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="7847a-105">若要筛选查询的结果，请使用标准 OData ``$filter`` Uri 中的表达式。</span><span class="sxs-lookup"><span data-stu-id="7847a-105">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="7847a-106">权限</span><span class="sxs-lookup"><span data-stu-id="7847a-106">Permissions</span></span>
<span data-ttu-id="7847a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7847a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7847a-109">请求者需要拥有以下角色之一：_具有权限的角色管理员_、_全局管理员_、_安全管理员_或_安全读取器_。</span><span class="sxs-lookup"><span data-stu-id="7847a-109">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="7847a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="7847a-110">Permission type</span></span>      | <span data-ttu-id="7847a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7847a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7847a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7847a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="7847a-113">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="7847a-113">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="7847a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7847a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7847a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7847a-115">Not supported.</span></span>    |
|<span data-ttu-id="7847a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="7847a-116">Application</span></span> | <span data-ttu-id="7847a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7847a-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7847a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7847a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="7847a-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="7847a-119">Optional query parameters</span></span>
<span data-ttu-id="7847a-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="7847a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="7847a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="7847a-121">Request headers</span></span>
| <span data-ttu-id="7847a-122">名称</span><span class="sxs-lookup"><span data-stu-id="7847a-122">Name</span></span>      |<span data-ttu-id="7847a-123">说明</span><span class="sxs-lookup"><span data-stu-id="7847a-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="7847a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="7847a-124">Authorization</span></span>  | <span data-ttu-id="7847a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7847a-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7847a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7847a-127">Request body</span></span>
<span data-ttu-id="7847a-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7847a-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7847a-129">响应</span><span class="sxs-lookup"><span data-stu-id="7847a-129">Response</span></span>

<span data-ttu-id="7847a-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[privilegedRole](../resources/privilegedrole.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="7847a-130">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="7847a-131">请注意，需要将其注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="7847a-131">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="7847a-132">否则，将返回的 HTTP 403 禁止访问状态代码。</span><span class="sxs-lookup"><span data-stu-id="7847a-132">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="7847a-133">示例</span><span class="sxs-lookup"><span data-stu-id="7847a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7847a-134">请求</span><span class="sxs-lookup"><span data-stu-id="7847a-134">Request</span></span>
<span data-ttu-id="7847a-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7847a-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles
```
##### <a name="response"></a><span data-ttu-id="7847a-136">响应</span><span class="sxs-lookup"><span data-stu-id="7847a-136">Response</span></span>
<span data-ttu-id="7847a-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7847a-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.privilegedRole",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 83

{
  "value": [
    {
      "id": "id-value",
      "name": "name-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List privilegedRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/privilegedrole-list.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
