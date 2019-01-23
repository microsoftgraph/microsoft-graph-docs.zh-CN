---
title: 创建 deviceComplianceActionItem
description: 创建新的 deviceComplianceActionItem 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 5e538bd064c2d590eeb743e2c2dea05abc869900
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421576"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="e9bc6-103">创建 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="e9bc6-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="e9bc6-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e9bc6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e9bc6-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e9bc6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e9bc6-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e9bc6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e9bc6-107">创建新的 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e9bc6-107">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e9bc6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e9bc6-108">Prerequisites</span></span>
<span data-ttu-id="e9bc6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e9bc6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e9bc6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e9bc6-111">Permission type</span></span>|<span data-ttu-id="e9bc6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e9bc6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e9bc6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e9bc6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e9bc6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e9bc6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e9bc6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e9bc6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e9bc6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9bc6-116">Not supported.</span></span>|
|<span data-ttu-id="e9bc6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e9bc6-117">Application</span></span>|<span data-ttu-id="e9bc6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e9bc6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e9bc6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e9bc6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="e9bc6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e9bc6-120">Request headers</span></span>
|<span data-ttu-id="e9bc6-121">标头</span><span class="sxs-lookup"><span data-stu-id="e9bc6-121">Header</span></span>|<span data-ttu-id="e9bc6-122">值</span><span class="sxs-lookup"><span data-stu-id="e9bc6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e9bc6-123">授权</span><span class="sxs-lookup"><span data-stu-id="e9bc6-123">Authorization</span></span>|<span data-ttu-id="e9bc6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e9bc6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e9bc6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e9bc6-125">Accept</span></span>|<span data-ttu-id="e9bc6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e9bc6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e9bc6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e9bc6-127">Request body</span></span>
<span data-ttu-id="e9bc6-128">在请求正文中，提供 deviceComplianceActionItem 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e9bc6-128">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="e9bc6-129">下表显示了创建 deviceComplianceActionItem 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e9bc6-129">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="e9bc6-130">属性</span><span class="sxs-lookup"><span data-stu-id="e9bc6-130">Property</span></span>|<span data-ttu-id="e9bc6-131">类型</span><span class="sxs-lookup"><span data-stu-id="e9bc6-131">Type</span></span>|<span data-ttu-id="e9bc6-132">说明</span><span class="sxs-lookup"><span data-stu-id="e9bc6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e9bc6-133">id</span><span class="sxs-lookup"><span data-stu-id="e9bc6-133">id</span></span>|<span data-ttu-id="e9bc6-134">String</span><span class="sxs-lookup"><span data-stu-id="e9bc6-134">String</span></span>|<span data-ttu-id="e9bc6-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e9bc6-135">Key of the entity.</span></span>|
|<span data-ttu-id="e9bc6-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="e9bc6-136">gracePeriodHours</span></span>|<span data-ttu-id="e9bc6-137">Int32</span><span class="sxs-lookup"><span data-stu-id="e9bc6-137">Int32</span></span>|<span data-ttu-id="e9bc6-138">强制执行操作前要等待的小时数。</span><span class="sxs-lookup"><span data-stu-id="e9bc6-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="e9bc6-139">有效值为 0 至 8760</span><span class="sxs-lookup"><span data-stu-id="e9bc6-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="e9bc6-140">actionType</span><span class="sxs-lookup"><span data-stu-id="e9bc6-140">actionType</span></span>|[<span data-ttu-id="e9bc6-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="e9bc6-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="e9bc6-142">要采取什么操作。</span><span class="sxs-lookup"><span data-stu-id="e9bc6-142">What action to take.</span></span> <span data-ttu-id="e9bc6-143">可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock`。</span><span class="sxs-lookup"><span data-stu-id="e9bc6-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="e9bc6-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="e9bc6-144">notificationTemplateId</span></span>|<span data-ttu-id="e9bc6-145">String</span><span class="sxs-lookup"><span data-stu-id="e9bc6-145">String</span></span>|<span data-ttu-id="e9bc6-146">要使用的通知消息模板</span><span class="sxs-lookup"><span data-stu-id="e9bc6-146">What notification Message template to use</span></span>|
|<span data-ttu-id="e9bc6-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="e9bc6-147">notificationMessageCCList</span></span>|<span data-ttu-id="e9bc6-148">String 集合</span><span class="sxs-lookup"><span data-stu-id="e9bc6-148">String collection</span></span>|<span data-ttu-id="e9bc6-149">指定此通知邮件抄送对象的组 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="e9bc6-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="e9bc6-150">响应</span><span class="sxs-lookup"><span data-stu-id="e9bc6-150">Response</span></span>
<span data-ttu-id="e9bc6-151">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e9bc6-151">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e9bc6-152">示例</span><span class="sxs-lookup"><span data-stu-id="e9bc6-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="e9bc6-153">请求</span><span class="sxs-lookup"><span data-stu-id="e9bc6-153">Request</span></span>
<span data-ttu-id="e9bc6-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e9bc6-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e9bc6-155">响应</span><span class="sxs-lookup"><span data-stu-id="e9bc6-155">Response</span></span>
<span data-ttu-id="e9bc6-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e9bc6-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




