---
title: 更新 deviceManagementExchangeOnPremisesPolicy
description: 更新 deviceManagementExchangeOnPremisesPolicy 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 3fff7cd3bbcacbbfdbff9156c805381d59a6dffe
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941720"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="e8b62-103">更新 deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="e8b62-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

> <span data-ttu-id="e8b62-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e8b62-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e8b62-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e8b62-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e8b62-106">更新[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e8b62-106">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e8b62-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e8b62-107">Prerequisites</span></span>
<span data-ttu-id="e8b62-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e8b62-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8b62-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8b62-110">Permission type</span></span>|<span data-ttu-id="e8b62-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e8b62-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8b62-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8b62-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e8b62-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8b62-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="e8b62-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8b62-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8b62-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8b62-115">Not supported.</span></span>|
|<span data-ttu-id="e8b62-116">Application</span><span class="sxs-lookup"><span data-stu-id="e8b62-116">Application</span></span>|<span data-ttu-id="e8b62-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8b62-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8b62-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8b62-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="e8b62-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8b62-119">Request headers</span></span>
|<span data-ttu-id="e8b62-120">标头</span><span class="sxs-lookup"><span data-stu-id="e8b62-120">Header</span></span>|<span data-ttu-id="e8b62-121">值</span><span class="sxs-lookup"><span data-stu-id="e8b62-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8b62-122">授权</span><span class="sxs-lookup"><span data-stu-id="e8b62-122">Authorization</span></span>|<span data-ttu-id="e8b62-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e8b62-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8b62-124">接受</span><span class="sxs-lookup"><span data-stu-id="e8b62-124">Accept</span></span>|<span data-ttu-id="e8b62-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e8b62-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8b62-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8b62-126">Request body</span></span>
<span data-ttu-id="e8b62-127">在请求正文中，提供[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8b62-127">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="e8b62-128">下表显示创建[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e8b62-128">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="e8b62-129">属性</span><span class="sxs-lookup"><span data-stu-id="e8b62-129">Property</span></span>|<span data-ttu-id="e8b62-130">类型</span><span class="sxs-lookup"><span data-stu-id="e8b62-130">Type</span></span>|<span data-ttu-id="e8b62-131">说明</span><span class="sxs-lookup"><span data-stu-id="e8b62-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8b62-132">id</span><span class="sxs-lookup"><span data-stu-id="e8b62-132">id</span></span>|<span data-ttu-id="e8b62-133">字符串</span><span class="sxs-lookup"><span data-stu-id="e8b62-133">String</span></span>|<span data-ttu-id="e8b62-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="e8b62-134">Not yet documented</span></span>|
|<span data-ttu-id="e8b62-135">notificationContent</span><span class="sxs-lookup"><span data-stu-id="e8b62-135">notificationContent</span></span>|<span data-ttu-id="e8b62-136">Binary</span><span class="sxs-lookup"><span data-stu-id="e8b62-136">Binary</span></span>|<span data-ttu-id="e8b62-137">将发送给此策略隔离的用户的通知文本。</span><span class="sxs-lookup"><span data-stu-id="e8b62-137">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="e8b62-138">这是 UTF8 编码的字节数组 HTML。</span><span class="sxs-lookup"><span data-stu-id="e8b62-138">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="e8b62-139">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="e8b62-139">defaultAccessLevel</span></span>|[<span data-ttu-id="e8b62-140">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="e8b62-140">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="e8b62-141">Exchange 中的默认访问状态。</span><span class="sxs-lookup"><span data-stu-id="e8b62-141">Default access state in Exchange.</span></span> <span data-ttu-id="e8b62-142">此规则全局应用于整个 Exchange 组织。</span><span class="sxs-lookup"><span data-stu-id="e8b62-142">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="e8b62-143">可取值为：`none`、`allow`、`block`、`quarantine`。</span><span class="sxs-lookup"><span data-stu-id="e8b62-143">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="e8b62-144">accessRules</span><span class="sxs-lookup"><span data-stu-id="e8b62-144">accessRules</span></span>|<span data-ttu-id="e8b62-145">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md)集合</span><span class="sxs-lookup"><span data-stu-id="e8b62-145">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="e8b62-146">Exchange 中的设备访问规则列表。</span><span class="sxs-lookup"><span data-stu-id="e8b62-146">The list of device access rules in Exchange.</span></span> <span data-ttu-id="e8b62-147">访问规则全局应用于整个 Exchange 组织</span><span class="sxs-lookup"><span data-stu-id="e8b62-147">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="e8b62-148">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="e8b62-148">knownDeviceClasses</span></span>|<span data-ttu-id="e8b62-149">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md)集合</span><span class="sxs-lookup"><span data-stu-id="e8b62-149">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="e8b62-150">已知的 Exchange 设备类别的列表</span><span class="sxs-lookup"><span data-stu-id="e8b62-150">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="e8b62-151">响应</span><span class="sxs-lookup"><span data-stu-id="e8b62-151">Response</span></span>
<span data-ttu-id="e8b62-152">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e8b62-152">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8b62-153">示例</span><span class="sxs-lookup"><span data-stu-id="e8b62-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="e8b62-154">请求</span><span class="sxs-lookup"><span data-stu-id="e8b62-154">Request</span></span>
<span data-ttu-id="e8b62-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e8b62-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/exchangeOnPremisesPolicy
Content-type: application/json
Content-length: 665

{
  "@odata.type": "#microsoft.graph.deviceManagementExchangeOnPremisesPolicy",
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

### <a name="response"></a><span data-ttu-id="e8b62-156">响应</span><span class="sxs-lookup"><span data-stu-id="e8b62-156">Response</span></span>
<span data-ttu-id="e8b62-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e8b62-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





