---
title: 更新 windowsAutopilotSettings
description: 更新 windowsAutopilotSettings 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 29ec5af7b5b900bcd6ec8f976c665782d371c165
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43452280"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="3a08d-103">更新 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="3a08d-103">Update windowsAutopilotSettings</span></span>

<span data-ttu-id="3a08d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3a08d-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3a08d-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3a08d-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3a08d-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3a08d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3a08d-107">更新[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3a08d-107">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3a08d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3a08d-108">Prerequisites</span></span>
<span data-ttu-id="3a08d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3a08d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3a08d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3a08d-111">Permission type</span></span>|<span data-ttu-id="3a08d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3a08d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3a08d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3a08d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3a08d-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a08d-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3a08d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3a08d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3a08d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3a08d-116">Not supported.</span></span>|
|<span data-ttu-id="3a08d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3a08d-117">Application</span></span>|<span data-ttu-id="3a08d-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3a08d-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3a08d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3a08d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="3a08d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3a08d-120">Request headers</span></span>
|<span data-ttu-id="3a08d-121">标头</span><span class="sxs-lookup"><span data-stu-id="3a08d-121">Header</span></span>|<span data-ttu-id="3a08d-122">值</span><span class="sxs-lookup"><span data-stu-id="3a08d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3a08d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3a08d-123">Authorization</span></span>|<span data-ttu-id="3a08d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3a08d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3a08d-125">接受</span><span class="sxs-lookup"><span data-stu-id="3a08d-125">Accept</span></span>|<span data-ttu-id="3a08d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3a08d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3a08d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3a08d-127">Request body</span></span>
<span data-ttu-id="3a08d-128">在请求正文中，提供[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3a08d-128">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="3a08d-129">下表显示创建[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3a08d-129">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="3a08d-130">属性</span><span class="sxs-lookup"><span data-stu-id="3a08d-130">Property</span></span>|<span data-ttu-id="3a08d-131">类型</span><span class="sxs-lookup"><span data-stu-id="3a08d-131">Type</span></span>|<span data-ttu-id="3a08d-132">说明</span><span class="sxs-lookup"><span data-stu-id="3a08d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3a08d-133">id</span><span class="sxs-lookup"><span data-stu-id="3a08d-133">id</span></span>|<span data-ttu-id="3a08d-134">String</span><span class="sxs-lookup"><span data-stu-id="3a08d-134">String</span></span>|<span data-ttu-id="3a08d-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="3a08d-135">The GUID for the object</span></span>|
|<span data-ttu-id="3a08d-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="3a08d-136">lastSyncDateTime</span></span>|<span data-ttu-id="3a08d-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a08d-137">DateTimeOffset</span></span>|<span data-ttu-id="3a08d-138">包含 DDS 服务的上次数据同步日期时间。</span><span class="sxs-lookup"><span data-stu-id="3a08d-138">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="3a08d-139">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="3a08d-139">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="3a08d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3a08d-140">DateTimeOffset</span></span>|<span data-ttu-id="3a08d-141">包含 DDS 服务的上次数据同步日期时间。</span><span class="sxs-lookup"><span data-stu-id="3a08d-141">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="3a08d-142">syncStatus</span><span class="sxs-lookup"><span data-stu-id="3a08d-142">syncStatus</span></span>|[<span data-ttu-id="3a08d-143">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="3a08d-143">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="3a08d-144">指示与设备数据同步（DDS）服务同步的状态。</span><span class="sxs-lookup"><span data-stu-id="3a08d-144">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="3a08d-145">可取值为：`unknown`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="3a08d-145">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="3a08d-146">响应</span><span class="sxs-lookup"><span data-stu-id="3a08d-146">Response</span></span>
<span data-ttu-id="3a08d-147">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3a08d-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3a08d-148">示例</span><span class="sxs-lookup"><span data-stu-id="3a08d-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="3a08d-149">请求</span><span class="sxs-lookup"><span data-stu-id="3a08d-149">Request</span></span>
<span data-ttu-id="3a08d-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3a08d-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings
Content-type: application/json
Content-length: 230

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```

### <a name="response"></a><span data-ttu-id="3a08d-151">响应</span><span class="sxs-lookup"><span data-stu-id="3a08d-151">Response</span></span>
<span data-ttu-id="3a08d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3a08d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 279

{
  "@odata.type": "#microsoft.graph.windowsAutopilotSettings",
  "id": "08c16770-6770-08c1-7067-c1087067c108",
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```



