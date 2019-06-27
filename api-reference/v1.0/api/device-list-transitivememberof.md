---
title: 列出设备可传递组
description: 获取设备所属的组。 此 API 请求是可传递的, 并且还将返回设备是其嵌套成员的所有组。
author: anchanda
localization_priority: Normal
ms.prod: groups
ms.openlocfilehash: 81b68344e018aa44e41923e02a519a541f547fe0
ms.sourcegitcommit: 0e1101d499f35b08aa2309e273871438b1774979
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/27/2019
ms.locfileid: "35276319"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="0c103-104">列出设备可传递组</span><span class="sxs-lookup"><span data-stu-id="0c103-104">List device transitive groups</span></span>

<span data-ttu-id="0c103-105">获取设备所属的组。</span><span class="sxs-lookup"><span data-stu-id="0c103-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="0c103-106">此 API 请求是可传递的, 并且还将返回设备是其嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="0c103-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="0c103-107">权限</span><span class="sxs-lookup"><span data-stu-id="0c103-107">Permissions</span></span>

<span data-ttu-id="0c103-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c103-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c103-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c103-110">Permission type</span></span>      | <span data-ttu-id="0c103-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0c103-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0c103-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c103-112">Delegated (work or school account)</span></span> | <span data-ttu-id="0c103-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0c103-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0c103-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c103-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0c103-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c103-115">Not supported.</span></span>    |
|<span data-ttu-id="0c103-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c103-116">Application</span></span> | <span data-ttu-id="0c103-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c103-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0c103-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c103-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id | userPrincipalName}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="0c103-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="0c103-119">Optional query parameters</span></span>

<span data-ttu-id="0c103-120">此方法支持 [OData 查询参数](/graph/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="0c103-120">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="0c103-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c103-121">Request headers</span></span>

| <span data-ttu-id="0c103-122">标头</span><span class="sxs-lookup"><span data-stu-id="0c103-122">Header</span></span>       | <span data-ttu-id="0c103-123">值</span><span class="sxs-lookup"><span data-stu-id="0c103-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="0c103-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c103-124">Authorization</span></span>  | <span data-ttu-id="0c103-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0c103-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="0c103-127">接受</span><span class="sxs-lookup"><span data-stu-id="0c103-127">Accept</span></span>  | <span data-ttu-id="0c103-128">application/json</span><span class="sxs-lookup"><span data-stu-id="0c103-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c103-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c103-129">Request body</span></span>

<span data-ttu-id="0c103-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0c103-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0c103-131">响应</span><span class="sxs-lookup"><span data-stu-id="0c103-131">Response</span></span>

<span data-ttu-id="0c103-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0c103-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c103-133">示例</span><span class="sxs-lookup"><span data-stu-id="0c103-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c103-134">请求</span><span class="sxs-lookup"><span data-stu-id="0c103-134">Request</span></span>

<span data-ttu-id="0c103-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0c103-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/v1.0/devices/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="0c103-136">响应</span><span class="sxs-lookup"><span data-stu-id="0c103-136">Response</span></span>

<span data-ttu-id="0c103-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0c103-137">Here is an example of the response.</span></span> 

><span data-ttu-id="0c103-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="0c103-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="0c103-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="0c103-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="0c103-141">C#</span><span class="sxs-lookup"><span data-stu-id="0c103-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_devices_transitivememberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="0c103-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="0c103-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_devices_transitivememberof-Javascript-snippets.md)]

# <a name="objective-ctabobjective-c"></a>[<span data-ttu-id="0c103-143">目标-C</span><span class="sxs-lookup"><span data-stu-id="0c103-143">Objective-C</span></span>](#tab/objective-c)
[!INCLUDE [sample-code](../includes/get_devices_transitivememberof-Objective-C-snippets.md)]
---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List devices transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/v1.0/api/device-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/objective-c](Objective-C)'. Did you mean: #objective-c (score: 4)",
    "Error: /api-reference/v1.0/api/device-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/v1.0/api/device-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}-->
