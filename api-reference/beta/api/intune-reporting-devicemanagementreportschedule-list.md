---
title: 列出 deviceManagementReportSchedules
description: 列出 deviceManagementReportSchedule 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d99a8fb917444e4dca6b248dfcc6ca199c8541e3
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49307736"
---
# <a name="list-devicemanagementreportschedules"></a><span data-ttu-id="b3c9b-103">列出 deviceManagementReportSchedules</span><span class="sxs-lookup"><span data-stu-id="b3c9b-103">List deviceManagementReportSchedules</span></span>

<span data-ttu-id="b3c9b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b3c9b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b3c9b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b3c9b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b3c9b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b3c9b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b3c9b-107">列出 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b3c9b-107">List properties and relationships of the [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b3c9b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b3c9b-108">Prerequisites</span></span>
<span data-ttu-id="b3c9b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3c9b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3c9b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3c9b-111">Permission type</span></span>|<span data-ttu-id="b3c9b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b3c9b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b3c9b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3c9b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b3c9b-114">Devicemanagementconfiguration.readwrite.all、Devicemanagementconfiguration.readwrite.all、Devicemanagementapps.readwrite.all、all、Devicemanagementapps.readwrite.all、all、devicemanagementmanageddevices.readwrite.all、all、devicemanagementmanageddevices.readwrite.all、all 和 Read. all。 All</span><span class="sxs-lookup"><span data-stu-id="b3c9b-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b3c9b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3c9b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b3c9b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b3c9b-116">Not supported.</span></span>|
|<span data-ttu-id="b3c9b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3c9b-117">Application</span></span>|<span data-ttu-id="b3c9b-118">Devicemanagementconfiguration.readwrite.all、Devicemanagementconfiguration.readwrite.all、Devicemanagementapps.readwrite.all、all、Devicemanagementapps.readwrite.all、all、devicemanagementmanageddevices.readwrite.all、all、devicemanagementmanageddevices.readwrite.all、all 和 Read. all。 All</span><span class="sxs-lookup"><span data-stu-id="b3c9b-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All, DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All, DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b3c9b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3c9b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/reports/reportSchedules
```

## <a name="request-headers"></a><span data-ttu-id="b3c9b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3c9b-120">Request headers</span></span>
|<span data-ttu-id="b3c9b-121">标头</span><span class="sxs-lookup"><span data-stu-id="b3c9b-121">Header</span></span>|<span data-ttu-id="b3c9b-122">值</span><span class="sxs-lookup"><span data-stu-id="b3c9b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b3c9b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3c9b-123">Authorization</span></span>|<span data-ttu-id="b3c9b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b3c9b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b3c9b-125">接受</span><span class="sxs-lookup"><span data-stu-id="b3c9b-125">Accept</span></span>|<span data-ttu-id="b3c9b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b3c9b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3c9b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3c9b-127">Request body</span></span>
<span data-ttu-id="b3c9b-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b3c9b-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3c9b-129">响应</span><span class="sxs-lookup"><span data-stu-id="b3c9b-129">Response</span></span>
<span data-ttu-id="b3c9b-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b3c9b-130">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementReportSchedule](../resources/intune-reporting-devicemanagementreportschedule.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b3c9b-131">示例</span><span class="sxs-lookup"><span data-stu-id="b3c9b-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b3c9b-132">请求</span><span class="sxs-lookup"><span data-stu-id="b3c9b-132">Request</span></span>
<span data-ttu-id="b3c9b-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b3c9b-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/reports/reportSchedules
```

### <a name="response"></a><span data-ttu-id="b3c9b-134">响应</span><span class="sxs-lookup"><span data-stu-id="b3c9b-134">Response</span></span>
<span data-ttu-id="b3c9b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b3c9b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 701

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementReportSchedule",
      "id": "00bb9785-9785-00bb-8597-bb008597bb00",
      "reportScheduleName": "Report Schedule Name value",
      "subject": "Subject value",
      "emails": [
        "Emails value"
      ],
      "recurrence": "daily",
      "startDateTime": "2016-12-31T23:58:46.7156189-08:00",
      "endDateTime": "2017-01-01T00:03:30.9241974-08:00",
      "userId": "User Id value",
      "reportName": "Report Name value",
      "filter": "Filter value",
      "select": [
        "Select value"
      ],
      "orderBy": [
        "Order By value"
      ],
      "format": "pdf"
    }
  ]
}
```




