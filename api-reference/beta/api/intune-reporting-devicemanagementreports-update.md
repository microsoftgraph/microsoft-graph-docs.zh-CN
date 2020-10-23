---
title: 更新 deviceManagementReports
description: 更新 deviceManagementReports 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a56d5495f714c639a699aa1d5ccebb81ea2b7c83
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48698132"
---
# <a name="update-devicemanagementreports"></a><span data-ttu-id="02078-103">更新 deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="02078-103">Update deviceManagementReports</span></span>

<span data-ttu-id="02078-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="02078-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="02078-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="02078-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="02078-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="02078-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="02078-107">更新 [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="02078-107">Update the properties of a [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="02078-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="02078-108">Prerequisites</span></span>
<span data-ttu-id="02078-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="02078-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="02078-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="02078-111">Permission type</span></span>|<span data-ttu-id="02078-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="02078-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="02078-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="02078-113">Delegated (work or school account)</span></span>|<span data-ttu-id="02078-114">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="02078-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="02078-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="02078-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="02078-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="02078-116">Not supported.</span></span>|
|<span data-ttu-id="02078-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="02078-117">Application</span></span>|<span data-ttu-id="02078-118">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="02078-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="02078-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="02078-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports
```

## <a name="request-headers"></a><span data-ttu-id="02078-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="02078-120">Request headers</span></span>
|<span data-ttu-id="02078-121">标头</span><span class="sxs-lookup"><span data-stu-id="02078-121">Header</span></span>|<span data-ttu-id="02078-122">值</span><span class="sxs-lookup"><span data-stu-id="02078-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="02078-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="02078-123">Authorization</span></span>|<span data-ttu-id="02078-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="02078-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="02078-125">接受</span><span class="sxs-lookup"><span data-stu-id="02078-125">Accept</span></span>|<span data-ttu-id="02078-126">application/json</span><span class="sxs-lookup"><span data-stu-id="02078-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="02078-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="02078-127">Request body</span></span>
<span data-ttu-id="02078-128">在请求正文中，提供 [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="02078-128">In the request body, supply a JSON representation for the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

<span data-ttu-id="02078-129">下表显示创建 [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="02078-129">The following table shows the properties that are required when you create the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md).</span></span>

|<span data-ttu-id="02078-130">属性</span><span class="sxs-lookup"><span data-stu-id="02078-130">Property</span></span>|<span data-ttu-id="02078-131">类型</span><span class="sxs-lookup"><span data-stu-id="02078-131">Type</span></span>|<span data-ttu-id="02078-132">说明</span><span class="sxs-lookup"><span data-stu-id="02078-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="02078-133">id</span><span class="sxs-lookup"><span data-stu-id="02078-133">id</span></span>|<span data-ttu-id="02078-134">String</span><span class="sxs-lookup"><span data-stu-id="02078-134">String</span></span>|<span data-ttu-id="02078-135">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="02078-135">Unique identifier for this entity</span></span>|



## <a name="response"></a><span data-ttu-id="02078-136">响应</span><span class="sxs-lookup"><span data-stu-id="02078-136">Response</span></span>
<span data-ttu-id="02078-137">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="02078-137">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="02078-138">示例</span><span class="sxs-lookup"><span data-stu-id="02078-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="02078-139">请求</span><span class="sxs-lookup"><span data-stu-id="02078-139">Request</span></span>
<span data-ttu-id="02078-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="02078-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.deviceManagementReports"
}
```

### <a name="response"></a><span data-ttu-id="02078-141">响应</span><span class="sxs-lookup"><span data-stu-id="02078-141">Response</span></span>
<span data-ttu-id="02078-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="02078-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "d6a697d3-97d3-d6a6-d397-a6d6d397a6d6"
}
```





