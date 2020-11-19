---
title: 更新 deviceComplianceActionItem
description: 更新 deviceComplianceActionItem 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 953f615d5de7cc0cc8ae587d8a514e5d856072ef
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49292686"
---
# <a name="update-devicecomplianceactionitem"></a><span data-ttu-id="5816b-103">更新 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="5816b-103">Update deviceComplianceActionItem</span></span>

<span data-ttu-id="5816b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5816b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5816b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5816b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5816b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5816b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5816b-107">更新 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5816b-107">Update the properties of a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5816b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5816b-108">Prerequisites</span></span>
<span data-ttu-id="5816b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5816b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5816b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5816b-111">Permission type</span></span>|<span data-ttu-id="5816b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5816b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5816b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5816b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5816b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5816b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="5816b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5816b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5816b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5816b-116">Not supported.</span></span>|
|<span data-ttu-id="5816b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5816b-117">Application</span></span>|<span data-ttu-id="5816b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5816b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5816b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5816b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations/{deviceComplianceActionItemId}
```

## <a name="request-headers"></a><span data-ttu-id="5816b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5816b-120">Request headers</span></span>
|<span data-ttu-id="5816b-121">标头</span><span class="sxs-lookup"><span data-stu-id="5816b-121">Header</span></span>|<span data-ttu-id="5816b-122">值</span><span class="sxs-lookup"><span data-stu-id="5816b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5816b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5816b-123">Authorization</span></span>|<span data-ttu-id="5816b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5816b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5816b-125">接受</span><span class="sxs-lookup"><span data-stu-id="5816b-125">Accept</span></span>|<span data-ttu-id="5816b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5816b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5816b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5816b-127">Request body</span></span>
<span data-ttu-id="5816b-128">在请求正文中，提供 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5816b-128">In the request body, supply a JSON representation for the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>

<span data-ttu-id="5816b-129">下表显示了创建 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5816b-129">The following table shows the properties that are required when you create the [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md).</span></span>

|<span data-ttu-id="5816b-130">属性</span><span class="sxs-lookup"><span data-stu-id="5816b-130">Property</span></span>|<span data-ttu-id="5816b-131">类型</span><span class="sxs-lookup"><span data-stu-id="5816b-131">Type</span></span>|<span data-ttu-id="5816b-132">说明</span><span class="sxs-lookup"><span data-stu-id="5816b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5816b-133">id</span><span class="sxs-lookup"><span data-stu-id="5816b-133">id</span></span>|<span data-ttu-id="5816b-134">字符串</span><span class="sxs-lookup"><span data-stu-id="5816b-134">String</span></span>|<span data-ttu-id="5816b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5816b-135">Key of the entity.</span></span>|
|<span data-ttu-id="5816b-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="5816b-136">gracePeriodHours</span></span>|<span data-ttu-id="5816b-137">Int32</span><span class="sxs-lookup"><span data-stu-id="5816b-137">Int32</span></span>|<span data-ttu-id="5816b-138">强制执行操作前要等待的小时数。</span><span class="sxs-lookup"><span data-stu-id="5816b-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="5816b-139">有效值为 0 至 8760</span><span class="sxs-lookup"><span data-stu-id="5816b-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="5816b-140">actionType</span><span class="sxs-lookup"><span data-stu-id="5816b-140">actionType</span></span>|[<span data-ttu-id="5816b-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="5816b-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="5816b-142">要执行的操作。</span><span class="sxs-lookup"><span data-stu-id="5816b-142">What action to take.</span></span> <span data-ttu-id="5816b-143">可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock`。</span><span class="sxs-lookup"><span data-stu-id="5816b-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="5816b-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="5816b-144">notificationTemplateId</span></span>|<span data-ttu-id="5816b-145">String</span><span class="sxs-lookup"><span data-stu-id="5816b-145">String</span></span>|<span data-ttu-id="5816b-146">要使用的通知消息模板</span><span class="sxs-lookup"><span data-stu-id="5816b-146">What notification Message template to use</span></span>|
|<span data-ttu-id="5816b-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="5816b-147">notificationMessageCCList</span></span>|<span data-ttu-id="5816b-148">String collection</span><span class="sxs-lookup"><span data-stu-id="5816b-148">String collection</span></span>|<span data-ttu-id="5816b-149">指定此通知邮件抄送对象的组 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="5816b-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="5816b-150">响应</span><span class="sxs-lookup"><span data-stu-id="5816b-150">Response</span></span>
<span data-ttu-id="5816b-151">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5816b-151">If successful, this method returns a `200 OK` response code and an updated [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5816b-152">示例</span><span class="sxs-lookup"><span data-stu-id="5816b-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="5816b-153">请求</span><span class="sxs-lookup"><span data-stu-id="5816b-153">Request</span></span>
<span data-ttu-id="5816b-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5816b-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="5816b-155">响应</span><span class="sxs-lookup"><span data-stu-id="5816b-155">Response</span></span>
<span data-ttu-id="5816b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5816b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




