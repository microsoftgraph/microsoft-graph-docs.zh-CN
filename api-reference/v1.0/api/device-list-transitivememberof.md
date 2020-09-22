---
title: List device transitive groups
description: 获取设备所属的组。
author: spunukol
ms.prod: microsoft-identity-platform
localization_priority: Normal
doc_type: apiPageType
ms.openlocfilehash: 859cd2fa83a62f04d65f2553e2fd33f3c483e760
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48078022"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="41113-103">List device transitive groups</span><span class="sxs-lookup"><span data-stu-id="41113-103">List device transitive groups</span></span>

<span data-ttu-id="41113-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="41113-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="41113-105">获取设备所属的组。</span><span class="sxs-lookup"><span data-stu-id="41113-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="41113-106">此 API 请求是可传递的，并且还将返回设备是其嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="41113-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="41113-107">权限</span><span class="sxs-lookup"><span data-stu-id="41113-107">Permissions</span></span>

<span data-ttu-id="41113-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="41113-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="41113-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="41113-110">Permission type</span></span>      | <span data-ttu-id="41113-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="41113-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="41113-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="41113-112">Delegated (work or school account)</span></span> | <span data-ttu-id="41113-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="41113-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="41113-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="41113-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="41113-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="41113-115">Not supported.</span></span>    |
|<span data-ttu-id="41113-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="41113-116">Application</span></span> | <span data-ttu-id="41113-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="41113-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

[!INCLUDE [limited-info](../../includes/limited-info.md)]

## <a name="http-request"></a><span data-ttu-id="41113-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="41113-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="41113-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="41113-119">Optional query parameters</span></span>

<span data-ttu-id="41113-120">此方法支持 [OData 查询参数](/graph/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="41113-120">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="41113-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="41113-121">Request headers</span></span>

| <span data-ttu-id="41113-122">标头</span><span class="sxs-lookup"><span data-stu-id="41113-122">Header</span></span>       | <span data-ttu-id="41113-123">值</span><span class="sxs-lookup"><span data-stu-id="41113-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="41113-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="41113-124">Authorization</span></span>  | <span data-ttu-id="41113-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="41113-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="41113-127">接受</span><span class="sxs-lookup"><span data-stu-id="41113-127">Accept</span></span>  | <span data-ttu-id="41113-128">application/json</span><span class="sxs-lookup"><span data-stu-id="41113-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="41113-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="41113-129">Request body</span></span>

<span data-ttu-id="41113-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="41113-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="41113-131">响应</span><span class="sxs-lookup"><span data-stu-id="41113-131">Response</span></span>

<span data-ttu-id="41113-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="41113-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="41113-133">示例</span><span class="sxs-lookup"><span data-stu-id="41113-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="41113-134">请求</span><span class="sxs-lookup"><span data-stu-id="41113-134">Request</span></span>

<span data-ttu-id="41113-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="41113-135">Here is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="41113-136">HTTP</span><span class="sxs-lookup"><span data-stu-id="41113-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf
```
# <a name="c"></a>[<span data-ttu-id="41113-137">C#</span><span class="sxs-lookup"><span data-stu-id="41113-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-transitivememberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="41113-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="41113-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-transitivememberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="41113-139">Objective-C</span><span class="sxs-lookup"><span data-stu-id="41113-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-transitivememberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="41113-140">Java</span><span class="sxs-lookup"><span data-stu-id="41113-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-transitivememberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="41113-141">响应</span><span class="sxs-lookup"><span data-stu-id="41113-141">Response</span></span>

<span data-ttu-id="41113-142">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="41113-142">Here is an example of the response.</span></span> 

><span data-ttu-id="41113-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="41113-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
  "description": "List devices transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->

