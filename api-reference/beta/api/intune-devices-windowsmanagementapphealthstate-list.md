---
title: 列出 windowsManagementAppHealthStates
description: 列出 windowsManagementAppHealthState 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e8bb672926e0ac067cb385e85b42a71ae26ed13f
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126330"
---
# <a name="list-windowsmanagementapphealthstates"></a><span data-ttu-id="e472f-103">列出 windowsManagementAppHealthStates</span><span class="sxs-lookup"><span data-stu-id="e472f-103">List windowsManagementAppHealthStates</span></span>

<span data-ttu-id="e472f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e472f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e472f-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e472f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e472f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e472f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e472f-107">列出 [windowsManagementAppHealthState 对象的属性和](../resources/intune-devices-windowsmanagementapphealthstate.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="e472f-107">List properties and relationships of the [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e472f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e472f-108">Prerequisites</span></span>
<span data-ttu-id="e472f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e472f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e472f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e472f-111">Permission type</span></span>|<span data-ttu-id="e472f-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e472f-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e472f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e472f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e472f-114">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e472f-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e472f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e472f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e472f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e472f-116">Not supported.</span></span>|
|<span data-ttu-id="e472f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e472f-117">Application</span></span>|<span data-ttu-id="e472f-118">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e472f-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e472f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e472f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsManagementApp/healthStates
```

## <a name="request-headers"></a><span data-ttu-id="e472f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e472f-120">Request headers</span></span>
|<span data-ttu-id="e472f-121">标头</span><span class="sxs-lookup"><span data-stu-id="e472f-121">Header</span></span>|<span data-ttu-id="e472f-122">值</span><span class="sxs-lookup"><span data-stu-id="e472f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e472f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e472f-123">Authorization</span></span>|<span data-ttu-id="e472f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e472f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e472f-125">接受</span><span class="sxs-lookup"><span data-stu-id="e472f-125">Accept</span></span>|<span data-ttu-id="e472f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e472f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e472f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e472f-127">Request body</span></span>
<span data-ttu-id="e472f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e472f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e472f-129">响应</span><span class="sxs-lookup"><span data-stu-id="e472f-129">Response</span></span>
<span data-ttu-id="e472f-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e472f-130">If successful, this method returns a `200 OK` response code and a collection of [windowsManagementAppHealthState](../resources/intune-devices-windowsmanagementapphealthstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e472f-131">示例</span><span class="sxs-lookup"><span data-stu-id="e472f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="e472f-132">请求</span><span class="sxs-lookup"><span data-stu-id="e472f-132">Request</span></span>
<span data-ttu-id="e472f-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e472f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthStates
```

### <a name="response"></a><span data-ttu-id="e472f-134">响应</span><span class="sxs-lookup"><span data-stu-id="e472f-134">Response</span></span>
<span data-ttu-id="e472f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e472f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 410

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsManagementAppHealthState",
      "id": "5c7e50fb-50fb-5c7e-fb50-7e5cfb507e5c",
      "healthState": "healthy",
      "installedVersion": "Installed Version value",
      "lastCheckInDateTime": "2016-12-31T23:59:56.413532-08:00",
      "deviceName": "Device Name value",
      "deviceOSVersion": "Device OSVersion value"
    }
  ]
}
```




