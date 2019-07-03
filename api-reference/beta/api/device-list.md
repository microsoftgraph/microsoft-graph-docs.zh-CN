---
title: 列出设备
description: '检索目录中的注册设备列表。 '
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: eec732d08a18158570f6826bb9b06208f8d4d4dd
ms.sourcegitcommit: 3f6a4eebe4b73ba848edbff74d51a2d5c81b7318
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/02/2019
ms.locfileid: "35437220"
---
# <a name="list-devices"></a><span data-ttu-id="d4b07-103">列出设备</span><span class="sxs-lookup"><span data-stu-id="d4b07-103">List devices</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d4b07-104">检索目录中的注册设备列表。</span><span class="sxs-lookup"><span data-stu-id="d4b07-104">Retrieve a list of devices registered in the directory.</span></span> 

## <a name="permissions"></a><span data-ttu-id="d4b07-105">权限</span><span class="sxs-lookup"><span data-stu-id="d4b07-105">Permissions</span></span>
<span data-ttu-id="d4b07-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4b07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="d4b07-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4b07-108">Permission type</span></span>      | <span data-ttu-id="d4b07-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d4b07-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="d4b07-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4b07-110">Delegated (work or school account)</span></span> | <span data-ttu-id="d4b07-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="d4b07-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="d4b07-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4b07-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="d4b07-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4b07-113">Not supported.</span></span>    |
|<span data-ttu-id="d4b07-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4b07-114">Application</span></span> | <span data-ttu-id="d4b07-115">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4b07-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="d4b07-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4b07-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="d4b07-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d4b07-117">Optional query parameters</span></span>
<span data-ttu-id="d4b07-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d4b07-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="d4b07-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4b07-119">Request headers</span></span>
| <span data-ttu-id="d4b07-120">名称</span><span class="sxs-lookup"><span data-stu-id="d4b07-120">Name</span></span>       | <span data-ttu-id="d4b07-121">类型</span><span class="sxs-lookup"><span data-stu-id="d4b07-121">Type</span></span> | <span data-ttu-id="d4b07-122">说明</span><span class="sxs-lookup"><span data-stu-id="d4b07-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="d4b07-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4b07-123">Authorization</span></span>  | <span data-ttu-id="d4b07-124">string</span><span class="sxs-lookup"><span data-stu-id="d4b07-124">string</span></span>  | <span data-ttu-id="d4b07-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="d4b07-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="d4b07-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4b07-127">Request body</span></span>
<span data-ttu-id="d4b07-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d4b07-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4b07-129">响应</span><span class="sxs-lookup"><span data-stu-id="d4b07-129">Response</span></span>

<span data-ttu-id="d4b07-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="d4b07-130">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="d4b07-131">示例</span><span class="sxs-lookup"><span data-stu-id="d4b07-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="d4b07-132">请求</span><span class="sxs-lookup"><span data-stu-id="d4b07-132">Request</span></span>
<span data-ttu-id="d4b07-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d4b07-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="d4b07-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="d4b07-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```http
GET https://graph.microsoft.com/beta/devices
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="d4b07-135">C#</span><span class="sxs-lookup"><span data-stu-id="d4b07-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="d4b07-136">Javascript</span><span class="sxs-lookup"><span data-stu-id="d4b07-136">Javascript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="d4b07-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="d4b07-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="d4b07-138">响应</span><span class="sxs-lookup"><span data-stu-id="d4b07-138">Response</span></span>
<span data-ttu-id="d4b07-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d4b07-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.device",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "value": [
    {
      "accountEnabled": true,
      "approximateLastSignInDateTime": "2016-10-19T10:37:00Z",
      "deviceId": "deviceId-value",
      "deviceMetadata": "deviceMetadata-value",
      "displayName" : "displayName-value",
      "id" : "id-value", 
      "operatingSystem" : "operatingSystem-value"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}
-->
