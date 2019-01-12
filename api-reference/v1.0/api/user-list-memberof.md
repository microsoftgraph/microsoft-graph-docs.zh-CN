---
title: 列出 memberOf
description: '返回用户是其直接成员的组和目录角色。 '
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 389cbe5a62b75e9396077d9710c0b92a497e8bd0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962525"
---
# <a name="list-memberof"></a><span data-ttu-id="fc6b1-103">列出 memberOf</span><span class="sxs-lookup"><span data-stu-id="fc6b1-103">List memberOf</span></span>

<span data-ttu-id="fc6b1-104">获取用户是其直接成员的[组](../resources/group.md)和[目录角色](../resources/directoryrole.md)。</span><span class="sxs-lookup"><span data-stu-id="fc6b1-104">Get [groups](../resources/group.md) and [directory roles](../resources/directoryrole.md) that the user is a direct member of.</span></span> 

## <a name="permissions"></a><span data-ttu-id="fc6b1-105">权限</span><span class="sxs-lookup"><span data-stu-id="fc6b1-105">Permissions</span></span>
<span data-ttu-id="fc6b1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fc6b1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fc6b1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc6b1-108">Permission type</span></span>      | <span data-ttu-id="fc6b1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fc6b1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fc6b1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc6b1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="fc6b1-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fc6b1-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fc6b1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc6b1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fc6b1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc6b1-113">Not supported.</span></span>    |
|<span data-ttu-id="fc6b1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc6b1-114">Application</span></span> | <span data-ttu-id="fc6b1-115">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc6b1-115">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fc6b1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc6b1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fc6b1-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fc6b1-117">Optional query parameters</span></span>
<span data-ttu-id="fc6b1-p102">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters)来帮助自定义响应。$filter 不受支持。</span><span class="sxs-lookup"><span data-stu-id="fc6b1-p102">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response. $filter is not supported.</span></span> 

## <a name="request-headers"></a><span data-ttu-id="fc6b1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc6b1-120">Request headers</span></span>
| <span data-ttu-id="fc6b1-121">标头</span><span class="sxs-lookup"><span data-stu-id="fc6b1-121">Header</span></span>       | <span data-ttu-id="fc6b1-122">值</span><span class="sxs-lookup"><span data-stu-id="fc6b1-122">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fc6b1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc6b1-123">Authorization</span></span>  | <span data-ttu-id="fc6b1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fc6b1-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fc6b1-126">Accept</span><span class="sxs-lookup"><span data-stu-id="fc6b1-126">Accept</span></span>  | <span data-ttu-id="fc6b1-127">application/json</span><span class="sxs-lookup"><span data-stu-id="fc6b1-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc6b1-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc6b1-128">Request body</span></span>
<span data-ttu-id="fc6b1-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fc6b1-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fc6b1-130">响应</span><span class="sxs-lookup"><span data-stu-id="fc6b1-130">Response</span></span>

<span data-ttu-id="fc6b1-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fc6b1-131">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="fc6b1-132">示例</span><span class="sxs-lookup"><span data-stu-id="fc6b1-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fc6b1-133">请求</span><span class="sxs-lookup"><span data-stu-id="fc6b1-133">Request</span></span>
<span data-ttu-id="fc6b1-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc6b1-134">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/memberOf
```
##### <a name="response"></a><span data-ttu-id="fc6b1-135">响应</span><span class="sxs-lookup"><span data-stu-id="fc6b1-135">Response</span></span>
<span data-ttu-id="fc6b1-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fc6b1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
