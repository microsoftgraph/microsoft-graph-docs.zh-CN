---
title: servicePrincipal： 列表 appRoleAssignments
description: 检索 approleassignment 对象的列表。
localization_priority: Normal
ms.openlocfilehash: 072060fe1cb7c7286632216c619bb064004baf7b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27864153"
---
# <a name="serviceprincipal-list-approleassignments"></a><span data-ttu-id="01920-103">servicePrincipal： 列表 appRoleAssignments</span><span class="sxs-lookup"><span data-stu-id="01920-103">servicePrincipal: List appRoleAssignments</span></span>

> <span data-ttu-id="01920-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="01920-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="01920-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="01920-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="01920-106">检索 approleassignment 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="01920-106">Retrieve a list of approleassignment objects.</span></span>

## <a name="permissions"></a><span data-ttu-id="01920-107">权限</span><span class="sxs-lookup"><span data-stu-id="01920-107">Permissions</span></span>
<span data-ttu-id="01920-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="01920-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="01920-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="01920-110">Permission type</span></span>      | <span data-ttu-id="01920-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="01920-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="01920-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="01920-112">Delegated (work or school account)</span></span> | <span data-ttu-id="01920-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="01920-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="01920-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="01920-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="01920-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="01920-115">Not supported.</span></span>    |
|<span data-ttu-id="01920-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="01920-116">Application</span></span> | <span data-ttu-id="01920-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="01920-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="01920-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="01920-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /servicePrincipals/{id}/appRoleAssignments
```
## <a name="optional-query-parameters"></a><span data-ttu-id="01920-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="01920-119">Optional query parameters</span></span>
<span data-ttu-id="01920-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="01920-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="01920-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="01920-121">Request headers</span></span>
| <span data-ttu-id="01920-122">名称</span><span class="sxs-lookup"><span data-stu-id="01920-122">Name</span></span>       | <span data-ttu-id="01920-123">类型</span><span class="sxs-lookup"><span data-stu-id="01920-123">Type</span></span> | <span data-ttu-id="01920-124">说明</span><span class="sxs-lookup"><span data-stu-id="01920-124">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="01920-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="01920-125">Authorization</span></span>  | <span data-ttu-id="01920-126">string</span><span class="sxs-lookup"><span data-stu-id="01920-126">string</span></span>  | <span data-ttu-id="01920-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="01920-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="01920-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="01920-129">Request body</span></span>
<span data-ttu-id="01920-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="01920-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="01920-131">响应</span><span class="sxs-lookup"><span data-stu-id="01920-131">Response</span></span>

<span data-ttu-id="01920-132">如果成功，此方法返回`200 OK`响应代码和响应正文中的[appRoleAssignment](../resources/approleassignment.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="01920-132">If successful, this method returns a `200 OK` response code and collection of [appRoleAssignment](../resources/approleassignment.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="01920-133">示例</span><span class="sxs-lookup"><span data-stu-id="01920-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="01920-134">请求</span><span class="sxs-lookup"><span data-stu-id="01920-134">Request</span></span>
<span data-ttu-id="01920-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="01920-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_approleassignments"
}-->
```http
GET https://graph.microsoft.com/beta/servicePrincipals/{id}/appRoleAssignments
```
##### <a name="response"></a><span data-ttu-id="01920-136">响应</span><span class="sxs-lookup"><span data-stu-id="01920-136">Response</span></span>
<span data-ttu-id="01920-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="01920-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.approleassignment",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 306

{
  "value": [
    {
      "creationTimestamp": "2016-10-19T10:37:00Z",
      "id": "id-value",
      "principalDisplayName": "principalDisplayName-value",
      "principalId": "principalId-value",
      "principalType": "principalType-value",
      "resourceDisplayName": "resourceDisplayName-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List appRoleAssignments",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
