---
title: 更新 deviceComplianceActionItem
description: 更新 deviceComplianceActionItem 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 497a5e8b653d7873a45a242d0594d025f5e8a680
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32471810"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="0c236-103">更新 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="0c236-103">Update deviceComplianceActionItem</span></span>

> <span data-ttu-id="0c236-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0c236-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0c236-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0c236-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0c236-106">更新 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0c236-106">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0c236-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0c236-107">Prerequisites</span></span>
<span data-ttu-id="0c236-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0c236-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0c236-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0c236-110">Permission type</span></span>|<span data-ttu-id="0c236-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0c236-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0c236-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0c236-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0c236-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0c236-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0c236-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0c236-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0c236-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c236-115">Not supported.</span></span>|
|<span data-ttu-id="0c236-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0c236-116">Application</span></span>|<span data-ttu-id="0c236-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0c236-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0c236-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0c236-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="0c236-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0c236-119">Request headers</span></span>
|<span data-ttu-id="0c236-120">标头</span><span class="sxs-lookup"><span data-stu-id="0c236-120">Header</span></span>|<span data-ttu-id="0c236-121">值</span><span class="sxs-lookup"><span data-stu-id="0c236-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0c236-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0c236-122">Authorization</span></span>|<span data-ttu-id="0c236-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0c236-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0c236-124">接受</span><span class="sxs-lookup"><span data-stu-id="0c236-124">Accept</span></span>|<span data-ttu-id="0c236-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0c236-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0c236-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0c236-126">Request body</span></span>
<span data-ttu-id="0c236-127">在请求正文中，提供 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0c236-127">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="0c236-128">下表显示了创建 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0c236-128">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="0c236-129">属性</span><span class="sxs-lookup"><span data-stu-id="0c236-129">Property</span></span>|<span data-ttu-id="0c236-130">类型</span><span class="sxs-lookup"><span data-stu-id="0c236-130">Type</span></span>|<span data-ttu-id="0c236-131">说明</span><span class="sxs-lookup"><span data-stu-id="0c236-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0c236-132">id</span><span class="sxs-lookup"><span data-stu-id="0c236-132">id</span></span>|<span data-ttu-id="0c236-133">String</span><span class="sxs-lookup"><span data-stu-id="0c236-133">String</span></span>|<span data-ttu-id="0c236-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0c236-134">Key of the entity.</span></span>|
|<span data-ttu-id="0c236-135">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="0c236-135">gracePeriodHours</span></span>|<span data-ttu-id="0c236-136">Int32</span><span class="sxs-lookup"><span data-stu-id="0c236-136">Int32</span></span>|<span data-ttu-id="0c236-137">强制执行操作前要等待的小时数。</span><span class="sxs-lookup"><span data-stu-id="0c236-137">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="0c236-138">有效值为 0 至 8760</span><span class="sxs-lookup"><span data-stu-id="0c236-138">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="0c236-139">actionType</span><span class="sxs-lookup"><span data-stu-id="0c236-139">actionType</span></span>|[<span data-ttu-id="0c236-140">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="0c236-140">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="0c236-141">要执行的操作。</span><span class="sxs-lookup"><span data-stu-id="0c236-141">What action to take.</span></span> <span data-ttu-id="0c236-142">可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock`。</span><span class="sxs-lookup"><span data-stu-id="0c236-142">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="0c236-143">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="0c236-143">notificationTemplateId</span></span>|<span data-ttu-id="0c236-144">String</span><span class="sxs-lookup"><span data-stu-id="0c236-144">String</span></span>|<span data-ttu-id="0c236-145">要使用的通知消息模板</span><span class="sxs-lookup"><span data-stu-id="0c236-145">What notification Message template to use</span></span>|
|<span data-ttu-id="0c236-146">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="0c236-146">notificationMessageCCList</span></span>|<span data-ttu-id="0c236-147">String collection</span><span class="sxs-lookup"><span data-stu-id="0c236-147">String collection</span></span>|<span data-ttu-id="0c236-148">指定此通知邮件抄送对象的组 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="0c236-148">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="0c236-149">响应</span><span class="sxs-lookup"><span data-stu-id="0c236-149">Response</span></span>
<span data-ttu-id="0c236-150">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0c236-150">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0c236-151">示例</span><span class="sxs-lookup"><span data-stu-id="0c236-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="0c236-152">请求</span><span class="sxs-lookup"><span data-stu-id="0c236-152">Request</span></span>
<span data-ttu-id="0c236-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0c236-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
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

### <a name="response"></a><span data-ttu-id="0c236-154">响应</span><span class="sxs-lookup"><span data-stu-id="0c236-154">Response</span></span>
<span data-ttu-id="0c236-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0c236-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





