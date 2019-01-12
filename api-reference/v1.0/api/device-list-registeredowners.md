---
title: 列出 registeredOwner
description: 检索身份为已注册设备的所有者的用户列表。 已注册的所有者是云加入设备或已注册个人设备的用户。 已注册的所有者是在注册时设置。 目前，只能有一个所有者。
localization_priority: Normal
author: lleonard-msft
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ec8990a2b0c2d0f674304c4005fbf28a0b5a631e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27976889"
---
# <a name="list-registeredowners"></a><span data-ttu-id="17b29-106">列出 registeredOwner</span><span class="sxs-lookup"><span data-stu-id="17b29-106">List registeredOwners</span></span>

<span data-ttu-id="17b29-107">检索身份为已注册设备的所有者的用户列表。</span><span class="sxs-lookup"><span data-stu-id="17b29-107">Retrieve a list of users that are registered owners of the device.</span></span> <span data-ttu-id="17b29-108">已注册的所有者是云加入设备或已注册个人设备的用户。</span><span class="sxs-lookup"><span data-stu-id="17b29-108">A registered owner is the user that cloud joined the device or registered their personal device.</span></span> <span data-ttu-id="17b29-109">已注册的所有者是在注册时设置。</span><span class="sxs-lookup"><span data-stu-id="17b29-109">The registered owner is set at the time of registration.</span></span> <span data-ttu-id="17b29-110">目前，只能有一个所有者。</span><span class="sxs-lookup"><span data-stu-id="17b29-110">Currently, there can be only one owner.</span></span>

## <a name="permissions"></a><span data-ttu-id="17b29-111">权限</span><span class="sxs-lookup"><span data-stu-id="17b29-111">Permissions</span></span>
<span data-ttu-id="17b29-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="17b29-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="17b29-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="17b29-114">Permission type</span></span>      | <span data-ttu-id="17b29-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="17b29-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="17b29-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="17b29-116">Delegated (work or school account)</span></span> | <span data-ttu-id="17b29-117">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="17b29-117">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="17b29-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="17b29-118">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="17b29-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="17b29-119">Not supported.</span></span>    |
|<span data-ttu-id="17b29-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="17b29-120">Application</span></span> | <span data-ttu-id="17b29-121">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="17b29-121">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="17b29-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="17b29-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredOwners
```
## <a name="optional-query-parameters"></a><span data-ttu-id="17b29-123">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="17b29-123">Optional query parameters</span></span>
<span data-ttu-id="17b29-124">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="17b29-124">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="17b29-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="17b29-125">Request headers</span></span>
| <span data-ttu-id="17b29-126">名称</span><span class="sxs-lookup"><span data-stu-id="17b29-126">Name</span></span>       | <span data-ttu-id="17b29-127">类型</span><span class="sxs-lookup"><span data-stu-id="17b29-127">Type</span></span> | <span data-ttu-id="17b29-128">说明</span><span class="sxs-lookup"><span data-stu-id="17b29-128">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="17b29-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="17b29-129">Authorization</span></span>  | <span data-ttu-id="17b29-130">string</span><span class="sxs-lookup"><span data-stu-id="17b29-130">string</span></span>  | <span data-ttu-id="17b29-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="17b29-p104">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="17b29-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="17b29-133">Request body</span></span>
<span data-ttu-id="17b29-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="17b29-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="17b29-135">响应</span><span class="sxs-lookup"><span data-stu-id="17b29-135">Response</span></span>

<span data-ttu-id="17b29-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="17b29-136">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="17b29-137">示例</span><span class="sxs-lookup"><span data-stu-id="17b29-137">Example</span></span>
##### <a name="request"></a><span data-ttu-id="17b29-138">请求</span><span class="sxs-lookup"><span data-stu-id="17b29-138">Request</span></span>
<span data-ttu-id="17b29-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="17b29-139">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredowners"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/registeredOwners
```
##### <a name="response"></a><span data-ttu-id="17b29-140">响应</span><span class="sxs-lookup"><span data-stu-id="17b29-140">Response</span></span>
<span data-ttu-id="17b29-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="17b29-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredOwners",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
