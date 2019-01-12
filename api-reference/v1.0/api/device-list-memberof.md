---
title: 列表设备组
description: 获取此设备直接成员的组。 此操作是不可传递的。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 1642b6ee758af5d2ab4004ea5b7a5293f33f7d01
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27912377"
---
# <a name="list-device-groups"></a><span data-ttu-id="fa568-104">列表设备组</span><span class="sxs-lookup"><span data-stu-id="fa568-104">List device groups</span></span>

<span data-ttu-id="fa568-105">获取此设备直接成员的组。</span><span class="sxs-lookup"><span data-stu-id="fa568-105">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="fa568-106">此操作是不可传递的。</span><span class="sxs-lookup"><span data-stu-id="fa568-106">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="fa568-107">权限</span><span class="sxs-lookup"><span data-stu-id="fa568-107">Permissions</span></span>

<span data-ttu-id="fa568-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fa568-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fa568-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fa568-110">Permission type</span></span>      | <span data-ttu-id="fa568-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fa568-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fa568-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fa568-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fa568-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fa568-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fa568-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fa568-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fa568-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fa568-115">Not supported.</span></span>    |
|<span data-ttu-id="fa568-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fa568-116">Application</span></span> | <span data-ttu-id="fa568-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fa568-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fa568-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fa568-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="fa568-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fa568-119">Optional query parameters</span></span>
<span data-ttu-id="fa568-120">此方法支持 [OData 查询参数](/graph/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fa568-120">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="fa568-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="fa568-121">Request headers</span></span>
| <span data-ttu-id="fa568-122">标头</span><span class="sxs-lookup"><span data-stu-id="fa568-122">Header</span></span>       | <span data-ttu-id="fa568-123">值</span><span class="sxs-lookup"><span data-stu-id="fa568-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="fa568-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="fa568-124">Authorization</span></span>  | <span data-ttu-id="fa568-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fa568-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fa568-127">Accept</span><span class="sxs-lookup"><span data-stu-id="fa568-127">Accept</span></span>  | <span data-ttu-id="fa568-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fa568-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fa568-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="fa568-129">Request body</span></span>
<span data-ttu-id="fa568-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fa568-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fa568-131">响应</span><span class="sxs-lookup"><span data-stu-id="fa568-131">Response</span></span>

<span data-ttu-id="fa568-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fa568-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fa568-133">示例</span><span class="sxs-lookup"><span data-stu-id="fa568-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="fa568-134">请求</span><span class="sxs-lookup"><span data-stu-id="fa568-134">Request</span></span>

<span data-ttu-id="fa568-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fa568-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_user_memberof"
}-->
```http
GET https://graph.microsoft.com/v1.0/devices/{id}/memberOf
```

### <a name="response"></a><span data-ttu-id="fa568-136">响应</span><span class="sxs-lookup"><span data-stu-id="fa568-136">Response</span></span>
<span data-ttu-id="fa568-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fa568-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
