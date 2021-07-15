---
title: 列出 managedDeviceCompliances
description: 获取 managedDeviceCompliance 对象及其属性的列表。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 4d0b9a47ee7d989d9e737914855cc1053509568e
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442017"
---
# <a name="list-manageddevicecompliances"></a><span data-ttu-id="accde-103">列出 managedDeviceCompliances</span><span class="sxs-lookup"><span data-stu-id="accde-103">List managedDeviceCompliances</span></span>
<span data-ttu-id="accde-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="accde-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="accde-105">获取 [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="accde-105">Get a list of the [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="accde-106">权限</span><span class="sxs-lookup"><span data-stu-id="accde-106">Permissions</span></span>
<span data-ttu-id="accde-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="accde-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="accde-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="accde-109">Permission type</span></span>|<span data-ttu-id="accde-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="accde-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="accde-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="accde-111">Delegated (work or school account)</span></span>|<span data-ttu-id="accde-112">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="accde-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="accde-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="accde-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="accde-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="accde-114">Not supported.</span></span>|
|<span data-ttu-id="accde-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="accde-115">Application</span></span>|<span data-ttu-id="accde-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="accde-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="accde-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="accde-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managedDeviceCompliances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="accde-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="accde-118">Optional query parameters</span></span>
<span data-ttu-id="accde-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="accde-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="accde-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="accde-120">Request headers</span></span>
|<span data-ttu-id="accde-121">名称</span><span class="sxs-lookup"><span data-stu-id="accde-121">Name</span></span>|<span data-ttu-id="accde-122">说明</span><span class="sxs-lookup"><span data-stu-id="accde-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="accde-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="accde-123">Authorization</span></span>|<span data-ttu-id="accde-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="accde-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="accde-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="accde-126">Request body</span></span>
<span data-ttu-id="accde-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="accde-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="accde-128">响应</span><span class="sxs-lookup"><span data-stu-id="accde-128">Response</span></span>

<span data-ttu-id="accde-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="accde-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="accde-130">示例</span><span class="sxs-lookup"><span data-stu-id="accde-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="accde-131">请求</span><span class="sxs-lookup"><span data-stu-id="accde-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="accde-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="accde-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_manageddevicecompliance"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managedDeviceCompliances
```
# <a name="c"></a>[<span data-ttu-id="accde-133">C#</span><span class="sxs-lookup"><span data-stu-id="accde-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-manageddevicecompliance-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="accde-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="accde-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-manageddevicecompliance-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="accde-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="accde-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-manageddevicecompliance-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="accde-136">Java</span><span class="sxs-lookup"><span data-stu-id="accde-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-manageddevicecompliance-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="accde-137">响应</span><span class="sxs-lookup"><span data-stu-id="accde-137">Response</span></span>
><span data-ttu-id="accde-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="accde-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.managedDeviceCompliance)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#managedDeviceCompliances",
  "value": [
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320_6dd4fe4b-5ea2-4ab2-8ac4-7dd2995f1649",
      "managedDeviceId": "6dd4fe4b-5ea2-4ab2-8ac4-7dd2995f1649",
      "managedDeviceName": "VM2688",
      "complianceStatus": "Noncompliant",
      "osDescription": "Windows",
      "osVersion": "10.0.19042.1083",
      "lastSyncDateTime": "2021-07-09T14:38:56.379702Z",
      "ownerType": "Company",
      "model": "Virtual Machine",
      "manufacturer": "Microsoft Corporation",
      "inGracePeriodUntilDateTime": "2021-06-14T14:35:24.8225Z",
      "lastRefreshedDateTime": "2021-07-11T07:03:54.0326474Z",
      "deviceType": "WindowsRT",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantDisplayName": "Consolidated Messenger"
    },
    {
      "id": "38227791-a88b-4fcc-81c5-58cf77668320_49ed91f1-32ac-4881-9c1b-b709ba29e31b",
      "managedDeviceId": "49ed91f1-32ac-4881-9c1b-b709ba29e31b",
      "managedDeviceName": "VM4511",
      "complianceStatus": "Noncompliant",
      "osDescription": "Windows",
      "osVersion": "10.0.19042.1052",
      "lastSyncDateTime": "2021-07-09T14:41:57.8785122Z",
      "ownerType": "Company",
      "model": "Virtual Machine",
      "manufacturer": "Microsoft Corporation",
      "inGracePeriodUntilDateTime": "2021-06-14T14:36:09.1851Z",
      "lastRefreshedDateTime": "2021-07-11T06:53:35.8484421Z",
      "deviceType": "WindowsRT",
      "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
      "tenantDisplayName": "Consolidated Messenger"
    }
  ]
}
```
