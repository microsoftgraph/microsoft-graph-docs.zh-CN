---
title: 更新 vulnerableManagedDevice
description: 更新 vulnerableManagedDevice 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5f054105fcbea0c4d6c9d5ae0411341702d46520
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51158743"
---
# <a name="update-vulnerablemanageddevice"></a><span data-ttu-id="f59fe-103">更新 vulnerableManagedDevice</span><span class="sxs-lookup"><span data-stu-id="f59fe-103">Update vulnerableManagedDevice</span></span>

<span data-ttu-id="f59fe-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f59fe-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f59fe-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f59fe-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f59fe-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f59fe-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f59fe-107">更新 [vulnerableManagedDevice 对象](../resources/intune-partnerintegration-vulnerablemanageddevice.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="f59fe-107">Update the properties of a [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f59fe-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f59fe-108">Prerequisites</span></span>
<span data-ttu-id="f59fe-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f59fe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f59fe-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f59fe-111">Permission type</span></span>|<span data-ttu-id="f59fe-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f59fe-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f59fe-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f59fe-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f59fe-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f59fe-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f59fe-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f59fe-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f59fe-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f59fe-116">Not supported.</span></span>|
|<span data-ttu-id="f59fe-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f59fe-117">Application</span></span>|<span data-ttu-id="f59fe-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f59fe-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f59fe-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f59fe-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH ** Entity URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

## <a name="request-headers"></a><span data-ttu-id="f59fe-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f59fe-120">Request headers</span></span>
|<span data-ttu-id="f59fe-121">标头</span><span class="sxs-lookup"><span data-stu-id="f59fe-121">Header</span></span>|<span data-ttu-id="f59fe-122">值</span><span class="sxs-lookup"><span data-stu-id="f59fe-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f59fe-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f59fe-123">Authorization</span></span>|<span data-ttu-id="f59fe-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f59fe-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f59fe-125">接受</span><span class="sxs-lookup"><span data-stu-id="f59fe-125">Accept</span></span>|<span data-ttu-id="f59fe-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f59fe-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f59fe-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f59fe-127">Request body</span></span>
<span data-ttu-id="f59fe-128">在请求正文中，提供 [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f59fe-128">In the request body, supply a JSON representation for the [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object.</span></span>

<span data-ttu-id="f59fe-129">下表显示创建 [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f59fe-129">The following table shows the properties that are required when you create the [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md).</span></span>

|<span data-ttu-id="f59fe-130">属性</span><span class="sxs-lookup"><span data-stu-id="f59fe-130">Property</span></span>|<span data-ttu-id="f59fe-131">类型</span><span class="sxs-lookup"><span data-stu-id="f59fe-131">Type</span></span>|<span data-ttu-id="f59fe-132">说明</span><span class="sxs-lookup"><span data-stu-id="f59fe-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f59fe-133">id</span><span class="sxs-lookup"><span data-stu-id="f59fe-133">id</span></span>|<span data-ttu-id="f59fe-134">String</span><span class="sxs-lookup"><span data-stu-id="f59fe-134">String</span></span>|<span data-ttu-id="f59fe-135">实体密钥和 AAD 设备 ID。</span><span class="sxs-lookup"><span data-stu-id="f59fe-135">The entity key, and AAD device ID.</span></span>|
|<span data-ttu-id="f59fe-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="f59fe-136">managedDeviceId</span></span>|<span data-ttu-id="f59fe-137">String</span><span class="sxs-lookup"><span data-stu-id="f59fe-137">String</span></span>|<span data-ttu-id="f59fe-138">Intune 托管设备 ID。</span><span class="sxs-lookup"><span data-stu-id="f59fe-138">The Intune managed device ID.</span></span>|
|<span data-ttu-id="f59fe-139">displayName</span><span class="sxs-lookup"><span data-stu-id="f59fe-139">displayName</span></span>|<span data-ttu-id="f59fe-140">String</span><span class="sxs-lookup"><span data-stu-id="f59fe-140">String</span></span>|<span data-ttu-id="f59fe-141">设备名称。</span><span class="sxs-lookup"><span data-stu-id="f59fe-141">The device name.</span></span>|
|<span data-ttu-id="f59fe-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="f59fe-142">lastSyncDateTime</span></span>|<span data-ttu-id="f59fe-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f59fe-143">DateTimeOffset</span></span>|<span data-ttu-id="f59fe-144">上次同步日期。</span><span class="sxs-lookup"><span data-stu-id="f59fe-144">The last sync date.</span></span>|



## <a name="response"></a><span data-ttu-id="f59fe-145">响应</span><span class="sxs-lookup"><span data-stu-id="f59fe-145">Response</span></span>
<span data-ttu-id="f59fe-146">如果成功，此方法在响应正文中返回 响应代码和更新 `200 OK` [的 vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f59fe-146">If successful, this method returns a `200 OK` response code and an updated [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f59fe-147">示例</span><span class="sxs-lookup"><span data-stu-id="f59fe-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="f59fe-148">请求</span><span class="sxs-lookup"><span data-stu-id="f59fe-148">Request</span></span>
<span data-ttu-id="f59fe-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f59fe-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta** Entity URI for microsoft.management.services.api.vulnerableManagedDevice not found
Content-type: application/json
Content-length: 214

{
  "@odata.type": "#microsoft.graph.vulnerableManagedDevice",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```

### <a name="response"></a><span data-ttu-id="f59fe-150">响应</span><span class="sxs-lookup"><span data-stu-id="f59fe-150">Response</span></span>
<span data-ttu-id="f59fe-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f59fe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 263

{
  "@odata.type": "#microsoft.graph.vulnerableManagedDevice",
  "id": "e59891d4-91d4-e598-d491-98e5d49198e5",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```




