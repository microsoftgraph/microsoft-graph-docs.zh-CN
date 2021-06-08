---
title: 获取 managedDeviceMobileAppConfigurationDeviceStatus
description: 读取 managedDeviceMobileAppConfigurationDeviceStatus 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 63b3ebe2fc98c8ea5d628b08c7e7050a043d3fd4
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52759866"
---
# <a name="get-manageddevicemobileappconfigurationdevicestatus"></a><span data-ttu-id="43741-103">获取 managedDeviceMobileAppConfigurationDeviceStatus</span><span class="sxs-lookup"><span data-stu-id="43741-103">Get managedDeviceMobileAppConfigurationDeviceStatus</span></span>

<span data-ttu-id="43741-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="43741-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="43741-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="43741-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="43741-106">读取 [managedDeviceMobileAppConfigurationDeviceStatus 对象的属性和](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="43741-106">Read properties and relationships of the [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="43741-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="43741-107">Prerequisites</span></span>
<span data-ttu-id="43741-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="43741-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="43741-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="43741-110">Permission type</span></span>|<span data-ttu-id="43741-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="43741-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="43741-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="43741-112">Delegated (work or school account)</span></span>|<span data-ttu-id="43741-113">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43741-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="43741-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="43741-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="43741-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="43741-115">Not supported.</span></span>|
|<span data-ttu-id="43741-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="43741-116">Application</span></span>|<span data-ttu-id="43741-117">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="43741-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="43741-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="43741-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="43741-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="43741-119">Optional query parameters</span></span>
<span data-ttu-id="43741-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="43741-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="43741-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="43741-121">Request headers</span></span>
|<span data-ttu-id="43741-122">标头</span><span class="sxs-lookup"><span data-stu-id="43741-122">Header</span></span>|<span data-ttu-id="43741-123">值</span><span class="sxs-lookup"><span data-stu-id="43741-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="43741-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="43741-124">Authorization</span></span>|<span data-ttu-id="43741-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="43741-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="43741-126">接受</span><span class="sxs-lookup"><span data-stu-id="43741-126">Accept</span></span>|<span data-ttu-id="43741-127">application/json</span><span class="sxs-lookup"><span data-stu-id="43741-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="43741-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="43741-128">Request body</span></span>
<span data-ttu-id="43741-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="43741-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="43741-130">响应</span><span class="sxs-lookup"><span data-stu-id="43741-130">Response</span></span>
<span data-ttu-id="43741-131">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="43741-131">If successful, this method returns a `200 OK` response code and [managedDeviceMobileAppConfigurationDeviceStatus](../resources/intune-apps-manageddevicemobileappconfigurationdevicestatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="43741-132">示例</span><span class="sxs-lookup"><span data-stu-id="43741-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="43741-133">请求</span><span class="sxs-lookup"><span data-stu-id="43741-133">Request</span></span>
<span data-ttu-id="43741-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="43741-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/deviceStatuses/{managedDeviceMobileAppConfigurationDeviceStatusId}
```

### <a name="response"></a><span data-ttu-id="43741-135">响应</span><span class="sxs-lookup"><span data-stu-id="43741-135">Response</span></span>
<span data-ttu-id="43741-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="43741-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 531

{
  "value": {
    "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationDeviceStatus",
    "id": "477d3651-3651-477d-5136-7d4751367d47",
    "deviceDisplayName": "Device Display Name value",
    "userName": "User Name value",
    "deviceModel": "Device Model value",
    "complianceGracePeriodExpirationDateTime": "2016-12-31T23:56:44.951111-08:00",
    "status": "notApplicable",
    "lastReportedDateTime": "2017-01-01T00:00:17.7769392-08:00",
    "userPrincipalName": "User Principal Name value"
  }
}
```




