---
title: 创建 vulnerableManagedDevice
description: 创建新的 vulnerableManagedDevice 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5d9bab17be811156f9aa0efcae52f024388f260d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49270412"
---
# <a name="create-vulnerablemanageddevice"></a><span data-ttu-id="afb79-103">创建 vulnerableManagedDevice</span><span class="sxs-lookup"><span data-stu-id="afb79-103">Create vulnerableManagedDevice</span></span>

<span data-ttu-id="afb79-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="afb79-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="afb79-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="afb79-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="afb79-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="afb79-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="afb79-107">创建新的 [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="afb79-107">Create a new [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="afb79-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="afb79-108">Prerequisites</span></span>
<span data-ttu-id="afb79-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="afb79-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="afb79-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="afb79-111">Permission type</span></span>|<span data-ttu-id="afb79-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="afb79-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="afb79-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="afb79-113">Delegated (work or school account)</span></span>|<span data-ttu-id="afb79-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afb79-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="afb79-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="afb79-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="afb79-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="afb79-116">Not supported.</span></span>|
|<span data-ttu-id="afb79-117">Application</span><span class="sxs-lookup"><span data-stu-id="afb79-117">Application</span></span>|<span data-ttu-id="afb79-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="afb79-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="afb79-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="afb79-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST ** Collection URI for microsoft.management.services.api.vulnerableManagedDevice not found
```

## <a name="request-headers"></a><span data-ttu-id="afb79-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="afb79-120">Request headers</span></span>
|<span data-ttu-id="afb79-121">标头</span><span class="sxs-lookup"><span data-stu-id="afb79-121">Header</span></span>|<span data-ttu-id="afb79-122">值</span><span class="sxs-lookup"><span data-stu-id="afb79-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="afb79-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="afb79-123">Authorization</span></span>|<span data-ttu-id="afb79-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="afb79-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="afb79-125">接受</span><span class="sxs-lookup"><span data-stu-id="afb79-125">Accept</span></span>|<span data-ttu-id="afb79-126">application/json</span><span class="sxs-lookup"><span data-stu-id="afb79-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="afb79-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="afb79-127">Request body</span></span>
<span data-ttu-id="afb79-128">在请求正文中，提供 vulnerableManagedDevice 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="afb79-128">In the request body, supply a JSON representation for the vulnerableManagedDevice object.</span></span>

<span data-ttu-id="afb79-129">下表显示创建 vulnerableManagedDevice 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="afb79-129">The following table shows the properties that are required when you create the vulnerableManagedDevice.</span></span>

|<span data-ttu-id="afb79-130">属性</span><span class="sxs-lookup"><span data-stu-id="afb79-130">Property</span></span>|<span data-ttu-id="afb79-131">类型</span><span class="sxs-lookup"><span data-stu-id="afb79-131">Type</span></span>|<span data-ttu-id="afb79-132">说明</span><span class="sxs-lookup"><span data-stu-id="afb79-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="afb79-133">id</span><span class="sxs-lookup"><span data-stu-id="afb79-133">id</span></span>|<span data-ttu-id="afb79-134">字符串</span><span class="sxs-lookup"><span data-stu-id="afb79-134">String</span></span>|<span data-ttu-id="afb79-135">实体密钥和 AAD 设备 ID。</span><span class="sxs-lookup"><span data-stu-id="afb79-135">The entity key, and AAD device ID.</span></span>|
|<span data-ttu-id="afb79-136">managedDeviceId</span><span class="sxs-lookup"><span data-stu-id="afb79-136">managedDeviceId</span></span>|<span data-ttu-id="afb79-137">字符串</span><span class="sxs-lookup"><span data-stu-id="afb79-137">String</span></span>|<span data-ttu-id="afb79-138">Intune 托管设备 ID。</span><span class="sxs-lookup"><span data-stu-id="afb79-138">The Intune managed device ID.</span></span>|
|<span data-ttu-id="afb79-139">displayName</span><span class="sxs-lookup"><span data-stu-id="afb79-139">displayName</span></span>|<span data-ttu-id="afb79-140">字符串</span><span class="sxs-lookup"><span data-stu-id="afb79-140">String</span></span>|<span data-ttu-id="afb79-141">设备名称。</span><span class="sxs-lookup"><span data-stu-id="afb79-141">The device name.</span></span>|
|<span data-ttu-id="afb79-142">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="afb79-142">lastSyncDateTime</span></span>|<span data-ttu-id="afb79-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="afb79-143">DateTimeOffset</span></span>|<span data-ttu-id="afb79-144">上次同步日期。</span><span class="sxs-lookup"><span data-stu-id="afb79-144">The last sync date.</span></span>|



## <a name="response"></a><span data-ttu-id="afb79-145">响应</span><span class="sxs-lookup"><span data-stu-id="afb79-145">Response</span></span>
<span data-ttu-id="afb79-146">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="afb79-146">If successful, this method returns a `201 Created` response code and a [vulnerableManagedDevice](../resources/intune-partnerintegration-vulnerablemanageddevice.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="afb79-147">示例</span><span class="sxs-lookup"><span data-stu-id="afb79-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="afb79-148">请求</span><span class="sxs-lookup"><span data-stu-id="afb79-148">Request</span></span>
<span data-ttu-id="afb79-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="afb79-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta** Collection URI for microsoft.management.services.api.vulnerableManagedDevice not found
Content-type: application/json
Content-length: 214

{
  "@odata.type": "#microsoft.graph.vulnerableManagedDevice",
  "managedDeviceId": "Managed Device Id value",
  "displayName": "Display Name value",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00"
}
```

### <a name="response"></a><span data-ttu-id="afb79-150">响应</span><span class="sxs-lookup"><span data-stu-id="afb79-150">Response</span></span>
<span data-ttu-id="afb79-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="afb79-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




