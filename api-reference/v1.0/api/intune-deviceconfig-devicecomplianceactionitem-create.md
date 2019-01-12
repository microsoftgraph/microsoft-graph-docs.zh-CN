---
title: 创建 deviceComplianceActionItem
description: 创建新的 deviceComplianceActionItem 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: cd7cb91d6dde4755f27bdc28b3fb1c0c8804a800
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27972059"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="db3a7-103">创建 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="db3a7-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="db3a7-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="db3a7-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="db3a7-105">创建新的 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db3a7-105">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="db3a7-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="db3a7-106">Prerequisites</span></span>
<span data-ttu-id="db3a7-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="db3a7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="db3a7-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="db3a7-109">Permission type</span></span>|<span data-ttu-id="db3a7-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="db3a7-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="db3a7-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="db3a7-111">Delegated (work or school account)</span></span>|<span data-ttu-id="db3a7-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="db3a7-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="db3a7-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="db3a7-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="db3a7-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="db3a7-114">Not supported.</span></span>|
|<span data-ttu-id="db3a7-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="db3a7-115">Application</span></span>|<span data-ttu-id="db3a7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="db3a7-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="db3a7-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="db3a7-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="db3a7-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="db3a7-118">Request headers</span></span>
|<span data-ttu-id="db3a7-119">标头</span><span class="sxs-lookup"><span data-stu-id="db3a7-119">Header</span></span>|<span data-ttu-id="db3a7-120">值</span><span class="sxs-lookup"><span data-stu-id="db3a7-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="db3a7-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="db3a7-121">Authorization</span></span>|<span data-ttu-id="db3a7-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="db3a7-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="db3a7-123">Accept</span><span class="sxs-lookup"><span data-stu-id="db3a7-123">Accept</span></span>|<span data-ttu-id="db3a7-124">application/json</span><span class="sxs-lookup"><span data-stu-id="db3a7-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="db3a7-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="db3a7-125">Request body</span></span>
<span data-ttu-id="db3a7-126">在请求正文中，提供 deviceComplianceActionItem 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="db3a7-126">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="db3a7-127">下表显示了创建 deviceComplianceActionItem 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="db3a7-127">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="db3a7-128">属性</span><span class="sxs-lookup"><span data-stu-id="db3a7-128">Property</span></span>|<span data-ttu-id="db3a7-129">类型</span><span class="sxs-lookup"><span data-stu-id="db3a7-129">Type</span></span>|<span data-ttu-id="db3a7-130">说明</span><span class="sxs-lookup"><span data-stu-id="db3a7-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="db3a7-131">id</span><span class="sxs-lookup"><span data-stu-id="db3a7-131">id</span></span>|<span data-ttu-id="db3a7-132">String</span><span class="sxs-lookup"><span data-stu-id="db3a7-132">String</span></span>|<span data-ttu-id="db3a7-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="db3a7-133">Key of the entity.</span></span>|
|<span data-ttu-id="db3a7-134">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="db3a7-134">gracePeriodHours</span></span>|<span data-ttu-id="db3a7-135">Int32</span><span class="sxs-lookup"><span data-stu-id="db3a7-135">Int32</span></span>|<span data-ttu-id="db3a7-136">强制执行操作前要等待的小时数。</span><span class="sxs-lookup"><span data-stu-id="db3a7-136">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="db3a7-137">有效值为 0 至 8760</span><span class="sxs-lookup"><span data-stu-id="db3a7-137">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="db3a7-138">actionType</span><span class="sxs-lookup"><span data-stu-id="db3a7-138">actionType</span></span>|[<span data-ttu-id="db3a7-139">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="db3a7-139">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="db3a7-140">要采取什么操作。</span><span class="sxs-lookup"><span data-stu-id="db3a7-140">What action to take.</span></span> <span data-ttu-id="db3a7-141">可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`。</span><span class="sxs-lookup"><span data-stu-id="db3a7-141">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`.</span></span>|
|<span data-ttu-id="db3a7-142">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="db3a7-142">notificationTemplateId</span></span>|<span data-ttu-id="db3a7-143">String</span><span class="sxs-lookup"><span data-stu-id="db3a7-143">String</span></span>|<span data-ttu-id="db3a7-144">要使用的通知消息模板</span><span class="sxs-lookup"><span data-stu-id="db3a7-144">What notification Message template to use</span></span>|
|<span data-ttu-id="db3a7-145">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="db3a7-145">notificationMessageCCList</span></span>|<span data-ttu-id="db3a7-146">String 集合</span><span class="sxs-lookup"><span data-stu-id="db3a7-146">String collection</span></span>|<span data-ttu-id="db3a7-147">指定此通知邮件抄送对象的组 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="db3a7-147">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="db3a7-148">响应</span><span class="sxs-lookup"><span data-stu-id="db3a7-148">Response</span></span>
<span data-ttu-id="db3a7-149">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="db3a7-149">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="db3a7-150">示例</span><span class="sxs-lookup"><span data-stu-id="db3a7-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="db3a7-151">请求</span><span class="sxs-lookup"><span data-stu-id="db3a7-151">Request</span></span>
<span data-ttu-id="db3a7-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="db3a7-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
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

### <a name="response"></a><span data-ttu-id="db3a7-153">响应</span><span class="sxs-lookup"><span data-stu-id="db3a7-153">Response</span></span>
<span data-ttu-id="db3a7-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="db3a7-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



