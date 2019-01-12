---
title: 列出 createdObjects
description: 获取由用户创建的 directory 对象列表。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 33b3f7ded23a7bd72274dff159a824acb03e6bb5
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27925754"
---
# <a name="list-createdobjects"></a><span data-ttu-id="e6b3d-103">列出 createdObjects</span><span class="sxs-lookup"><span data-stu-id="e6b3d-103">List createdObjects</span></span>

<span data-ttu-id="e6b3d-104">获取由用户创建的 directory 对象列表。</span><span class="sxs-lookup"><span data-stu-id="e6b3d-104">Get a list of directory objects that were created by the user.</span></span>
## <a name="permissions"></a><span data-ttu-id="e6b3d-105">权限</span><span class="sxs-lookup"><span data-stu-id="e6b3d-105">Permissions</span></span>
<span data-ttu-id="e6b3d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e6b3d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e6b3d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="e6b3d-108">Permission type</span></span>      | <span data-ttu-id="e6b3d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e6b3d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="e6b3d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e6b3d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="e6b3d-111">User.Read、User.ReadWrite、User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="e6b3d-111">User.Read, User.ReadWrite, User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="e6b3d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e6b3d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="e6b3d-113">User.Read、User.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="e6b3d-113">User.Read, User.ReadWrite</span></span>    |
|<span data-ttu-id="e6b3d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="e6b3d-114">Application</span></span> | <span data-ttu-id="e6b3d-115">User.Read.All、User.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e6b3d-115">User.Read.All, User.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="e6b3d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e6b3d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /users/{id | userPrincipalName}/createdObjects
```
## <a name="optional-query-parameters"></a><span data-ttu-id="e6b3d-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="e6b3d-117">Optional query parameters</span></span>
<span data-ttu-id="e6b3d-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="e6b3d-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="e6b3d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e6b3d-119">Request headers</span></span>
| <span data-ttu-id="e6b3d-120">标头</span><span class="sxs-lookup"><span data-stu-id="e6b3d-120">Header</span></span>       | <span data-ttu-id="e6b3d-121">值</span><span class="sxs-lookup"><span data-stu-id="e6b3d-121">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="e6b3d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e6b3d-122">Authorization</span></span>  | <span data-ttu-id="e6b3d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e6b3d-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="e6b3d-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="e6b3d-125">Content-Type</span></span>  | <span data-ttu-id="e6b3d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e6b3d-126">application/json</span></span>  |

## <a name="request-body"></a><span data-ttu-id="e6b3d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e6b3d-127">Request body</span></span>
<span data-ttu-id="e6b3d-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e6b3d-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e6b3d-129">响应</span><span class="sxs-lookup"><span data-stu-id="e6b3d-129">Response</span></span>

<span data-ttu-id="e6b3d-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e6b3d-130">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e6b3d-131">示例</span><span class="sxs-lookup"><span data-stu-id="e6b3d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e6b3d-132">请求</span><span class="sxs-lookup"><span data-stu-id="e6b3d-132">Request</span></span>
<span data-ttu-id="e6b3d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e6b3d-133">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_createdobjects"
}-->
```http
GET https://graph.microsoft.com/v1.0/me/createdObjects
```
##### <a name="response"></a><span data-ttu-id="e6b3d-134">响应</span><span class="sxs-lookup"><span data-stu-id="e6b3d-134">Response</span></span>
<span data-ttu-id="e6b3d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e6b3d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!-- {
  "type": "#page.annotation",
  "description": "List createdObjects",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
