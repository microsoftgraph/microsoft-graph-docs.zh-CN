---
title: 列出 deviceManagementCachedReportConfigurations
description: 列出 deviceManagementCachedReportConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 9116c3a9fac85ff780df14ca58d00cfae43b9cb7
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698300"
---
# <a name="list-devicemanagementcachedreportconfigurations"></a><span data-ttu-id="145c0-103">列出 deviceManagementCachedReportConfigurations</span><span class="sxs-lookup"><span data-stu-id="145c0-103">List deviceManagementCachedReportConfigurations</span></span>

<span data-ttu-id="145c0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="145c0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="145c0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="145c0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="145c0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="145c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="145c0-107">列出 [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="145c0-107">List properties and relationships of the [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="145c0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="145c0-108">Prerequisites</span></span>
<span data-ttu-id="145c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="145c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="145c0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="145c0-111">Permission type</span></span>|<span data-ttu-id="145c0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="145c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="145c0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="145c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="145c0-114">Devicemanagementconfiguration.readwrite.all、Devicemanagementconfiguration.readwrite.all、Devicemanagementapps.readwrite.all、all、Devicemanagementapps.readwrite.all、all、devicemanagementmanageddevices.readwrite.all、all、devicemanagementmanageddevices.readwrite.all、all 和 Read. all。 All</span><span class="sxs-lookup"><span data-stu-id="145c0-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="145c0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="145c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="145c0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="145c0-116">Not supported.</span></span>|
|<span data-ttu-id="145c0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="145c0-117">Application</span></span>|<span data-ttu-id="145c0-118">Devicemanagementconfiguration.readwrite.all、Devicemanagementconfiguration.readwrite.all、Devicemanagementapps.readwrite.all、all、Devicemanagementapps.readwrite.all、all、devicemanagementmanageddevices.readwrite.all、all、devicemanagementmanageddevices.readwrite.all、all 和 Read. all。 All</span><span class="sxs-lookup"><span data-stu-id="145c0-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="145c0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="145c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/cachedReportConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="145c0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="145c0-120">Request headers</span></span>
|<span data-ttu-id="145c0-121">标头</span><span class="sxs-lookup"><span data-stu-id="145c0-121">Header</span></span>|<span data-ttu-id="145c0-122">值</span><span class="sxs-lookup"><span data-stu-id="145c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="145c0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="145c0-123">Authorization</span></span>|<span data-ttu-id="145c0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="145c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="145c0-125">接受</span><span class="sxs-lookup"><span data-stu-id="145c0-125">Accept</span></span>|<span data-ttu-id="145c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="145c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="145c0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="145c0-127">Request body</span></span>
<span data-ttu-id="145c0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="145c0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="145c0-129">响应</span><span class="sxs-lookup"><span data-stu-id="145c0-129">Response</span></span>
<span data-ttu-id="145c0-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="145c0-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementCachedReportConfiguration](../resources/intune-reporting-devicemanagementcachedreportconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="145c0-131">示例</span><span class="sxs-lookup"><span data-stu-id="145c0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="145c0-132">请求</span><span class="sxs-lookup"><span data-stu-id="145c0-132">Request</span></span>
<span data-ttu-id="145c0-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="145c0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/cachedReportConfigurations
```

### <a name="response"></a><span data-ttu-id="145c0-134">响应</span><span class="sxs-lookup"><span data-stu-id="145c0-134">Response</span></span>
<span data-ttu-id="145c0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="145c0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 556

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementCachedReportConfiguration",
      "id": "46947722-7722-4694-2277-944622779446",
      "reportName": "Report Name value",
      "filter": "Filter value",
      "select": [
        "Select value"
      ],
      "orderBy": [
        "Order By value"
      ],
      "metadata": "Metadata value",
      "status": "notStarted",
      "lastRefreshDateTime": "2016-12-31T23:58:49.97047-08:00",
      "expirationDateTime": "2016-12-31T23:57:57.2481234-08:00"
    }
  ]
}
```





