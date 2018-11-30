---
title: 列表 privilegedRoles
description: 检索 privilegedRole 对象的列表。
ms.openlocfilehash: 6800096f36e1fb8237216cf9ea708b3b20ff21ae
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044266"
---
# <a name="list-privilegedroles"></a><span data-ttu-id="d1dd6-103">列表 privilegedRoles</span><span class="sxs-lookup"><span data-stu-id="d1dd6-103">List privilegedRoles</span></span>

> <span data-ttu-id="d1dd6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d1dd6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d1dd6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d1dd6-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d1dd6-106">检索[privilegedRole](../resources/privilegedrole.md)对象的列表。</span><span class="sxs-lookup"><span data-stu-id="d1dd6-106">Retrieve a list of [privilegedRole](../resources/privilegedrole.md) objects.</span></span>

<span data-ttu-id="d1dd6-107">若要筛选查询的结果，请使用标准 OData ``$filter`` Uri 中的表达式。</span><span class="sxs-lookup"><span data-stu-id="d1dd6-107">To filter the results from the query, use the standard OData ``$filter`` expressions in the URIs.</span></span>
## <a name="permissions"></a><span data-ttu-id="d1dd6-108">权限</span><span class="sxs-lookup"><span data-stu-id="d1dd6-108">Permissions</span></span>
<span data-ttu-id="d1dd6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d1dd6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="d1dd6-111">请求者需要拥有以下角色之一：_具有权限的角色管理员_、_全局管理员_、_安全管理员_或_安全读取器_。</span><span class="sxs-lookup"><span data-stu-id="d1dd6-111">The requestor needs to have one of the following roles: _Privileged Role Administrator_, _Global Administrator_, _Security Administrator_, or _Security Reader_.</span></span>
 

|<span data-ttu-id="d1dd6-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="d1dd6-112">Permission type</span></span>      | <span data-ttu-id="d1dd6-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d1dd6-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d1dd6-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d1dd6-114">Delegated (work or school account)</span></span> | <span data-ttu-id="d1dd6-115">Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d1dd6-115">Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d1dd6-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d1dd6-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d1dd6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1dd6-117">Not supported.</span></span>    |
|<span data-ttu-id="d1dd6-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="d1dd6-118">Application</span></span> | <span data-ttu-id="d1dd6-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="d1dd6-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="d1dd6-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d1dd6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /privilegedRoles
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d1dd6-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d1dd6-121">Optional query parameters</span></span>
<span data-ttu-id="d1dd6-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d1dd6-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d1dd6-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="d1dd6-123">Request headers</span></span>
| <span data-ttu-id="d1dd6-124">名称</span><span class="sxs-lookup"><span data-stu-id="d1dd6-124">Name</span></span>      |<span data-ttu-id="d1dd6-125">说明</span><span class="sxs-lookup"><span data-stu-id="d1dd6-125">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="d1dd6-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="d1dd6-126">Authorization</span></span>  | <span data-ttu-id="d1dd6-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d1dd6-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d1dd6-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="d1dd6-129">Request body</span></span>
<span data-ttu-id="d1dd6-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d1dd6-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d1dd6-131">响应</span><span class="sxs-lookup"><span data-stu-id="d1dd6-131">Response</span></span>

<span data-ttu-id="d1dd6-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[privilegedRole](../resources/privilegedrole.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="d1dd6-132">If successful, this method returns a `200 OK` response code and collection of [privilegedRole](../resources/privilegedrole.md) objects in the response body.</span></span>

<span data-ttu-id="d1dd6-133">请注意，需要将其注册到 PIM 租户。</span><span class="sxs-lookup"><span data-stu-id="d1dd6-133">Note that the tenant needs to be registered to PIM.</span></span> <span data-ttu-id="d1dd6-134">否则，将返回的 HTTP 403 禁止访问状态代码。</span><span class="sxs-lookup"><span data-stu-id="d1dd6-134">Otherwise, the HTTP 403 Forbidden status code will be returned.</span></span>
## <a name="example"></a><span data-ttu-id="d1dd6-135">示例</span><span class="sxs-lookup"><span data-stu-id="d1dd6-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d1dd6-136">请求</span><span class="sxs-lookup"><span data-stu-id="d1dd6-136">Request</span></span>
<span data-ttu-id="d1dd6-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d1dd6-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_privilegedroles"
}-->
```http
GET https://graph.microsoft.com/beta/privilegedRoles
```
##### <a name="response"></a><span data-ttu-id="d1dd6-138">响应</span><span class="sxs-lookup"><span data-stu-id="d1dd6-138">Response</span></span>
<span data-ttu-id="d1dd6-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d1dd6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List privilegedRoles",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->