---
title: 更新 deviceManagementExchangeOnPremisesPolicy
description: 更新 deviceManagementExchangeOnPremisesPolicy 对象的属性。
ms.openlocfilehash: afc3df27d79b2cefab434126da8971f0fff5c8e4
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27042672"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="265f4-103">更新 deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="265f4-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="265f4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="265f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="265f4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="265f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="265f4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="265f4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="265f4-107">更新[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="265f4-107">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="265f4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="265f4-108">Prerequisites</span></span>
<span data-ttu-id="265f4-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="265f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="265f4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="265f4-111">Permission type</span></span>|<span data-ttu-id="265f4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="265f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="265f4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="265f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="265f4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="265f4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="265f4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="265f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="265f4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="265f4-116">Not supported.</span></span>|
|<span data-ttu-id="265f4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="265f4-117">Application</span></span>|<span data-ttu-id="265f4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="265f4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="265f4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="265f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="265f4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="265f4-120">Request headers</span></span>
|<span data-ttu-id="265f4-121">标头</span><span class="sxs-lookup"><span data-stu-id="265f4-121">Header</span></span>|<span data-ttu-id="265f4-122">值</span><span class="sxs-lookup"><span data-stu-id="265f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="265f4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="265f4-123">Authorization</span></span>|<span data-ttu-id="265f4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="265f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="265f4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="265f4-125">Accept</span></span>|<span data-ttu-id="265f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="265f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="265f4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="265f4-127">Request body</span></span>
<span data-ttu-id="265f4-128">在请求正文中，提供[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="265f4-128">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="265f4-129">下表显示时创建[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="265f4-129">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="265f4-130">属性</span><span class="sxs-lookup"><span data-stu-id="265f4-130">Property</span></span>|<span data-ttu-id="265f4-131">类型</span><span class="sxs-lookup"><span data-stu-id="265f4-131">Type</span></span>|<span data-ttu-id="265f4-132">说明</span><span class="sxs-lookup"><span data-stu-id="265f4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="265f4-133">id</span><span class="sxs-lookup"><span data-stu-id="265f4-133">id</span></span>|<span data-ttu-id="265f4-134">字符串</span><span class="sxs-lookup"><span data-stu-id="265f4-134">String</span></span>|<span data-ttu-id="265f4-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="265f4-135">Not yet documented</span></span>|
|<span data-ttu-id="265f4-136">notificationContent</span><span class="sxs-lookup"><span data-stu-id="265f4-136">notificationContent</span></span>|<span data-ttu-id="265f4-137">二进制数</span><span class="sxs-lookup"><span data-stu-id="265f4-137">Binary</span></span>|<span data-ttu-id="265f4-138">将发送到隔离通过此策略的用户的通知文本。</span><span class="sxs-lookup"><span data-stu-id="265f4-138">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="265f4-139">这是 UTF8 编码字节数组 HTML。</span><span class="sxs-lookup"><span data-stu-id="265f4-139">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="265f4-140">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="265f4-140">defaultAccessLevel</span></span>|[<span data-ttu-id="265f4-141">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="265f4-141">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="265f4-142">Exchange 中的默认访问状态。</span><span class="sxs-lookup"><span data-stu-id="265f4-142">Default access state in Exchange.</span></span> <span data-ttu-id="265f4-143">此规则全局适用于整个 Exchange 组织。</span><span class="sxs-lookup"><span data-stu-id="265f4-143">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="265f4-144">可取值为：`none`、`allow`、`block`、`quarantine`。</span><span class="sxs-lookup"><span data-stu-id="265f4-144">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="265f4-145">accessRules</span><span class="sxs-lookup"><span data-stu-id="265f4-145">accessRules</span></span>|<span data-ttu-id="265f4-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="265f4-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="265f4-147">在 Exchange 规则设备访问的列表。</span><span class="sxs-lookup"><span data-stu-id="265f4-147">The list of device access rules in Exchange.</span></span> <span data-ttu-id="265f4-148">访问规则应用于整个 Exchange 组织的全局</span><span class="sxs-lookup"><span data-stu-id="265f4-148">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="265f4-149">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="265f4-149">knownDeviceClasses</span></span>|<span data-ttu-id="265f4-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)集合</span><span class="sxs-lookup"><span data-stu-id="265f4-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="265f4-151">已知到 Exchange 的设备类列表</span><span class="sxs-lookup"><span data-stu-id="265f4-151">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="265f4-152">响应</span><span class="sxs-lookup"><span data-stu-id="265f4-152">Response</span></span>
<span data-ttu-id="265f4-153">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="265f4-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="265f4-154">示例</span><span class="sxs-lookup"><span data-stu-id="265f4-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="265f4-155">请求</span><span class="sxs-lookup"><span data-stu-id="265f4-155">Request</span></span>
<span data-ttu-id="265f4-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="265f4-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
Content-type: application/json
Content-length: 586

{
  "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
  "defaultAccessLevel": "allow",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      },
      "accessLevel": "allow"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "Name value",
      "type": "model"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="265f4-157">响应</span><span class="sxs-lookup"><span data-stu-id="265f4-157">Response</span></span>
<span data-ttu-id="265f4-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="265f4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 714

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
  "id": "16e76336-6336-16e7-3663-e7163663e716",
  "notificationContent": "bm90aWZpY2F0aW9uQ29udGVudA==",
  "defaultAccessLevel": "allow",
  "accessRules": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeAccessRule",
      "deviceClass": {
        "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
        "name": "Name value",
        "type": "model"
      },
      "accessLevel": "allow"
    }
  ],
  "knownDeviceClasses": [
    {
      "@odata.type": "microsoft.graph.deviceManagementExchangeDeviceClass",
      "name": "Name value",
      "type": "model"
    }
  ]
}
```





