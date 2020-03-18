---
title: 更新 deviceManagementReports
description: 更新 deviceManagementReports 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7e00e9a9f6e9e3ff2e0586f576a118608388cf27
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42801353"
---
# <a name="update-devicemanagementreports"></a><span data-ttu-id="9ef2b-103">更新 deviceManagementReports</span><span class="sxs-lookup"><span data-stu-id="9ef2b-103">Update deviceManagementReports</span></span>

> <span data-ttu-id="9ef2b-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9ef2b-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ef2b-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ef2b-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ef2b-106">更新[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="9ef2b-106">Update the properties of a [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ef2b-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="9ef2b-107">Prerequisites</span></span>
<span data-ttu-id="9ef2b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ef2b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ef2b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ef2b-110">Permission type</span></span>|<span data-ttu-id="9ef2b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9ef2b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ef2b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ef2b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="9ef2b-113">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="9ef2b-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="9ef2b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ef2b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ef2b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ef2b-115">Not supported.</span></span>|
|<span data-ttu-id="9ef2b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ef2b-116">Application</span></span>|<span data-ttu-id="9ef2b-117">Devicemanagementconfiguration.readwrite.all，Devicemanagementapps.readwrite.all，all，Devicemanagementmanageddevices.readwrite.all，All</span><span class="sxs-lookup"><span data-stu-id="9ef2b-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementApps.ReadWrite.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ef2b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ef2b-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/reports
```

## <a name="request-headers"></a><span data-ttu-id="9ef2b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ef2b-119">Request headers</span></span>
|<span data-ttu-id="9ef2b-120">标头</span><span class="sxs-lookup"><span data-stu-id="9ef2b-120">Header</span></span>|<span data-ttu-id="9ef2b-121">值</span><span class="sxs-lookup"><span data-stu-id="9ef2b-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ef2b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ef2b-122">Authorization</span></span>|<span data-ttu-id="9ef2b-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9ef2b-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ef2b-124">接受</span><span class="sxs-lookup"><span data-stu-id="9ef2b-124">Accept</span></span>|<span data-ttu-id="9ef2b-125">application/json</span><span class="sxs-lookup"><span data-stu-id="9ef2b-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ef2b-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ef2b-126">Request body</span></span>
<span data-ttu-id="9ef2b-127">在请求正文中，提供[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ef2b-127">In the request body, supply a JSON representation for the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object.</span></span>

<span data-ttu-id="9ef2b-128">下表显示创建[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9ef2b-128">The following table shows the properties that are required when you create the [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md).</span></span>

|<span data-ttu-id="9ef2b-129">属性</span><span class="sxs-lookup"><span data-stu-id="9ef2b-129">Property</span></span>|<span data-ttu-id="9ef2b-130">类型</span><span class="sxs-lookup"><span data-stu-id="9ef2b-130">Type</span></span>|<span data-ttu-id="9ef2b-131">说明</span><span class="sxs-lookup"><span data-stu-id="9ef2b-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ef2b-132">id</span><span class="sxs-lookup"><span data-stu-id="9ef2b-132">id</span></span>|<span data-ttu-id="9ef2b-133">String</span><span class="sxs-lookup"><span data-stu-id="9ef2b-133">String</span></span>|<span data-ttu-id="9ef2b-134">此实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="9ef2b-134">Unique identifier for this entity</span></span>|



## <a name="response"></a><span data-ttu-id="9ef2b-135">响应</span><span class="sxs-lookup"><span data-stu-id="9ef2b-135">Response</span></span>
<span data-ttu-id="9ef2b-136">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md)对象。</span><span class="sxs-lookup"><span data-stu-id="9ef2b-136">If successful, this method returns a `200 OK` response code and an updated [deviceManagementReports](../resources/intune-reporting-devicemanagementreports.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ef2b-137">示例</span><span class="sxs-lookup"><span data-stu-id="9ef2b-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ef2b-138">请求</span><span class="sxs-lookup"><span data-stu-id="9ef2b-138">Request</span></span>
<span data-ttu-id="9ef2b-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9ef2b-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/reports
Content-type: application/json
Content-length: 65

{
  "@odata.type": "#microsoft.graph.deviceManagementReports"
}
```

### <a name="response"></a><span data-ttu-id="9ef2b-140">响应</span><span class="sxs-lookup"><span data-stu-id="9ef2b-140">Response</span></span>
<span data-ttu-id="9ef2b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9ef2b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 114

{
  "@odata.type": "#microsoft.graph.deviceManagementReports",
  "id": "d6a697d3-97d3-d6a6-d397-a6d6d397a6d6"
}
```




