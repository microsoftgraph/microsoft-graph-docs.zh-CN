---
title: List directReports
description: 获取用户的直接下属。 返回指定此用户作为经理的用户和联系人。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: b87425e47b511361031aeec29aba5304383179e4
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33334860"
---
# <a name="list-directreports"></a><span data-ttu-id="3067a-104">List directReports</span><span class="sxs-lookup"><span data-stu-id="3067a-104">List directReports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3067a-105">获取用户的直接下属。</span><span class="sxs-lookup"><span data-stu-id="3067a-105">Get user's direct reports.</span></span> <span data-ttu-id="3067a-106">返回指定此用户作为经理的用户和联系人。</span><span class="sxs-lookup"><span data-stu-id="3067a-106">Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="3067a-107">权限</span><span class="sxs-lookup"><span data-stu-id="3067a-107">Permissions</span></span>
<span data-ttu-id="3067a-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3067a-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3067a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3067a-110">Permission type</span></span>      | <span data-ttu-id="3067a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3067a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="3067a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3067a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="3067a-113">如果是, 则为用户读取、用户读取、全部、全部、全部、directory.accessasuser.all、全部、全部、全部、目录。</span><span class="sxs-lookup"><span data-stu-id="3067a-113">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="3067a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3067a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="3067a-115">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="3067a-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="3067a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3067a-116">Application</span></span> | <span data-ttu-id="3067a-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3067a-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="3067a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3067a-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="3067a-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="3067a-119">Optional query parameters</span></span>
<span data-ttu-id="3067a-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="3067a-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="3067a-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="3067a-121">Request headers</span></span>
| <span data-ttu-id="3067a-122">标头</span><span class="sxs-lookup"><span data-stu-id="3067a-122">Header</span></span>       | <span data-ttu-id="3067a-123">值</span><span class="sxs-lookup"><span data-stu-id="3067a-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="3067a-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="3067a-124">Authorization</span></span>  | <span data-ttu-id="3067a-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3067a-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3067a-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3067a-127">Content-Type</span></span>   | <span data-ttu-id="3067a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="3067a-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="3067a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="3067a-129">Request body</span></span>
<span data-ttu-id="3067a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3067a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3067a-131">响应</span><span class="sxs-lookup"><span data-stu-id="3067a-131">Response</span></span>

<span data-ttu-id="3067a-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3067a-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="3067a-133">示例</span><span class="sxs-lookup"><span data-stu-id="3067a-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="3067a-134">请求</span><span class="sxs-lookup"><span data-stu-id="3067a-134">Request</span></span>
<span data-ttu-id="3067a-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3067a-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/beta/me/directReports
```
##### <a name="response"></a><span data-ttu-id="3067a-136">响应</span><span class="sxs-lookup"><span data-stu-id="3067a-136">Response</span></span>
<span data-ttu-id="3067a-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3067a-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List directReports",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
