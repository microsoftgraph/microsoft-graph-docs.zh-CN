---
title: 列出 managedDeviceCompliances
description: 获取 managedDeviceCompliance 对象及其属性的列表。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 0376c59d5a43f4c5d8b4dc9aa4429fcbfee42d85
ms.sourcegitcommit: e372382019f1a136543eadab02ba70af3921e098
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/13/2021
ms.locfileid: "53402030"
---
# <a name="list-manageddevicecompliances"></a><span data-ttu-id="ed491-103">列出 managedDeviceCompliances</span><span class="sxs-lookup"><span data-stu-id="ed491-103">List managedDeviceCompliances</span></span>
<span data-ttu-id="ed491-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="ed491-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed491-105">获取 [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="ed491-105">Get a list of the [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="ed491-106">权限</span><span class="sxs-lookup"><span data-stu-id="ed491-106">Permissions</span></span>
<span data-ttu-id="ed491-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed491-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ed491-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed491-109">Permission type</span></span>|<span data-ttu-id="ed491-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed491-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ed491-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed491-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ed491-112">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ed491-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="ed491-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed491-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed491-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed491-114">Not supported.</span></span>|
|<span data-ttu-id="ed491-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed491-115">Application</span></span>|<span data-ttu-id="ed491-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed491-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed491-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed491-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managedDeviceCompliances
```

## <a name="optional-query-parameters"></a><span data-ttu-id="ed491-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="ed491-118">Optional query parameters</span></span>
<span data-ttu-id="ed491-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="ed491-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="ed491-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed491-120">Request headers</span></span>
|<span data-ttu-id="ed491-121">名称</span><span class="sxs-lookup"><span data-stu-id="ed491-121">Name</span></span>|<span data-ttu-id="ed491-122">说明</span><span class="sxs-lookup"><span data-stu-id="ed491-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="ed491-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed491-123">Authorization</span></span>|<span data-ttu-id="ed491-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ed491-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed491-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed491-126">Request body</span></span>
<span data-ttu-id="ed491-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ed491-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ed491-128">响应</span><span class="sxs-lookup"><span data-stu-id="ed491-128">Response</span></span>

<span data-ttu-id="ed491-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="ed491-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceCompliance](../resources/managedtenants-manageddevicecompliance.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="ed491-130">示例</span><span class="sxs-lookup"><span data-stu-id="ed491-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="ed491-131">请求</span><span class="sxs-lookup"><span data-stu-id="ed491-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_manageddevicecompliance"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managedDeviceCompliances
```


### <a name="response"></a><span data-ttu-id="ed491-132">响应</span><span class="sxs-lookup"><span data-stu-id="ed491-132">Response</span></span>
><span data-ttu-id="ed491-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="ed491-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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
