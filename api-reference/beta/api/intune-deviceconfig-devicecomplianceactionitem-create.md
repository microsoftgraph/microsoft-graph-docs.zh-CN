---
title: 创建 deviceComplianceActionItem
description: 创建新的 deviceComplianceActionItem 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02ace77a993d8f9e36331981a38093990343fafa
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48695773"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="08d5e-103">创建 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="08d5e-103">Create deviceComplianceActionItem</span></span>

<span data-ttu-id="08d5e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08d5e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08d5e-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="08d5e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08d5e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08d5e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08d5e-107">创建新的 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08d5e-107">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08d5e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="08d5e-108">Prerequisites</span></span>
<span data-ttu-id="08d5e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08d5e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08d5e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="08d5e-111">Permission type</span></span>|<span data-ttu-id="08d5e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="08d5e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08d5e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08d5e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08d5e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08d5e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08d5e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08d5e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08d5e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="08d5e-116">Not supported.</span></span>|
|<span data-ttu-id="08d5e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="08d5e-117">Application</span></span>|<span data-ttu-id="08d5e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08d5e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08d5e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08d5e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="08d5e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="08d5e-120">Request headers</span></span>
|<span data-ttu-id="08d5e-121">标头</span><span class="sxs-lookup"><span data-stu-id="08d5e-121">Header</span></span>|<span data-ttu-id="08d5e-122">值</span><span class="sxs-lookup"><span data-stu-id="08d5e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08d5e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08d5e-123">Authorization</span></span>|<span data-ttu-id="08d5e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="08d5e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08d5e-125">接受</span><span class="sxs-lookup"><span data-stu-id="08d5e-125">Accept</span></span>|<span data-ttu-id="08d5e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08d5e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08d5e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="08d5e-127">Request body</span></span>
<span data-ttu-id="08d5e-128">在请求正文中，提供 deviceComplianceActionItem 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08d5e-128">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="08d5e-129">下表显示了创建 deviceComplianceActionItem 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="08d5e-129">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="08d5e-130">属性</span><span class="sxs-lookup"><span data-stu-id="08d5e-130">Property</span></span>|<span data-ttu-id="08d5e-131">类型</span><span class="sxs-lookup"><span data-stu-id="08d5e-131">Type</span></span>|<span data-ttu-id="08d5e-132">说明</span><span class="sxs-lookup"><span data-stu-id="08d5e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08d5e-133">id</span><span class="sxs-lookup"><span data-stu-id="08d5e-133">id</span></span>|<span data-ttu-id="08d5e-134">String</span><span class="sxs-lookup"><span data-stu-id="08d5e-134">String</span></span>|<span data-ttu-id="08d5e-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="08d5e-135">Key of the entity.</span></span>|
|<span data-ttu-id="08d5e-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="08d5e-136">gracePeriodHours</span></span>|<span data-ttu-id="08d5e-137">Int32</span><span class="sxs-lookup"><span data-stu-id="08d5e-137">Int32</span></span>|<span data-ttu-id="08d5e-138">强制执行操作前要等待的小时数。</span><span class="sxs-lookup"><span data-stu-id="08d5e-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="08d5e-139">有效值为 0 至 8760</span><span class="sxs-lookup"><span data-stu-id="08d5e-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="08d5e-140">actionType</span><span class="sxs-lookup"><span data-stu-id="08d5e-140">actionType</span></span>|[<span data-ttu-id="08d5e-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="08d5e-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="08d5e-142">要执行的操作。</span><span class="sxs-lookup"><span data-stu-id="08d5e-142">What action to take.</span></span> <span data-ttu-id="08d5e-143">可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock`。</span><span class="sxs-lookup"><span data-stu-id="08d5e-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="08d5e-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="08d5e-144">notificationTemplateId</span></span>|<span data-ttu-id="08d5e-145">String</span><span class="sxs-lookup"><span data-stu-id="08d5e-145">String</span></span>|<span data-ttu-id="08d5e-146">要使用的通知消息模板</span><span class="sxs-lookup"><span data-stu-id="08d5e-146">What notification Message template to use</span></span>|
|<span data-ttu-id="08d5e-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="08d5e-147">notificationMessageCCList</span></span>|<span data-ttu-id="08d5e-148">String collection</span><span class="sxs-lookup"><span data-stu-id="08d5e-148">String collection</span></span>|<span data-ttu-id="08d5e-149">指定此通知邮件抄送对象的组 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="08d5e-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="08d5e-150">响应</span><span class="sxs-lookup"><span data-stu-id="08d5e-150">Response</span></span>
<span data-ttu-id="08d5e-151">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08d5e-151">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08d5e-152">示例</span><span class="sxs-lookup"><span data-stu-id="08d5e-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="08d5e-153">请求</span><span class="sxs-lookup"><span data-stu-id="08d5e-153">Request</span></span>
<span data-ttu-id="08d5e-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="08d5e-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="08d5e-155">响应</span><span class="sxs-lookup"><span data-stu-id="08d5e-155">Response</span></span>
<span data-ttu-id="08d5e-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="08d5e-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 320

{
  "@odata.type": "#microsoft.graph.deviceComplianceActionItem",
  "id": "e01a1893-1893-e01a-9318-1ae093181ae0",
  "gracePeriodHours": 0,
  "actionType": "notification",
  "notificationTemplateId": "Notification Template Id value",
  "notificationMessageCCList": [
    "Notification Message CCList value"
  ]
}
```





