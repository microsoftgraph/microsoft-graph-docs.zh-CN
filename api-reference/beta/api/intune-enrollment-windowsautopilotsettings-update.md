---
title: 更新 windowsAutopilotSettings
description: 更新 windowsAutopilotSettings 对象的属性。
author: tfitzmac
ms.openlocfilehash: 281a0ff6412151e284c566444886092e2566b491
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316084"
---
# <a name="update-windowsautopilotsettings"></a><span data-ttu-id="971b1-103">更新 windowsAutopilotSettings</span><span class="sxs-lookup"><span data-stu-id="971b1-103">Update windowsAutopilotSettings</span></span>

> <span data-ttu-id="971b1-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="971b1-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="971b1-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="971b1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="971b1-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="971b1-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="971b1-107">更新[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="971b1-107">Update the properties of a [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="971b1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="971b1-108">Prerequisites</span></span>
<span data-ttu-id="971b1-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="971b1-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="971b1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="971b1-111">Permission type</span></span>|<span data-ttu-id="971b1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="971b1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="971b1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="971b1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="971b1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="971b1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="971b1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="971b1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="971b1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="971b1-116">Not supported.</span></span>|
|<span data-ttu-id="971b1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="971b1-117">Application</span></span>|<span data-ttu-id="971b1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="971b1-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="971b1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="971b1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsAutopilotSettings
```

## <a name="request-headers"></a><span data-ttu-id="971b1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="971b1-120">Request headers</span></span>
|<span data-ttu-id="971b1-121">标头</span><span class="sxs-lookup"><span data-stu-id="971b1-121">Header</span></span>|<span data-ttu-id="971b1-122">值</span><span class="sxs-lookup"><span data-stu-id="971b1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="971b1-123">授权</span><span class="sxs-lookup"><span data-stu-id="971b1-123">Authorization</span></span>|<span data-ttu-id="971b1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="971b1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="971b1-125">Accept</span><span class="sxs-lookup"><span data-stu-id="971b1-125">Accept</span></span>|<span data-ttu-id="971b1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="971b1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="971b1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="971b1-127">Request body</span></span>
<span data-ttu-id="971b1-128">在请求正文中，提供[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="971b1-128">In the request body, supply a JSON representation for the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object.</span></span>

<span data-ttu-id="971b1-129">下表显示时创建[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="971b1-129">The following table shows the properties that are required when you create the [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md).</span></span>

|<span data-ttu-id="971b1-130">属性</span><span class="sxs-lookup"><span data-stu-id="971b1-130">Property</span></span>|<span data-ttu-id="971b1-131">类型</span><span class="sxs-lookup"><span data-stu-id="971b1-131">Type</span></span>|<span data-ttu-id="971b1-132">说明</span><span class="sxs-lookup"><span data-stu-id="971b1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="971b1-133">id</span><span class="sxs-lookup"><span data-stu-id="971b1-133">id</span></span>|<span data-ttu-id="971b1-134">字符串</span><span class="sxs-lookup"><span data-stu-id="971b1-134">String</span></span>|<span data-ttu-id="971b1-135">对象的 GUID</span><span class="sxs-lookup"><span data-stu-id="971b1-135">The GUID for the object</span></span>|
|<span data-ttu-id="971b1-136">lastSyncDateTime</span><span class="sxs-lookup"><span data-stu-id="971b1-136">lastSyncDateTime</span></span>|<span data-ttu-id="971b1-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="971b1-137">DateTimeOffset</span></span>|<span data-ttu-id="971b1-138">最后一个数据同步与 DD 服务的日期时间。</span><span class="sxs-lookup"><span data-stu-id="971b1-138">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="971b1-139">lastManualSyncTriggerDateTime</span><span class="sxs-lookup"><span data-stu-id="971b1-139">lastManualSyncTriggerDateTime</span></span>|<span data-ttu-id="971b1-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="971b1-140">DateTimeOffset</span></span>|<span data-ttu-id="971b1-141">最后一个数据同步与 DD 服务的日期时间。</span><span class="sxs-lookup"><span data-stu-id="971b1-141">Last data sync date time with DDS service.</span></span>|
|<span data-ttu-id="971b1-142">syncStatus</span><span class="sxs-lookup"><span data-stu-id="971b1-142">syncStatus</span></span>|[<span data-ttu-id="971b1-143">windowsAutopilotSyncStatus</span><span class="sxs-lookup"><span data-stu-id="971b1-143">windowsAutopilotSyncStatus</span></span>](../resources/intune-enrollment-windowsautopilotsyncstatus.md)|<span data-ttu-id="971b1-144">指示与设备数据同步 (DD) 服务的同步状态。</span><span class="sxs-lookup"><span data-stu-id="971b1-144">Indicates the status of sync with Device data sync (DDS) service.</span></span> <span data-ttu-id="971b1-145">可取值为：`unknown`、`inProgress`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="971b1-145">Possible values are: `unknown`, `inProgress`, `completed`, `failed`.</span></span>|



## <a name="response"></a><span data-ttu-id="971b1-146">响应</span><span class="sxs-lookup"><span data-stu-id="971b1-146">Response</span></span>
<span data-ttu-id="971b1-147">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="971b1-147">If successful, this method returns a `200 OK` response code and an updated [windowsAutopilotSettings](../resources/intune-enrollment-windowsautopilotsettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="971b1-148">示例</span><span class="sxs-lookup"><span data-stu-id="971b1-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="971b1-149">请求</span><span class="sxs-lookup"><span data-stu-id="971b1-149">Request</span></span>
<span data-ttu-id="971b1-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="971b1-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsAutopilotSettings
Content-type: application/json
Content-length: 167

{
  "lastSyncDateTime": "2017-01-01T00:02:49.3205976-08:00",
  "lastManualSyncTriggerDateTime": "2016-12-31T23:57:54.7364636-08:00",
  "syncStatus": "inProgress"
}
```

### <a name="response"></a><span data-ttu-id="971b1-151">响应</span><span class="sxs-lookup"><span data-stu-id="971b1-151">Response</span></span>
<span data-ttu-id="971b1-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="971b1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





