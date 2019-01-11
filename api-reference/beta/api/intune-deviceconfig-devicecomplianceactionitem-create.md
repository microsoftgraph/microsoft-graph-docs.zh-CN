---
title: 创建 deviceComplianceActionItem
description: 创建新的 deviceComplianceActionItem 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 282babf1cf567752885858bbb397977b095a7a34
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27873610"
---
# <a name="create-devicecomplianceactionitem"></a><span data-ttu-id="b6163-103">创建 deviceComplianceActionItem</span><span class="sxs-lookup"><span data-stu-id="b6163-103">Create deviceComplianceActionItem</span></span>

> <span data-ttu-id="b6163-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b6163-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b6163-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b6163-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6163-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="b6163-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="b6163-107">创建新的 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b6163-107">Create a new [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="b6163-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b6163-108">Prerequisites</span></span>
<span data-ttu-id="b6163-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="b6163-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6163-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6163-111">Permission type</span></span>|<span data-ttu-id="b6163-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b6163-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6163-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6163-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6163-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6163-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b6163-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6163-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6163-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6163-116">Not supported.</span></span>|
|<span data-ttu-id="b6163-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6163-117">Application</span></span>|<span data-ttu-id="b6163-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6163-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6163-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6163-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceCompliancePolicies/{deviceCompliancePolicyId}/scheduledActionsForRule/{deviceComplianceScheduledActionForRuleId}/scheduledActionConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b6163-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6163-120">Request headers</span></span>
|<span data-ttu-id="b6163-121">标头</span><span class="sxs-lookup"><span data-stu-id="b6163-121">Header</span></span>|<span data-ttu-id="b6163-122">值</span><span class="sxs-lookup"><span data-stu-id="b6163-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6163-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6163-123">Authorization</span></span>|<span data-ttu-id="b6163-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b6163-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6163-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b6163-125">Accept</span></span>|<span data-ttu-id="b6163-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6163-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6163-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6163-127">Request body</span></span>
<span data-ttu-id="b6163-128">在请求正文中，提供 deviceComplianceActionItem 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6163-128">In the request body, supply a JSON representation for the deviceComplianceActionItem object.</span></span>

<span data-ttu-id="b6163-129">下表显示了创建 deviceComplianceActionItem 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b6163-129">The following table shows the properties that are required when you create the deviceComplianceActionItem.</span></span>

|<span data-ttu-id="b6163-130">属性</span><span class="sxs-lookup"><span data-stu-id="b6163-130">Property</span></span>|<span data-ttu-id="b6163-131">类型</span><span class="sxs-lookup"><span data-stu-id="b6163-131">Type</span></span>|<span data-ttu-id="b6163-132">说明</span><span class="sxs-lookup"><span data-stu-id="b6163-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6163-133">id</span><span class="sxs-lookup"><span data-stu-id="b6163-133">id</span></span>|<span data-ttu-id="b6163-134">String</span><span class="sxs-lookup"><span data-stu-id="b6163-134">String</span></span>|<span data-ttu-id="b6163-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b6163-135">Key of the entity.</span></span>|
|<span data-ttu-id="b6163-136">gracePeriodHours</span><span class="sxs-lookup"><span data-stu-id="b6163-136">gracePeriodHours</span></span>|<span data-ttu-id="b6163-137">Int32</span><span class="sxs-lookup"><span data-stu-id="b6163-137">Int32</span></span>|<span data-ttu-id="b6163-138">强制执行操作前要等待的小时数。</span><span class="sxs-lookup"><span data-stu-id="b6163-138">Number of hours to wait till the action will be enforced.</span></span> <span data-ttu-id="b6163-139">有效值为 0 至 8760</span><span class="sxs-lookup"><span data-stu-id="b6163-139">Valid values 0 to 8760</span></span>|
|<span data-ttu-id="b6163-140">actionType</span><span class="sxs-lookup"><span data-stu-id="b6163-140">actionType</span></span>|[<span data-ttu-id="b6163-141">deviceComplianceActionType</span><span class="sxs-lookup"><span data-stu-id="b6163-141">deviceComplianceActionType</span></span>](../resources/intune-deviceconfig-devicecomplianceactiontype.md)|<span data-ttu-id="b6163-142">要采取什么操作。</span><span class="sxs-lookup"><span data-stu-id="b6163-142">What action to take.</span></span> <span data-ttu-id="b6163-143">可取值为：`noAction`、`notification`、`block`、`retire`、`wipe`、`removeResourceAccessProfiles`、`pushNotification`、`remoteLock`。</span><span class="sxs-lookup"><span data-stu-id="b6163-143">Possible values are: `noAction`, `notification`, `block`, `retire`, `wipe`, `removeResourceAccessProfiles`, `pushNotification`, `remoteLock`.</span></span>|
|<span data-ttu-id="b6163-144">notificationTemplateId</span><span class="sxs-lookup"><span data-stu-id="b6163-144">notificationTemplateId</span></span>|<span data-ttu-id="b6163-145">String</span><span class="sxs-lookup"><span data-stu-id="b6163-145">String</span></span>|<span data-ttu-id="b6163-146">要使用的通知消息模板</span><span class="sxs-lookup"><span data-stu-id="b6163-146">What notification Message template to use</span></span>|
|<span data-ttu-id="b6163-147">notificationMessageCCList</span><span class="sxs-lookup"><span data-stu-id="b6163-147">notificationMessageCCList</span></span>|<span data-ttu-id="b6163-148">String 集合</span><span class="sxs-lookup"><span data-stu-id="b6163-148">String collection</span></span>|<span data-ttu-id="b6163-149">指定此通知邮件抄送对象的组 ID 列表。</span><span class="sxs-lookup"><span data-stu-id="b6163-149">A list of group IDs to speicify who to CC this notification message to.</span></span>|



## <a name="response"></a><span data-ttu-id="b6163-150">响应</span><span class="sxs-lookup"><span data-stu-id="b6163-150">Response</span></span>
<span data-ttu-id="b6163-151">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b6163-151">If successful, this method returns a `201 Created` response code and a [deviceComplianceActionItem](../resources/intune-deviceconfig-devicecomplianceactionitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6163-152">示例</span><span class="sxs-lookup"><span data-stu-id="b6163-152">Example</span></span>
### <a name="request"></a><span data-ttu-id="b6163-153">请求</span><span class="sxs-lookup"><span data-stu-id="b6163-153">Request</span></span>
<span data-ttu-id="b6163-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b6163-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b6163-155">响应</span><span class="sxs-lookup"><span data-stu-id="b6163-155">Response</span></span>
<span data-ttu-id="b6163-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b6163-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





