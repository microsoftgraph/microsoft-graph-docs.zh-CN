---
title: 列出设备
description: 检索组织中注册的 device 对象的列表。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 4a6b1ce4ec8d467ed1d269b4344d18bdbc854028
ms.sourcegitcommit: d1742ec820776f1e95cba76d98c6cfd17d3eadbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/04/2019
ms.locfileid: "36721319"
---
# <a name="list-devices"></a><span data-ttu-id="ff5fc-103">列出设备</span><span class="sxs-lookup"><span data-stu-id="ff5fc-103">List devices</span></span>

<span data-ttu-id="ff5fc-104">检索组织中注册的 device 对象的列表。</span><span class="sxs-lookup"><span data-stu-id="ff5fc-104">Retrieve a list of device objects registered in the organization.</span></span>

## <a name="permissions"></a><span data-ttu-id="ff5fc-105">权限</span><span class="sxs-lookup"><span data-stu-id="ff5fc-105">Permissions</span></span>
<span data-ttu-id="ff5fc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff5fc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="ff5fc-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff5fc-108">Permission type</span></span>      | <span data-ttu-id="ff5fc-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ff5fc-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ff5fc-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff5fc-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ff5fc-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ff5fc-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ff5fc-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff5fc-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ff5fc-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff5fc-113">Not supported.</span></span>    |
|<span data-ttu-id="ff5fc-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff5fc-114">Application</span></span> | <span data-ttu-id="ff5fc-115">Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ff5fc-115">Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ff5fc-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff5fc-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
GET /devices
```
## <a name="optional-query-parameters"></a><span data-ttu-id="ff5fc-117">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ff5fc-117">Optional query parameters</span></span>
<span data-ttu-id="ff5fc-118">此方法支持 [OData 查询参数](https://developer.microsoft.com/graph/docs/concepts/query_parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="ff5fc-118">This method supports the [OData Query Parameters](https://developer.microsoft.com/graph/docs/concepts/query_parameters) to help customize the response.</span></span>
## <a name="request-headers"></a><span data-ttu-id="ff5fc-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff5fc-119">Request headers</span></span>
| <span data-ttu-id="ff5fc-120">名称</span><span class="sxs-lookup"><span data-stu-id="ff5fc-120">Name</span></span>       | <span data-ttu-id="ff5fc-121">类型</span><span class="sxs-lookup"><span data-stu-id="ff5fc-121">Type</span></span> | <span data-ttu-id="ff5fc-122">说明</span><span class="sxs-lookup"><span data-stu-id="ff5fc-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ff5fc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff5fc-123">Authorization</span></span>  | <span data-ttu-id="ff5fc-124">string</span><span class="sxs-lookup"><span data-stu-id="ff5fc-124">string</span></span>  | <span data-ttu-id="ff5fc-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ff5fc-p102">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ff5fc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff5fc-127">Request body</span></span>
<span data-ttu-id="ff5fc-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ff5fc-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff5fc-129">响应</span><span class="sxs-lookup"><span data-stu-id="ff5fc-129">Response</span></span>

<span data-ttu-id="ff5fc-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [device](../resources/device.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ff5fc-130">If successful, this method returns a `200 OK` response code and collection of [device](../resources/device.md) objects in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ff5fc-131">示例</span><span class="sxs-lookup"><span data-stu-id="ff5fc-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ff5fc-132">请求</span><span class="sxs-lookup"><span data-stu-id="ff5fc-132">Request</span></span>
<span data-ttu-id="ff5fc-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ff5fc-133">Here is an example of the request.</span></span>

# <a name="httptabhttp"></a>[<span data-ttu-id="ff5fc-134">HTTP.SYS</span><span class="sxs-lookup"><span data-stu-id="ff5fc-134">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_devices"
}-->
```msgraph-interactive
GET https://graph.microsoft.com/v1.0/devices
```
# <a name="ctabcsharp"></a>[<span data-ttu-id="ff5fc-135">C#</span><span class="sxs-lookup"><span data-stu-id="ff5fc-135">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-devices-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascripttabjavascript"></a>[<span data-ttu-id="ff5fc-136">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ff5fc-136">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-devices-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-ctabobjc"></a>[<span data-ttu-id="ff5fc-137">目标-C</span><span class="sxs-lookup"><span data-stu-id="ff5fc-137">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-devices-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javatabjava"></a>[<span data-ttu-id="ff5fc-138">Java</span><span class="sxs-lookup"><span data-stu-id="ff5fc-138">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-devices-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


##### <a name="response"></a><span data-ttu-id="ff5fc-139">响应</span><span class="sxs-lookup"><span data-stu-id="ff5fc-139">Response</span></span>
<span data-ttu-id="ff5fc-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ff5fc-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
      "accountEnabled":false,
      "deviceId":"4c299165-6e8f-4b45-a5ba-c5d250a707ff",
      "displayName":"Test device",
      "id": "id-value",
      "operatingSystem":"linux",
      "operatingSystemVersion":"1"
    }
  ]
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "List devices",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
  ]
}-->
