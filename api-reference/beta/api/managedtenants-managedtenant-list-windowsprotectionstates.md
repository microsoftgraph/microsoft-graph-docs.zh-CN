---
title: 列出 windowsProtectionStates
description: 获取 windowsProtectionState 对象及其属性的列表。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: ae7de7e8edbb0141df25db91464a45ac1a6499fe
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53442290"
---
# <a name="list-windowsprotectionstates"></a><span data-ttu-id="991be-103">列出 windowsProtectionStates</span><span class="sxs-lookup"><span data-stu-id="991be-103">List windowsProtectionStates</span></span>
<span data-ttu-id="991be-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="991be-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="991be-105">获取 [windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) 对象及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="991be-105">Get a list of the [windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="991be-106">权限</span><span class="sxs-lookup"><span data-stu-id="991be-106">Permissions</span></span>
<span data-ttu-id="991be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="991be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="991be-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="991be-109">Permission type</span></span>|<span data-ttu-id="991be-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="991be-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="991be-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="991be-111">Delegated (work or school account)</span></span>|<span data-ttu-id="991be-112">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="991be-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="991be-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="991be-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="991be-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="991be-114">Not supported.</span></span>|
|<span data-ttu-id="991be-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="991be-115">Application</span></span>|<span data-ttu-id="991be-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="991be-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="991be-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="991be-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/windowsProtectionStates
```

## <a name="optional-query-parameters"></a><span data-ttu-id="991be-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="991be-118">Optional query parameters</span></span>
<span data-ttu-id="991be-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="991be-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="991be-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="991be-120">Request headers</span></span>
|<span data-ttu-id="991be-121">名称</span><span class="sxs-lookup"><span data-stu-id="991be-121">Name</span></span>|<span data-ttu-id="991be-122">说明</span><span class="sxs-lookup"><span data-stu-id="991be-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="991be-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="991be-123">Authorization</span></span>|<span data-ttu-id="991be-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="991be-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="991be-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="991be-126">Request body</span></span>
<span data-ttu-id="991be-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="991be-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="991be-128">响应</span><span class="sxs-lookup"><span data-stu-id="991be-128">Response</span></span>

<span data-ttu-id="991be-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="991be-129">If successful, this method returns a `200 OK` response code and a collection of [windowsProtectionState](../resources/managedtenants-windowsprotectionstate.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="991be-130">示例</span><span class="sxs-lookup"><span data-stu-id="991be-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="991be-131">请求</span><span class="sxs-lookup"><span data-stu-id="991be-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="991be-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="991be-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_windowsprotectionstate"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/windowsProtectionStates
```
# <a name="c"></a>[<span data-ttu-id="991be-133">C#</span><span class="sxs-lookup"><span data-stu-id="991be-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-windowsprotectionstate-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="991be-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="991be-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-windowsprotectionstate-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="991be-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="991be-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-windowsprotectionstate-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="991be-136">Java</span><span class="sxs-lookup"><span data-stu-id="991be-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-windowsprotectionstate-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="991be-137">响应</span><span class="sxs-lookup"><span data-stu-id="991be-137">Response</span></span>
><span data-ttu-id="991be-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="991be-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.windowsProtectionState)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#tenantRelationships/managedTenants/windowsProtectionStates",
    "value": [
        {
            "id": "34298981-4fc8-4974-9486-c8909ed1521b_95378ac4-eded-4671-8fa2-4e42e5de3463",
            "managedDeviceId": "95378ac4-eded-4671-8fa2-4e42e5de3463",
            "managedDeviceName": "vm11",
            "malwareProtectionEnabled": true,
            "managedDeviceHealthState": "Clean",
            "realTimeProtectionEnabled": true,
            "networkInspectionSystemEnabled": true,
            "quickScanOverdue": false,
            "fullScanOverdue": false,
            "signatureUpdateOverdue": false,
            "rebootRequired": false,
            "attentionRequired": false,
            "fullScanRequired": false,
            "engineVersion": "1.1.18300.4",
            "signatureVersion": "1.343.642.0",
            "antiMalwareVersion": "4.18.2106.6",
            "lastQuickScanDateTime": "2021-06-24T14:50:28Z",
            "lastFullScanDateTime": null,
            "lastQuickScanSignatureVersion": "1.341.1288.0",
            "lastFullScanSignatureVersion": "0.0.0.0",
            "lastReportedDateTime": "2021-07-09T14:43:45Z",
            "devicePropertiesRefreshTime": "2021-07-09T14:44:28Z",
            "deviceDeleted": false,
            "lastRefreshedDateTime": "2021-07-11T02:02:35.9816065Z",
            "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
            "tenantDisplayName": "Fourth Coffee",
            "devicePropertiesRefreshDateTime": "2021-07-09T14:44:28Z"
        },
        {
            "id": "38227791-a88b-4fcc-81c5-58cf77668320_49ed91f1-32ac-4881-9c1b-b709ba29e31b",
            "managedDeviceId": "49ed91f1-32ac-4881-9c1b-b709ba29e31b",
            "managedDeviceName": "VM4511",
            "malwareProtectionEnabled": true,
            "managedDeviceHealthState": "Clean",
            "realTimeProtectionEnabled": true,
            "networkInspectionSystemEnabled": true,
            "quickScanOverdue": false,
            "fullScanOverdue": false,
            "signatureUpdateOverdue": false,
            "rebootRequired": false,
            "attentionRequired": false,
            "fullScanRequired": false,
            "engineVersion": "1.1.18300.4",
            "signatureVersion": "1.343.618.0",
            "antiMalwareVersion": "4.18.2105.5",
            "lastQuickScanDateTime": "2021-06-21T15:05:41Z",
            "lastFullScanDateTime": "2021-04-19T20:03:26Z",
            "lastQuickScanSignatureVersion": "1.341.1157.0",
            "lastFullScanSignatureVersion": "1.303.25.0",
            "lastReportedDateTime": "2021-07-09T14:43:52Z",
            "devicePropertiesRefreshTime": "2021-07-09T14:44:28Z",
            "deviceDeleted": false,
            "lastRefreshedDateTime": "2021-07-11T02:02:35.9816065Z",
            "tenantId": "38227791-a88b-4fcc-81c5-58cf77668320",
            "tenantDisplayName": "Consolidated Messenger",
            "devicePropertiesRefreshDateTime": "2021-07-09T14:44:28Z"
        }
    ]
}
```
