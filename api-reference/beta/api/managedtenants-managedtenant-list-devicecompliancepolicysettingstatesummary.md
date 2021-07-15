---
title: 列出 deviceCompliancePolicySettingStateSummary
description: 获取 deviceCompliancePolicySettingStateSummary 对象及其属性的列表。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: ec117e3f93732e3134f6451c83477eb342a98d39
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441997"
---
# <a name="list-devicecompliancepolicysettingstatesummary"></a><span data-ttu-id="5f159-103">列出 deviceCompliancePolicySettingStateSummary</span><span class="sxs-lookup"><span data-stu-id="5f159-103">List deviceCompliancePolicySettingStateSummary</span></span>
<span data-ttu-id="5f159-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="5f159-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5f159-105">获取 [deviceCompliancePolicySettingStateSummary 对象](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) 及其属性的列表。</span><span class="sxs-lookup"><span data-stu-id="5f159-105">Get a list of the [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) objects and their properties.</span></span>

## <a name="permissions"></a><span data-ttu-id="5f159-106">权限</span><span class="sxs-lookup"><span data-stu-id="5f159-106">Permissions</span></span>
<span data-ttu-id="5f159-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f159-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f159-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f159-109">Permission type</span></span>|<span data-ttu-id="5f159-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5f159-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f159-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f159-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5f159-112">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5f159-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="5f159-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f159-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f159-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f159-114">Not supported.</span></span>|
|<span data-ttu-id="5f159-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f159-115">Application</span></span>|<span data-ttu-id="5f159-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f159-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f159-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f159-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummary
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f159-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5f159-118">Optional query parameters</span></span>
<span data-ttu-id="5f159-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="5f159-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f159-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f159-120">Request headers</span></span>
|<span data-ttu-id="5f159-121">名称</span><span class="sxs-lookup"><span data-stu-id="5f159-121">Name</span></span>|<span data-ttu-id="5f159-122">说明</span><span class="sxs-lookup"><span data-stu-id="5f159-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="5f159-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f159-123">Authorization</span></span>|<span data-ttu-id="5f159-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5f159-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f159-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f159-126">Request body</span></span>
<span data-ttu-id="5f159-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5f159-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f159-128">响应</span><span class="sxs-lookup"><span data-stu-id="5f159-128">Response</span></span>

<span data-ttu-id="5f159-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="5f159-129">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicySettingStateSummary](../resources/managedtenants-devicecompliancepolicysettingstatesummary.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5f159-130">示例</span><span class="sxs-lookup"><span data-stu-id="5f159-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5f159-131">请求</span><span class="sxs-lookup"><span data-stu-id="5f159-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="5f159-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="5f159-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_devicecompliancepolicysettingstatesummary"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/deviceCompliancePolicySettingStateSummary
```
# <a name="c"></a>[<span data-ttu-id="5f159-133">C#</span><span class="sxs-lookup"><span data-stu-id="5f159-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-devicecompliancepolicysettingstatesummary-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="5f159-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5f159-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-devicecompliancepolicysettingstatesummary-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5f159-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5f159-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-devicecompliancepolicysettingstatesummary-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5f159-136">Java</span><span class="sxs-lookup"><span data-stu-id="5f159-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-devicecompliancepolicysettingstatesummary-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="5f159-137">响应</span><span class="sxs-lookup"><span data-stu-id="5f159-137">Response</span></span>
><span data-ttu-id="5f159-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="5f159-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedTenants.deviceCompliancePolicySettingStateSummary",
      "id": "9f6922d9-5a58-4f4d-b6e3-708f7659e5b2",
      "tenantId": "String",
      "tenantDisplayName": "String",
      "conflictDeviceCount": "Integer",
      "errorDeviceCount": "Integer",
      "failedDeviceCount": "Integer",
      "intuneAccountId": "String",
      "intuneSettingId": "String",
      "notApplicableDeviceCount": "Integer",
      "pendingDeviceCount": "Integer",
      "policyType": "String",
      "settingName": "String",
      "succeededDeviceCount": "Integer",
      "lastRefreshedDateTime": "String (timestamp)"
    }
  ]
}
```
