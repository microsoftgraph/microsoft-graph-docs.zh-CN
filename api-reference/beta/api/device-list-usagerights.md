---
title: 列出设备 usageRights
description: 检索设备的 usageRights 对象列表。
author: jeeshnair
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 41c6cea58577b0d03dfd32086bdf6d1daddf716c
ms.sourcegitcommit: 9a5facff47a8d4e05ecd2c6cd68294a948c47c4d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2021
ms.locfileid: "49944346"
---
# <a name="list-device-usagerights"></a><span data-ttu-id="6af12-103">列出设备 usageRights</span><span class="sxs-lookup"><span data-stu-id="6af12-103">List device usageRights</span></span>
<span data-ttu-id="6af12-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6af12-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="6af12-105">检索给定设备的 [usageRight](../resources/usageright.md) 对象列表。</span><span class="sxs-lookup"><span data-stu-id="6af12-105">Retrieve a list of [usageRight](../resources/usageright.md) objects for a given device.</span></span>

## <a name="permissions"></a><span data-ttu-id="6af12-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="6af12-106">Permissions</span></span>
<span data-ttu-id="6af12-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6af12-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6af12-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6af12-109">Permission type</span></span>|<span data-ttu-id="6af12-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6af12-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6af12-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6af12-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6af12-112">Device.Read.All、Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6af12-112">Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>|
|<span data-ttu-id="6af12-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6af12-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6af12-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6af12-114">Not supported.</span></span>|
|<span data-ttu-id="6af12-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6af12-115">Application</span></span>|<span data-ttu-id="6af12-116">Device.Read.All、Device.ReadWrite.All、Directory.Read.All、Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6af12-116">Device.Read.All, Device.ReadWrite.All, Directory.Read.All, Directory.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6af12-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6af12-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /devices/{objectId}/usageRights
```

## <a name="optional-query-parameters"></a><span data-ttu-id="6af12-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="6af12-118">Optional query parameters</span></span>
<span data-ttu-id="6af12-119">此 API 支持 $filter [OData 查询参数](/graph/query-parameters)。</span><span class="sxs-lookup"><span data-stu-id="6af12-119">This API supports the $filter [OData query parameter](/graph/query-parameters).</span></span> <span data-ttu-id="6af12-120">支持以下$filter模式：</span><span class="sxs-lookup"><span data-stu-id="6af12-120">The following patterns of $filter are supported:</span></span>

- <span data-ttu-id="6af12-121">$filter = state eq 'value'</span><span class="sxs-lookup"><span data-stu-id="6af12-121">$filter = state eq 'value'</span></span>
- <span data-ttu-id="6af12-122">$filter = serviceIdentifier eq 'value'</span><span class="sxs-lookup"><span data-stu-id="6af12-122">$filter = serviceIdentifier eq 'value'</span></span>
- <span data-ttu-id="6af12-123">$filter = state eq 'value' and serviceIdentifier eq 'value'</span><span class="sxs-lookup"><span data-stu-id="6af12-123">$filter = state eq 'value' and serviceIdentifier eq 'value'</span></span>
- <span data-ttu-id="6af12-124">$filter = ("value1"中的状态，"value2") </span><span class="sxs-lookup"><span data-stu-id="6af12-124">$filter = state in ('value1', 'value2')</span></span>
- <span data-ttu-id="6af12-125">$filter =serviceIdentifier in ('value1'， 'value2') </span><span class="sxs-lookup"><span data-stu-id="6af12-125">$filter = serviceIdentifier in ('value1', 'value2')</span></span>
- <span data-ttu-id="6af12-126">$filter = ("value1"、"value2") 和 ("value1"中的 serviceIdentifier 中的状态，"value2") </span><span class="sxs-lookup"><span data-stu-id="6af12-126">$filter = state in ('value1', 'value2') and serviceIdentifier in ('value1', 'value2')</span></span>

## <a name="request-headers"></a><span data-ttu-id="6af12-127">请求标头</span><span class="sxs-lookup"><span data-stu-id="6af12-127">Request headers</span></span>
|<span data-ttu-id="6af12-128">名称</span><span class="sxs-lookup"><span data-stu-id="6af12-128">Name</span></span>|<span data-ttu-id="6af12-129">说明</span><span class="sxs-lookup"><span data-stu-id="6af12-129">Description</span></span>|
|:---|:---|
|<span data-ttu-id="6af12-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="6af12-130">Authorization</span></span>|<span data-ttu-id="6af12-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="6af12-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="6af12-133">odata.maxpagesize</span><span class="sxs-lookup"><span data-stu-id="6af12-133">odata.maxpagesize</span></span>|<span data-ttu-id="6af12-134">设置最大结果页大小限制。</span><span class="sxs-lookup"><span data-stu-id="6af12-134">Set the max result page size pereference.</span></span> <span data-ttu-id="6af12-135">可选。</span><span class="sxs-lookup"><span data-stu-id="6af12-135">Optional.</span></span>|

## <a name="request-body"></a><span data-ttu-id="6af12-136">请求正文</span><span class="sxs-lookup"><span data-stu-id="6af12-136">Request body</span></span>
<span data-ttu-id="6af12-137">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6af12-137">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6af12-138">响应</span><span class="sxs-lookup"><span data-stu-id="6af12-138">Response</span></span>
<span data-ttu-id="6af12-139">如果成功，此方法在 `200 OK` 响应正文中返回响应代码和 [usageRight](../resources/usageright.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6af12-139">If successful, this method returns a `200 OK` response code and a collection of [usageRight](../resources/usageright.md) objects in the response body.</span></span>

<span data-ttu-id="6af12-140">此外，如果响应中有更多的页面，则返回 @odata.nextLink。</span><span class="sxs-lookup"><span data-stu-id="6af12-140">Additionally, if there are more pages in the response an @odata.nextLink is returned.</span></span>

## <a name="examples"></a><span data-ttu-id="6af12-141">示例</span><span class="sxs-lookup"><span data-stu-id="6af12-141">Examples</span></span>

### <a name="example-1-get-all-usage-rights-for-a-device"></a><span data-ttu-id="6af12-142">示例 1：获取设备的所有使用权限</span><span class="sxs-lookup"><span data-stu-id="6af12-142">Example 1: Get all usage rights for a device</span></span>
 
#### <a name="request"></a><span data-ttu-id="6af12-143">请求</span><span class="sxs-lookup"><span data-stu-id="6af12-143">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_usageright"
}
-->
``` http
GET https://graph.microsoft.com/beta/devices/{objectId}/usageRights
```

#### <a name="response"></a><span data-ttu-id="6af12-144">响应</span><span class="sxs-lookup"><span data-stu-id="6af12-144">Response</span></span>
><span data-ttu-id="6af12-145">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6af12-145">**Note:** The response object shown here might be shortened for readability.</span></span>
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

### <a name="example-2-get-usage-rights-for-a-device-with-specific-service-identifiers-and-states"></a><span data-ttu-id="6af12-146">示例 2：获取具有特定服务标识符和状态的设备的使用权限</span><span class="sxs-lookup"><span data-stu-id="6af12-146">Example 2: Get usage rights for a device with specific service identifiers and states</span></span>

#### <a name="request"></a><span data-ttu-id="6af12-147">请求</span><span class="sxs-lookup"><span data-stu-id="6af12-147">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_usageright"
}
-->
``` http
GET https://graph.microsoft.com/beta/devices/{objectId}/usageRights?$filter=state in ('active', 'suspended') and serviceIdentifier in ('ABCD')
```

#### <a name="response"></a><span data-ttu-id="6af12-148">响应</span><span class="sxs-lookup"><span data-stu-id="6af12-148">Response</span></span>
><span data-ttu-id="6af12-149">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="6af12-149">**Note:** The response object shown here might be shortened for readability.</span></span>
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