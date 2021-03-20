---
title: 列出设备使用情况Rights
description: 检索设备的 usageRights 对象列表。
author: jeeshnair
localization_priority: Normal
ms.prod: directory-management
doc_type: apiPageType
ms.openlocfilehash: a855ebf34d8e97a7a5fad00df2a022779ff2bc0d
ms.sourcegitcommit: 68b49fc847ceb1032a9cc9821a9ec0f7ac4abe44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/20/2021
ms.locfileid: "50946799"
---
# <a name="list-device-usagerights"></a><span data-ttu-id="a53eb-103">列出设备使用情况Rights</span><span class="sxs-lookup"><span data-stu-id="a53eb-103">List device usageRights</span></span>
<span data-ttu-id="a53eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a53eb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a53eb-105">检索给定设备的 [usageRight](../resources/usageright.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="a53eb-105">Retrieve a list of [usageRight](../resources/usageright.md) objects for a given device.</span></span>

## <a name="permissions"></a><span data-ttu-id="a53eb-106">权限</span><span class="sxs-lookup"><span data-stu-id="a53eb-106">Permissions</span></span>
<span data-ttu-id="a53eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a53eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a53eb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a53eb-109">Permission type</span></span>|<span data-ttu-id="a53eb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a53eb-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a53eb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a53eb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a53eb-112">Device.Read.All、Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a53eb-112">Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="a53eb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a53eb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a53eb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a53eb-114">Not supported.</span></span>|
|<span data-ttu-id="a53eb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a53eb-115">Application</span></span>|<span data-ttu-id="a53eb-116">Device.Read.All、Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a53eb-116">Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a53eb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a53eb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /devices/{objectId}/usageRights
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a53eb-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a53eb-118">Optional query parameters</span></span>
<span data-ttu-id="a53eb-119">此 API 支持 $filter [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="a53eb-119">This API supports the $filter [OData query parameter](/graph/query-parameters).</span></span> <span data-ttu-id="a53eb-120">支持以下$filter模式：</span><span class="sxs-lookup"><span data-stu-id="a53eb-120">The following patterns of $filter are supported:</span></span>

- <span data-ttu-id="a53eb-121">$filter = state eq 'value'</span><span class="sxs-lookup"><span data-stu-id="a53eb-121">$filter = state eq 'value'</span></span>
- <span data-ttu-id="a53eb-122">$filter = serviceIdentifier eq 'value'</span><span class="sxs-lookup"><span data-stu-id="a53eb-122">$filter = serviceIdentifier eq 'value'</span></span>
- <span data-ttu-id="a53eb-123">$filter = state eq 'value' and serviceIdentifier eq 'value'</span><span class="sxs-lookup"><span data-stu-id="a53eb-123">$filter = state eq 'value' and serviceIdentifier eq 'value'</span></span>
- <span data-ttu-id="a53eb-124">$filter = ( value1、value2") </span><span class="sxs-lookup"><span data-stu-id="a53eb-124">$filter = state in ('value1', 'value2')</span></span>
- <span data-ttu-id="a53eb-125">$filter =serviceIdentifier in ('value1'， 'value2') </span><span class="sxs-lookup"><span data-stu-id="a53eb-125">$filter = serviceIdentifier in ('value1', 'value2')</span></span>
- <span data-ttu-id="a53eb-126">$filter = ( value1、value2") 和 serviceIdentifier 中的 state ( value1"，"value2") </span><span class="sxs-lookup"><span data-stu-id="a53eb-126">$filter = state in ('value1', 'value2') and serviceIdentifier in ('value1', 'value2')</span></span>

## <a name="request-headers"></a><span data-ttu-id="a53eb-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="a53eb-127">Request headers</span></span>
|<span data-ttu-id="a53eb-128">名称</span><span class="sxs-lookup"><span data-stu-id="a53eb-128">Name</span></span>|<span data-ttu-id="a53eb-129">说明</span><span class="sxs-lookup"><span data-stu-id="a53eb-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="a53eb-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="a53eb-130">Authorization</span></span>|<span data-ttu-id="a53eb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a53eb-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="a53eb-133">odata.maxpagesize</span><span class="sxs-lookup"><span data-stu-id="a53eb-133">odata.maxpagesize</span></span>|<span data-ttu-id="a53eb-134">设置每个结果页的最大大小。</span><span class="sxs-lookup"><span data-stu-id="a53eb-134">Set the max result page size pereference.</span></span> <span data-ttu-id="a53eb-135">可选。</span><span class="sxs-lookup"><span data-stu-id="a53eb-135">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a53eb-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="a53eb-136">Request body</span></span>
<span data-ttu-id="a53eb-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a53eb-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a53eb-138">响应</span><span class="sxs-lookup"><span data-stu-id="a53eb-138">Response</span></span>
<span data-ttu-id="a53eb-139">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [usageRight](../resources/usageright.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="a53eb-139">If successful, this method returns a `200 OK` response code and a collection of [usageRight](../resources/usageright.md) objects in the response body.</span></span>

<span data-ttu-id="a53eb-140">此外，如果响应中有更多的页面，@odata.nextLink。</span><span class="sxs-lookup"><span data-stu-id="a53eb-140">Additionally, if there are more pages in the response an @odata.nextLink is returned.</span></span>

## <a name="examples"></a><span data-ttu-id="a53eb-141">示例</span><span class="sxs-lookup"><span data-stu-id="a53eb-141">Examples</span></span>

### <a name="example-1-get-all-usage-rights-for-a-device"></a><span data-ttu-id="a53eb-142">示例 1：获取设备的所有使用权限</span><span class="sxs-lookup"><span data-stu-id="a53eb-142">Example 1: Get all usage rights for a device</span></span>
 
#### <a name="request"></a><span data-ttu-id="a53eb-143">请求</span><span class="sxs-lookup"><span data-stu-id="a53eb-143">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a53eb-144">HTTP</span><span class="sxs-lookup"><span data-stu-id="a53eb-144">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright_1"
}
-->
``` http
GET https://graph.microsoft.com/beta/devices/{objectId}/usageRights
```
# <a name="c"></a>[<span data-ttu-id="a53eb-145">C#</span><span class="sxs-lookup"><span data-stu-id="a53eb-145">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-1-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a53eb-146">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a53eb-146">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-1-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a53eb-147">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a53eb-147">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-1-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a53eb-148">Java</span><span class="sxs-lookup"><span data-stu-id="a53eb-148">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-1-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a53eb-149">响应</span><span class="sxs-lookup"><span data-stu-id="a53eb-149">Response</span></span>
><span data-ttu-id="a53eb-150">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a53eb-150">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.usageRight)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#devices('fead5c35-ebc5-47c4-a909-c43b4faf2160')/usageRights",
  "@odata.nextLink": "https://graph.microsoft.com/beta/devices/fead5c35-ebc5-47c4-a909-c43b4faf2160/usageRights?$skiptoken=W4diD29cGKX1bX",
  "value": [
    {
      "id": "99f828b9-09f2-445d-a758-b6727316dbe1",
      "catalogId": "CFQ7TTC0KCRG:0001",
      "serviceIdentifier": "mscrm.f6d23ec7-255c-4bd8-8c99-dc041d5cb8b3.517f7ddd-df45-4f1c-83ec-a081a047f546",
      "state": "active"
    }
  ]
}
```

### <a name="example-2-get-usage-rights-for-a-device-with-specific-service-identifiers-and-states"></a><span data-ttu-id="a53eb-151">示例 2：获取具有特定服务标识符和状态的设备的使用权限</span><span class="sxs-lookup"><span data-stu-id="a53eb-151">Example 2: Get usage rights for a device with specific service identifiers and states</span></span>

#### <a name="request"></a><span data-ttu-id="a53eb-152">请求</span><span class="sxs-lookup"><span data-stu-id="a53eb-152">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="a53eb-153">HTTP</span><span class="sxs-lookup"><span data-stu-id="a53eb-153">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_usageright_2"
}
-->
``` http
GET https://graph.microsoft.com/beta/devices/{objectId}/usageRights?$filter=state in ('active', 'suspended') and serviceIdentifier in ('ABCD')
```
# <a name="c"></a>[<span data-ttu-id="a53eb-154">C#</span><span class="sxs-lookup"><span data-stu-id="a53eb-154">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-usageright-2-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a53eb-155">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a53eb-155">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-usageright-2-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a53eb-156">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a53eb-156">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-usageright-2-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a53eb-157">Java</span><span class="sxs-lookup"><span data-stu-id="a53eb-157">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-usageright-2-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


#### <a name="response"></a><span data-ttu-id="a53eb-158">响应</span><span class="sxs-lookup"><span data-stu-id="a53eb-158">Response</span></span>
><span data-ttu-id="a53eb-159">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="a53eb-159">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.usageRight)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#devices('fead5c35-ebc5-47c4-a909-c43b4faf2160')/usageRights",
  "value": [
    {
      "id": "9905e6b1-9040-4926-b028-fdb748c359d6",
      "catalogId": "CFQ7TTC0KCRG:0001",
      "serviceIdentifier": "ABCD",
      "state": "active"
    }
  ]
}
```
