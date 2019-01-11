---
title: 列出 registeredUser
description: 检索已注册为设备用户的用户列表。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8e552ffe1d3bb07c365f06c4bcfcee08bdacedba
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843594"
---
# <a name="list-registeredusers"></a><span data-ttu-id="c288d-103">列出 registeredUser</span><span class="sxs-lookup"><span data-stu-id="c288d-103">List registeredUsers</span></span>

> <span data-ttu-id="c288d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c288d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c288d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c288d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="c288d-106">检索已注册为设备用户的用户列表。</span><span class="sxs-lookup"><span data-stu-id="c288d-106">Retrieve a list of users that are registered users of the device.</span></span>

<span data-ttu-id="c288d-107">对于云加入设备和已注册的个人设备，已注册用户在设备注册时设置为与已注册所有者相同的值。</span><span class="sxs-lookup"><span data-stu-id="c288d-107">For cloud joined devices and registered personal devices, registered users are set to the same value as registered owners at the time of registration.</span></span>

## <a name="permissions"></a><span data-ttu-id="c288d-108">权限</span><span class="sxs-lookup"><span data-stu-id="c288d-108">Permissions</span></span>
<span data-ttu-id="c288d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c288d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c288d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c288d-111">Permission type</span></span>      | <span data-ttu-id="c288d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c288d-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c288d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c288d-113">Delegated (work or school account)</span></span> | <span data-ttu-id="c288d-114">Directory.Read.All Directory.ReadWrite.All 或 Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c288d-114">Directory.Read.All or Directory.ReadWrite.All or Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c288d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c288d-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c288d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c288d-116">Not supported.</span></span> |
|<span data-ttu-id="c288d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c288d-117">Application</span></span> | <span data-ttu-id="c288d-118">Directory.Read.All 或 Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c288d-118">Directory.Read.All or Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c288d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c288d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/registeredUsers
```

> <span data-ttu-id="c288d-120">注意：请求中的“id”是设备的“id”属性，不是“deviceId”属性。</span><span class="sxs-lookup"><span data-stu-id="c288d-120">Note: The "id" in the request is the "id" property of the device, not the "deviceId" property.</span></span>

## <a name="optional-query-parameters"></a><span data-ttu-id="c288d-121">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c288d-121">Optional query parameters</span></span>
<span data-ttu-id="c288d-122">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c288d-122">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="c288d-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="c288d-123">Request headers</span></span>
| <span data-ttu-id="c288d-124">名称</span><span class="sxs-lookup"><span data-stu-id="c288d-124">Name</span></span>       | <span data-ttu-id="c288d-125">类型</span><span class="sxs-lookup"><span data-stu-id="c288d-125">Type</span></span> | <span data-ttu-id="c288d-126">说明</span><span class="sxs-lookup"><span data-stu-id="c288d-126">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="c288d-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="c288d-127">Authorization</span></span>  | <span data-ttu-id="c288d-128">string</span><span class="sxs-lookup"><span data-stu-id="c288d-128">string</span></span>  | <span data-ttu-id="c288d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c288d-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="c288d-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="c288d-131">Request body</span></span>
<span data-ttu-id="c288d-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c288d-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c288d-133">响应</span><span class="sxs-lookup"><span data-stu-id="c288d-133">Response</span></span>

<span data-ttu-id="c288d-134">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="c288d-134">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="c288d-135">示例</span><span class="sxs-lookup"><span data-stu-id="c288d-135">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c288d-136">请求</span><span class="sxs-lookup"><span data-stu-id="c288d-136">Request</span></span>
<span data-ttu-id="c288d-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c288d-137">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_registeredusers"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/registeredUsers
```
##### <a name="response"></a><span data-ttu-id="c288d-138">响应</span><span class="sxs-lookup"><span data-stu-id="c288d-138">Response</span></span>
<span data-ttu-id="c288d-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c288d-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
  "description": "List registeredUsers",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
