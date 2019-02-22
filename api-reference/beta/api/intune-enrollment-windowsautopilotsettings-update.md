---
title: 更新 windowsAutopilotSettings
description: 更新 windowsAutopilotSettings 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: da2b5e622d9f5d8657e78162bff40d5843482081
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30144119"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="93505-103">更新 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="93505-103">Update windowsAutopilotSettings</span></span>

> <span data-ttu-id="93505-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="93505-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="93505-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="93505-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="93505-106">更新[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="93505-106">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="93505-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="93505-107">Prerequisites</span></span>
<span data-ttu-id="93505-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="93505-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="93505-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="93505-110">Permission type</span></span>|<span data-ttu-id="93505-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="93505-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="93505-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="93505-112">Delegated (work or school account)</span></span>|<span data-ttu-id="93505-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="93505-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="93505-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="93505-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="93505-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="93505-115">Not supported.</span></span>|
|<span data-ttu-id="93505-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="93505-116">Application</span></span>|<span data-ttu-id="93505-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="93505-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="93505-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="93505-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="93505-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="93505-119">Request headers</span></span>
|<span data-ttu-id="93505-120">标头</span><span class="sxs-lookup"><span data-stu-id="93505-120">Header</span></span>|<span data-ttu-id="93505-121">值</span><span class="sxs-lookup"><span data-stu-id="93505-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="93505-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="93505-122">Authorization</span></span>|<span data-ttu-id="93505-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="93505-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="93505-124">Accept</span><span class="sxs-lookup"><span data-stu-id="93505-124">Accept</span></span>|<span data-ttu-id="93505-125">application/json</span><span class="sxs-lookup"><span data-stu-id="93505-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="93505-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="93505-126">Request body</span></span>
<span data-ttu-id="93505-127">在请求正文中, 提供[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="93505-127">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="93505-128">下表显示创建[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="93505-128">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="93505-129">属性</span><span class="sxs-lookup"><span data-stu-id="93505-129">Property</span></span>|<span data-ttu-id="93505-130">类型</span><span class="sxs-lookup"><span data-stu-id="93505-130">Type</span></span>|<span data-ttu-id="93505-131">说明</span><span class="sxs-lookup"><span data-stu-id="93505-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="93505-132">id</span><span class="sxs-lookup"><span data-stu-id="93505-132">id</span></span>|<span data-ttu-id="93505-133">字符串</span><span class="sxs-lookup"><span data-stu-id="93505-133">String</span></span>|<span data-ttu-id="93505-134">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="93505-134">The GUID for the object</span></span>|
|<span data-ttu-id="93505-135">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="93505-135">lastSyncDateTime</span></span>|<span data-ttu-id="93505-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93505-136">DateTimeOffset</span></span>|<span data-ttu-id="93505-137">包含 DDS 服务的上次数据同步日期时间。</span><span class="sxs-lookup"><span data-stu-id="93505-137">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="93505-138">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="93505-138">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="93505-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="93505-139">DateTimeOffset</span></span>|<span data-ttu-id="93505-140">包含 DDS 服务的上次数据同步日期时间。</span><span class="sxs-lookup"><span data-stu-id="93505-140">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="93505-141">syncStatus</span><span class="sxs-lookup"><span data-stu-id="93505-141">syncStatus</span></span>|[<span data-ttu-id="93505-142">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="93505-142">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="93505-143">指示与设备数据同步 (DDS) 服务同步的状态。</span><span class="sxs-lookup"><span data-stu-id="93505-143">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="93505-144">可取值为：`unknown`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="93505-144">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="93505-145">响应</span><span class="sxs-lookup"><span data-stu-id="93505-145">Response</span></span>
<span data-ttu-id="93505-146">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="93505-146">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="93505-147">示例</span><span class="sxs-lookup"><span data-stu-id="93505-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="93505-148">请求</span><span class="sxs-lookup"><span data-stu-id="93505-148">Request</span></span>
<span data-ttu-id="93505-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="93505-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="93505-150">响应</span><span class="sxs-lookup"><span data-stu-id="93505-150">Response</span></span>
<span data-ttu-id="93505-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="93505-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




