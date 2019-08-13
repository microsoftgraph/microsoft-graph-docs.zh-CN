---
title: 列出设备组
description: 获取此设备是其直接成员的组。 此操作不可传递。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 9a0e7a3ec93766b8b517b558a3bfa5b6778d45c7
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36321463"
---
# <a name="list-device-groups"></a><span data-ttu-id="50105-104">列出设备组</span><span class="sxs-lookup"><span data-stu-id="50105-104">List device groups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="50105-105">获取此设备是其直接成员的组。</span><span class="sxs-lookup"><span data-stu-id="50105-105">Get groups that this device is a direct member of.</span></span> <span data-ttu-id="50105-106">此操作不可传递。</span><span class="sxs-lookup"><span data-stu-id="50105-106">This operation is not transitive.</span></span>

## <a name="permissions"></a><span data-ttu-id="50105-107">权限</span><span class="sxs-lookup"><span data-stu-id="50105-107">Permissions</span></span>

<span data-ttu-id="50105-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="50105-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="50105-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="50105-110">Permission type</span></span>      | <span data-ttu-id="50105-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="50105-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="50105-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="50105-112">Delegated (work or school account)</span></span> | <span data-ttu-id="50105-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="50105-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="50105-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="50105-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="50105-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="50105-115">Not supported.</span></span>    |
|<span data-ttu-id="50105-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="50105-116">Application</span></span> | <span data-ttu-id="50105-117">Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="50105-117">Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="50105-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="50105-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices/{id}/memberOf
```
## <a name="optional-query-parameters"></a><span data-ttu-id="50105-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="50105-119">Optional query parameters</span></span>
<span data-ttu-id="50105-120">此方法支持 [OData 查询参数](/graph/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="50105-120">This method supports the [OData Query Parameters](/graph/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="50105-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="50105-121">Request headers</span></span>
| <span data-ttu-id="50105-122">标头</span><span class="sxs-lookup"><span data-stu-id="50105-122">Header</span></span>       | <span data-ttu-id="50105-123">值</span><span class="sxs-lookup"><span data-stu-id="50105-123">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="50105-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="50105-124">Authorization</span></span>  | <span data-ttu-id="50105-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="50105-p104">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="50105-127">接受</span><span class="sxs-lookup"><span data-stu-id="50105-127">Accept</span></span>  | <span data-ttu-id="50105-128">application/json</span><span class="sxs-lookup"><span data-stu-id="50105-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="50105-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="50105-129">Request body</span></span>
<span data-ttu-id="50105-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="50105-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="50105-131">响应</span><span class="sxs-lookup"><span data-stu-id="50105-131">Response</span></span>

<span data-ttu-id="50105-132">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [directoryObject](../resources/directoryobject.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="50105-132">If successful, this method returns a `200 OK` response code and collection of [directoryObject](../resources/directoryobject.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="50105-133">示例</span><span class="sxs-lookup"><span data-stu-id="50105-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="50105-134">请求</span><span class="sxs-lookup"><span data-stu-id="50105-134">Request</span></span>

<span data-ttu-id="50105-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="50105-135">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="50105-136">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="50105-136">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_device_memberof"
}-->
```http
GET https://graph.microsoft.com/beta/devices/{id}/memberOf
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="50105-137">C#</span><span class="sxs-lookup"><span data-stu-id="50105-137">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-device-memberof-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="50105-138">JavaScript</span><span class="sxs-lookup"><span data-stu-id="50105-138">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-device-memberof-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="50105-139">目标-C</span><span class="sxs-lookup"><span data-stu-id="50105-139">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-device-memberof-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="50105-140">Java</span><span class="sxs-lookup"><span data-stu-id="50105-140">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-device-memberof-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="50105-141">响应</span><span class="sxs-lookup"><span data-stu-id="50105-141">Response</span></span>
<span data-ttu-id="50105-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="50105-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
<!--
{
  "type": "#page.annotation",
  "description": "List memberOf",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
