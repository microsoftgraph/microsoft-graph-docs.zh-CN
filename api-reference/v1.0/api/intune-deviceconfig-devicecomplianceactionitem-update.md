---
title: 更新 deviceComplianceActionItem
description: 更新 deviceComplianceActionItem 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5da502820ccf13b0494a6914811db698ff8abc65
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30254021"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="5b8aa-103">更新 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="5b8aa-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="5b8aa-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5b8aa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5b8aa-105">更新 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5b8aa-105">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5b8aa-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="5b8aa-106">Prerequisites</span></span>
<span data-ttu-id="5b8aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="5b8aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="5b8aa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5b8aa-109">Permission type</span></span>|<span data-ttu-id="5b8aa-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5b8aa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5b8aa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5b8aa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5b8aa-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5b8aa-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5b8aa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5b8aa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5b8aa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b8aa-114">Not supported.</span></span>|
|<span data-ttu-id="5b8aa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5b8aa-115">Application</span></span>|<span data-ttu-id="5b8aa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5b8aa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5b8aa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5b8aa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="5b8aa-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5b8aa-118">Request headers</span></span>
|<span data-ttu-id="5b8aa-119">标头</span><span class="sxs-lookup"><span data-stu-id="5b8aa-119">Header</span></span>|<span data-ttu-id="5b8aa-120">值</span><span class="sxs-lookup"><span data-stu-id="5b8aa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5b8aa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5b8aa-121">Authorization</span></span>|<span data-ttu-id="5b8aa-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5b8aa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5b8aa-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5b8aa-123">Accept</span></span>|<span data-ttu-id="5b8aa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5b8aa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5b8aa-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5b8aa-125">Request body</span></span>
<span data-ttu-id="5b8aa-126">在请求正文中，提供 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5b8aa-126">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="5b8aa-127">下表显示了创建 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5b8aa-127">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="5b8aa-128">属性</span><span class="sxs-lookup"><span data-stu-id="5b8aa-128">Property</span></span>|<span data-ttu-id="5b8aa-129">类型</span><span class="sxs-lookup"><span data-stu-id="5b8aa-129">Type</span></span>|<span data-ttu-id="5b8aa-130">说明</span><span class="sxs-lookup"><span data-stu-id="5b8aa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5b8aa-131">id</span><span class="sxs-lookup"><span data-stu-id="5b8aa-131">id</span></span>|<span data-ttu-id="5b8aa-132">字符串</span><span class="sxs-lookup"><span data-stu-id="5b8aa-132">String</span></span>|<span data-ttu-id="5b8aa-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5b8aa-133">Key of the entity.</span></span>|
|<span data-ttu-id="5b8aa-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="5b8aa-134">gracePeriodHours</span></span>|<span data-ttu-id="5b8aa-135">Int32</span><span class="sxs-lookup"><span data-stu-id="5b8aa-135">Int32</span></span>|<span data-ttu-id="5b8aa-136">强制执行操作前要等待的小时数。</span><span class="sxs-lookup"><span data-stu-id="5b8aa-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="5b8aa-137">有效值为 0 至 8760</span><span class="sxs-lookup"><span data-stu-id="5b8aa-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="5b8aa-138">actionType</span><span class="sxs-lookup"><span data-stu-id="5b8aa-138">actionType</span></span>|[<span data-ttu-id="5b8aa-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="5b8aa-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="5b8aa-140">要执行的操作。</span><span class="sxs-lookup"><span data-stu-id="5b8aa-140">What action to take.</span></span> <span data-ttu-id="5b8aa-141">可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`。</span><span class="sxs-lookup"><span data-stu-id="5b8aa-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="5b8aa-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="5b8aa-142">notificationTemplateId</span></span>|<span data-ttu-id="5b8aa-143">String</span><span class="sxs-lookup"><span data-stu-id="5b8aa-143">String</span></span>|<span data-ttu-id="5b8aa-144">要使用的通知消息模板</span><span class="sxs-lookup"><span data-stu-id="5b8aa-144">What notification Message template to use</span></span>|
|<span data-ttu-id="5b8aa-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="5b8aa-145">notificationMessageCCList</span></span>|<span data-ttu-id="5b8aa-146">String collection</span><span class="sxs-lookup"><span data-stu-id="5b8aa-146">String collection</span></span>|<span data-ttu-id="5b8aa-147">指定此通知邮件抄送对象的组 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="5b8aa-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="5b8aa-148">响应</span><span class="sxs-lookup"><span data-stu-id="5b8aa-148">Response</span></span>
<span data-ttu-id="5b8aa-149">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5b8aa-149">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5b8aa-150">示例</span><span class="sxs-lookup"><span data-stu-id="5b8aa-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="5b8aa-151">请求</span><span class="sxs-lookup"><span data-stu-id="5b8aa-151">Request</span></span>
<span data-ttu-id="5b8aa-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5b8aa-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
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

### <a name="response"></a><span data-ttu-id="5b8aa-153">响应</span><span class="sxs-lookup"><span data-stu-id="5b8aa-153">Response</span></span>
<span data-ttu-id="5b8aa-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5b8aa-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



