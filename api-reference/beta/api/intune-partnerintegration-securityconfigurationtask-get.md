---
title: 获取 securityConfigurationTask
description: 读取 securityConfigurationTask 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1b952342d8b3efb92506413a9eabb4ca0284e9d2
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49217926"
---
# <a name="get-securityconfigurationtask"></a><span data-ttu-id="a1502-103">获取 securityConfigurationTask</span><span class="sxs-lookup"><span data-stu-id="a1502-103">Get securityConfigurationTask</span></span>

<span data-ttu-id="a1502-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1502-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1502-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a1502-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a1502-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1502-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1502-107">读取 [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="a1502-107">Read properties and relationships of the [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1502-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a1502-108">Prerequisites</span></span>
<span data-ttu-id="a1502-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1502-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1502-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1502-111">Permission type</span></span>|<span data-ttu-id="a1502-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a1502-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1502-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1502-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a1502-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1502-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="a1502-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1502-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1502-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1502-116">Not supported.</span></span>|
|<span data-ttu-id="a1502-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1502-117">Application</span></span>|<span data-ttu-id="a1502-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="a1502-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1502-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1502-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="a1502-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="a1502-120">Optional query parameters</span></span>
<span data-ttu-id="a1502-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="a1502-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="a1502-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1502-122">Request headers</span></span>
|<span data-ttu-id="a1502-123">标头</span><span class="sxs-lookup"><span data-stu-id="a1502-123">Header</span></span>|<span data-ttu-id="a1502-124">值</span><span class="sxs-lookup"><span data-stu-id="a1502-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1502-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1502-125">Authorization</span></span>|<span data-ttu-id="a1502-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a1502-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1502-127">接受</span><span class="sxs-lookup"><span data-stu-id="a1502-127">Accept</span></span>|<span data-ttu-id="a1502-128">application/json</span><span class="sxs-lookup"><span data-stu-id="a1502-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1502-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1502-129">Request body</span></span>
<span data-ttu-id="a1502-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a1502-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a1502-131">响应</span><span class="sxs-lookup"><span data-stu-id="a1502-131">Response</span></span>
<span data-ttu-id="a1502-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a1502-132">If successful, this method returns a `200 OK` response code and [securityConfigurationTask](../resources/intune-partnerintegration-securityconfigurationtask.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1502-133">示例</span><span class="sxs-lookup"><span data-stu-id="a1502-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1502-134">请求</span><span class="sxs-lookup"><span data-stu-id="a1502-134">Request</span></span>
<span data-ttu-id="a1502-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1502-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/deviceAppManagementTasks/{deviceAppManagementTaskId}
```

### <a name="response"></a><span data-ttu-id="a1502-136">响应</span><span class="sxs-lookup"><span data-stu-id="a1502-136">Response</span></span>
<span data-ttu-id="a1502-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1502-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 921

{
  "value": {
    "@odata.type": "#microsoft.graph.securityConfigurationTask",
    "id": "5d630f12-0f12-5d63-120f-635d120f635d",
    "displayName": "Display Name value",
    "description": "Description value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "dueDateTime": "2017-01-01T00:02:18.1994089-08:00",
    "category": "advancedThreatProtection",
    "priority": "high",
    "creator": "Creator value",
    "creatorNotes": "Creator Notes value",
    "assignedTo": "Assigned To value",
    "status": "pending",
    "endpointSecurityPolicy": "antivirus",
    "applicablePlatform": "macOS",
    "endpointSecurityPolicyProfile": "antivirus",
    "insights": "Insights value",
    "managedDeviceCount": 2,
    "intendedSettings": [
      {
        "@odata.type": "microsoft.graph.keyValuePair",
        "name": "Name value",
        "value": "Value value"
      }
    ]
  }
}
```




