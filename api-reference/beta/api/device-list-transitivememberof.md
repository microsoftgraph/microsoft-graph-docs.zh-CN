---
title: 列出设备可传递组
description: 获取设备所属的组。 此 API 请求是可传递的, 并且还将返回设备是其嵌套成员的所有组。
localization_priority: Normal
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 93d27fcfc4163afbe5b833a2f510365d8093fbc3
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34656312"
---
# <a name="list-device-transitive-groups"></a><span data-ttu-id="cef0c-104">列出设备可传递组</span><span class="sxs-lookup"><span data-stu-id="cef0c-104">List device transitive groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="cef0c-105">获取设备所属的组。</span><span class="sxs-lookup"><span data-stu-id="cef0c-105">Get groups that the device is a member of.</span></span> <span data-ttu-id="cef0c-106">此 API 请求是可传递的, 并且还将返回设备是其嵌套成员的所有组。</span><span class="sxs-lookup"><span data-stu-id="cef0c-106">This API request is transitive, and will also return all groups the device is a nested member of.</span></span>

## <a name="permissions"></a><span data-ttu-id="cef0c-107">权限</span><span class="sxs-lookup"><span data-stu-id="cef0c-107">Permissions</span></span>

<span data-ttu-id="cef0c-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cef0c-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cef0c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cef0c-110">Permission type</span></span>      | <span data-ttu-id="cef0c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="cef0c-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="cef0c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cef0c-112">Delegated (work or school account)</span></span> | <span data-ttu-id="cef0c-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="cef0c-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="cef0c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cef0c-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="cef0c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cef0c-115">Not supported.</span></span>    |
|<span data-ttu-id="cef0c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cef0c-116">Application</span></span> | <span data-ttu-id="cef0c-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cef0c-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="cef0c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cef0c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
GET /devices/{id}/transitiveMemberOf
```

## <a name="optional-query-parameters"></a><span data-ttu-id="cef0c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="cef0c-119">Optional query parameters</span></span>

<span data-ttu-id="cef0c-120">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="cef0c-120">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="cef0c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="cef0c-121">Request headers</span></span>

| <span data-ttu-id="cef0c-122">标头</span><span class="sxs-lookup"><span data-stu-id="cef0c-122">Header</span></span>       | <span data-ttu-id="cef0c-123">值</span><span class="sxs-lookup"><span data-stu-id="cef0c-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="cef0c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="cef0c-124">Authorization</span></span>  | <span data-ttu-id="cef0c-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cef0c-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cef0c-127">接受</span><span class="sxs-lookup"><span data-stu-id="cef0c-127">Accept</span></span>  | <span data-ttu-id="cef0c-128">application/json</span><span class="sxs-lookup"><span data-stu-id="cef0c-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cef0c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="cef0c-129">Request body</span></span>

<span data-ttu-id="cef0c-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cef0c-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cef0c-131">响应</span><span class="sxs-lookup"><span data-stu-id="cef0c-131">Response</span></span>

<span data-ttu-id="cef0c-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cef0c-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cef0c-133">示例</span><span class="sxs-lookup"><span data-stu-id="cef0c-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="cef0c-134">请求</span><span class="sxs-lookup"><span data-stu-id="cef0c-134">Request</span></span>

<span data-ttu-id="cef0c-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cef0c-135">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "get_devices_transitivememberof"
}-->

```http
GET https://graph.microsoft.com/beta/devices/{id}/transitiveMemberOf
```

### <a name="response"></a><span data-ttu-id="cef0c-136">响应</span><span class="sxs-lookup"><span data-stu-id="cef0c-136">Response</span></span>

<span data-ttu-id="cef0c-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cef0c-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

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
#### <a name="sdk-sample-code"></a><span data-ttu-id="cef0c-140">SDK 示例代码</span><span class="sxs-lookup"><span data-stu-id="cef0c-140">SDK sample code</span></span>
# <a name="ctabcs"></a>[<span data-ttu-id="cef0c-141">C#</span><span class="sxs-lookup"><span data-stu-id="cef0c-141">C#</span></span>](#tab/cs)
[!INCLUDE [sample-code](../includes/get_devices_transitivememberof-Cs-snippets.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="cef0c-142">Javascript</span><span class="sxs-lookup"><span data-stu-id="cef0c-142">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/get_devices_transitivememberof-Javascript-snippets.md)]

---

[!INCLUDE [sdk-documentation](../includes/snippets_sdk_documentation_link.md)]

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List devices transitiveMsemberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/device-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/cs](C#)'. Did you mean: #c (score: 5)",
    "Error: /api-reference/beta/api/device-list-transitivememberof.md:\r\n      BookmarkMissing: '[#tab/javascript](Javascript)'. Did you mean: #javascript (score: 4)"
  ]
}
-->
