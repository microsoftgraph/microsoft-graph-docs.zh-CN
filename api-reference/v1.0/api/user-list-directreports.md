---
title: 列出 directReports
description: 获取用户的直接下属。 返回指定此用户作为经理的用户和联系人。
localization_priority: Normal
author: dkershaw10
ms.prod: microsoft-identity-platform
ms.openlocfilehash: a397e45675b245325d1a086e0b87117358514e15
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32571399"
---
# <a name="list-directreports"></a><span data-ttu-id="41220-104">列出 directReports</span><span class="sxs-lookup"><span data-stu-id="41220-104">List directReports</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="41220-105">获取用户的直接下属。</span><span class="sxs-lookup"><span data-stu-id="41220-105">Get user's direct reports.</span></span> <span data-ttu-id="41220-106">返回指定此用户作为经理的用户和联系人。</span><span class="sxs-lookup"><span data-stu-id="41220-106">Returns the users and contacts for whom this user is assigned as manager.</span></span>
## <a name="permissions"></a><span data-ttu-id="41220-107">权限</span><span class="sxs-lookup"><span data-stu-id="41220-107">Permissions</span></span>
<span data-ttu-id="41220-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41220-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41220-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="41220-110">Permission type</span></span>      | <span data-ttu-id="41220-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="41220-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41220-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41220-112">Delegated (work or school account)</span></span> | <span data-ttu-id="41220-113">User.Read、User.ReadWrite、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="41220-113">User.Read, User.ReadWrite, User.ReadBasic.All, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="41220-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41220-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41220-115">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="41220-115">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="41220-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="41220-116">Application</span></span> | <span data-ttu-id="41220-117">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41220-117">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="41220-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41220-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/directReports
```
## <a name="optional-query-parameters"></a><span data-ttu-id="41220-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="41220-119">Optional query parameters</span></span>
<span data-ttu-id="41220-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="41220-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="41220-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="41220-121">Request headers</span></span>
| <span data-ttu-id="41220-122">标头</span><span class="sxs-lookup"><span data-stu-id="41220-122">Header</span></span>       | <span data-ttu-id="41220-123">值</span><span class="sxs-lookup"><span data-stu-id="41220-123">Value</span></span>|
|:-----------|:------|
| <span data-ttu-id="41220-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="41220-124">Authorization</span></span>  | <span data-ttu-id="41220-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="41220-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="41220-127">Content-Type</span><span class="sxs-lookup"><span data-stu-id="41220-127">Content-Type</span></span>   | <span data-ttu-id="41220-128">application/json</span><span class="sxs-lookup"><span data-stu-id="41220-128">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="41220-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="41220-129">Request body</span></span>
<span data-ttu-id="41220-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="41220-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41220-131">响应</span><span class="sxs-lookup"><span data-stu-id="41220-131">Response</span></span>

<span data-ttu-id="41220-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="41220-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="41220-133">示例</span><span class="sxs-lookup"><span data-stu-id="41220-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="41220-134">请求</span><span class="sxs-lookup"><span data-stu-id="41220-134">Request</span></span>
<span data-ttu-id="41220-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41220-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_directreports"
}-->
```http
GET https://graph.microsoft.com/beta/me/directReports
```
##### <a name="response"></a><span data-ttu-id="41220-136">响应</span><span class="sxs-lookup"><span data-stu-id="41220-136">Response</span></span>
<span data-ttu-id="41220-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="41220-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
