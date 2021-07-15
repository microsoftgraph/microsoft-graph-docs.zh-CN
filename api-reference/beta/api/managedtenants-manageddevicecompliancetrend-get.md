---
title: 获取 managedDeviceComplianceTrend
description: 读取 managedDeviceComplianceTrend 对象的属性和关系。
author: isaiahwilliams
localization_priority: Normal
ms.prod: microsoft-365-lighthouse
doc_type: apiPageType
ms.openlocfilehash: 21e6583fe4e4f5840409e4153d47b0a945bd3ba9
ms.sourcegitcommit: 486fe9c77d4d89c5416bb83e8c716e6918c47370
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/15/2021
ms.locfileid: "53441611"
---
# <a name="get-manageddevicecompliancetrend"></a><span data-ttu-id="f4d54-103">获取 managedDeviceComplianceTrend</span><span class="sxs-lookup"><span data-stu-id="f4d54-103">Get managedDeviceComplianceTrend</span></span>
<span data-ttu-id="f4d54-104">命名空间：microsoft.graph.managedTenants</span><span class="sxs-lookup"><span data-stu-id="f4d54-104">Namespace: microsoft.graph.managedTenants</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4d54-105">读取 [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f4d54-105">Read the properties and relationships of a [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="f4d54-106">权限</span><span class="sxs-lookup"><span data-stu-id="f4d54-106">Permissions</span></span>
<span data-ttu-id="f4d54-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f4d54-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f4d54-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f4d54-109">Permission type</span></span>|<span data-ttu-id="f4d54-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f4d54-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f4d54-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f4d54-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f4d54-112">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f4d54-112">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f4d54-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f4d54-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f4d54-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4d54-114">Not supported.</span></span>|
|<span data-ttu-id="f4d54-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f4d54-115">Application</span></span>|<span data-ttu-id="f4d54-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f4d54-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f4d54-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f4d54-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /tenantRelationships/managedTenants/managedDeviceComplianceTrends/{managedDeviceComplianceTrendId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="f4d54-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="f4d54-118">Optional query parameters</span></span>
<span data-ttu-id="f4d54-119">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应，包括 `$apply` `$count` `$filter` `$orderBy` `$select` 、、 `$skip` 和 `$top` 。</span><span class="sxs-lookup"><span data-stu-id="f4d54-119">This method supports the [OData query parameters](/graph/query-parameters) to help customize the response, including `$apply`, `$count`, `$filter`, `$orderBy`, `$select`, `$skip`, and `$top`.</span></span>

## <a name="request-headers"></a><span data-ttu-id="f4d54-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f4d54-120">Request headers</span></span>
|<span data-ttu-id="f4d54-121">名称</span><span class="sxs-lookup"><span data-stu-id="f4d54-121">Name</span></span>|<span data-ttu-id="f4d54-122">说明</span><span class="sxs-lookup"><span data-stu-id="f4d54-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f4d54-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f4d54-123">Authorization</span></span>|<span data-ttu-id="f4d54-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f4d54-p102">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f4d54-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f4d54-126">Request body</span></span>
<span data-ttu-id="f4d54-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f4d54-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f4d54-128">响应</span><span class="sxs-lookup"><span data-stu-id="f4d54-128">Response</span></span>

<span data-ttu-id="f4d54-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f4d54-129">If successful, this method returns a `200 OK` response code and a [managedDeviceComplianceTrend](../resources/managedtenants-manageddevicecompliancetrend.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f4d54-130">示例</span><span class="sxs-lookup"><span data-stu-id="f4d54-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f4d54-131">请求</span><span class="sxs-lookup"><span data-stu-id="f4d54-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f4d54-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="f4d54-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "get_manageddevicecompliancetrend"
}
-->
``` http
GET https://graph.microsoft.com/beta/tenantRelationships/managedTenants/managedDeviceComplianceTrends/{managedDeviceComplianceTrendId}
```
# <a name="c"></a>[<span data-ttu-id="f4d54-133">C#</span><span class="sxs-lookup"><span data-stu-id="f4d54-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/get-manageddevicecompliancetrend-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f4d54-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f4d54-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/get-manageddevicecompliancetrend-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f4d54-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f4d54-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/get-manageddevicecompliancetrend-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f4d54-136">Java</span><span class="sxs-lookup"><span data-stu-id="f4d54-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/get-manageddevicecompliancetrend-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f4d54-137">响应</span><span class="sxs-lookup"><span data-stu-id="f4d54-137">Response</span></span>
><span data-ttu-id="f4d54-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f4d54-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.managedTenants.managedDeviceComplianceTrend"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.type": "#microsoft.graph.managedTenants.managedDeviceComplianceTrend",
  "id": "34298981-4fc8-4974-9486-c8909ed1521b_2021-07-11T00:00:00Z",
  "tenantDisplayName": "Fourth Coffee",
  "tenantId": "34298981-4fc8-4974-9486-c8909ed1521b",
  "unknownDeviceCount": 2,
  "compliantDeviceCount": 0,
  "noncompliantDeviceCount": 41,
  "errorDeviceCount": 1,
  "inGracePeriodDeviceCount": 0,
  "configManagerDeviceCount": 0,
  "totalDeviceCount": 44,
  "countDateTime": "2021-07-11T00:00:00Z"
}
```
