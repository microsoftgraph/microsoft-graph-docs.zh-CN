---
title: 更新 deviceManagementExchangeOnPremisesPolicy
description: 更新 deviceManagementExchangeOnPremisesPolicy 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0d1aaec016c95845c0f33ede2f413811a58fa44c
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156889"
---
# <a name="update-devicemanagementexchangeonpremisespolicy"></a><span data-ttu-id="65c29-103">更新 deviceManagementExchangeOnPremisesPolicy</span><span class="sxs-lookup"><span data-stu-id="65c29-103">Update deviceManagementExchangeOnPremisesPolicy</span></span>

<span data-ttu-id="65c29-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65c29-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="65c29-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="65c29-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="65c29-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="65c29-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="65c29-107">更新 [deviceManagementExchangeOnPremisesPolicy 对象](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="65c29-107">Update the properties of a [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="65c29-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="65c29-108">Prerequisites</span></span>
<span data-ttu-id="65c29-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65c29-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="65c29-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="65c29-111">Permission type</span></span>|<span data-ttu-id="65c29-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="65c29-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="65c29-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65c29-113">Delegated (work or school account)</span></span>|<span data-ttu-id="65c29-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65c29-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="65c29-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65c29-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65c29-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="65c29-116">Not supported.</span></span>|
|<span data-ttu-id="65c29-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="65c29-117">Application</span></span>|<span data-ttu-id="65c29-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="65c29-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="65c29-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65c29-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/exchangeOnPremisesPolicy
PATCH /deviceManagement/exchangeOnPremisesPolicies/{deviceManagementExchangeOnPremisesPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="65c29-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="65c29-120">Request headers</span></span>
|<span data-ttu-id="65c29-121">标头</span><span class="sxs-lookup"><span data-stu-id="65c29-121">Header</span></span>|<span data-ttu-id="65c29-122">值</span><span class="sxs-lookup"><span data-stu-id="65c29-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="65c29-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="65c29-123">Authorization</span></span>|<span data-ttu-id="65c29-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="65c29-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="65c29-125">接受</span><span class="sxs-lookup"><span data-stu-id="65c29-125">Accept</span></span>|<span data-ttu-id="65c29-126">application/json</span><span class="sxs-lookup"><span data-stu-id="65c29-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="65c29-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="65c29-127">Request body</span></span>
<span data-ttu-id="65c29-128">在请求正文中，提供 [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65c29-128">In the request body, supply a JSON representation for the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object.</span></span>

<span data-ttu-id="65c29-129">下表显示创建 [deviceManagementExchangeOnPremisesPolicy 时所需的属性](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="65c29-129">The following table shows the properties that are required when you create the [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md).</span></span>

|<span data-ttu-id="65c29-130">属性</span><span class="sxs-lookup"><span data-stu-id="65c29-130">Property</span></span>|<span data-ttu-id="65c29-131">类型</span><span class="sxs-lookup"><span data-stu-id="65c29-131">Type</span></span>|<span data-ttu-id="65c29-132">说明</span><span class="sxs-lookup"><span data-stu-id="65c29-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="65c29-133">id</span><span class="sxs-lookup"><span data-stu-id="65c29-133">id</span></span>|<span data-ttu-id="65c29-134">String</span><span class="sxs-lookup"><span data-stu-id="65c29-134">String</span></span>|<span data-ttu-id="65c29-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="65c29-135">Not yet documented</span></span>|
|<span data-ttu-id="65c29-136">notificationContent</span><span class="sxs-lookup"><span data-stu-id="65c29-136">notificationContent</span></span>|<span data-ttu-id="65c29-137">Binary</span><span class="sxs-lookup"><span data-stu-id="65c29-137">Binary</span></span>|<span data-ttu-id="65c29-138">将发送给此策略隔离的用户的通知文本。</span><span class="sxs-lookup"><span data-stu-id="65c29-138">Notification text that will be sent to users quarantined by this policy.</span></span> <span data-ttu-id="65c29-139">这是 UTF8 编码的字节数组 HTML。</span><span class="sxs-lookup"><span data-stu-id="65c29-139">This is UTF8 encoded byte array HTML.</span></span>|
|<span data-ttu-id="65c29-140">defaultAccessLevel</span><span class="sxs-lookup"><span data-stu-id="65c29-140">defaultAccessLevel</span></span>|[<span data-ttu-id="65c29-141">deviceManagementExchangeAccessLevel</span><span class="sxs-lookup"><span data-stu-id="65c29-141">deviceManagementExchangeAccessLevel</span></span>](../resources/intune-onboarding-devicemanagementexchangeaccesslevel.md)|<span data-ttu-id="65c29-142">Exchange 中的默认访问状态。</span><span class="sxs-lookup"><span data-stu-id="65c29-142">Default access state in Exchange.</span></span> <span data-ttu-id="65c29-143">此规则全局应用于整个 Exchange 组织。</span><span class="sxs-lookup"><span data-stu-id="65c29-143">This rule applies globally to the entire Exchange organization.</span></span> <span data-ttu-id="65c29-144">可取值为：`none`、`allow`、`block`、`quarantine`。</span><span class="sxs-lookup"><span data-stu-id="65c29-144">Possible values are: `none`, `allow`, `block`, `quarantine`.</span></span>|
|<span data-ttu-id="65c29-145">accessRules</span><span class="sxs-lookup"><span data-stu-id="65c29-145">accessRules</span></span>|<span data-ttu-id="65c29-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) 集合</span><span class="sxs-lookup"><span data-stu-id="65c29-146">[deviceManagementExchangeAccessRule](../resources/intune-onboarding-devicemanagementexchangeaccessrule.md) collection</span></span>|<span data-ttu-id="65c29-147">Exchange 中的设备访问规则列表。</span><span class="sxs-lookup"><span data-stu-id="65c29-147">The list of device access rules in Exchange.</span></span> <span data-ttu-id="65c29-148">访问规则全局应用于整个 Exchange 组织</span><span class="sxs-lookup"><span data-stu-id="65c29-148">The access rules apply globally to the entire Exchange organization</span></span>|
|<span data-ttu-id="65c29-149">knownDeviceClasses</span><span class="sxs-lookup"><span data-stu-id="65c29-149">knownDeviceClasses</span></span>|<span data-ttu-id="65c29-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) 集合</span><span class="sxs-lookup"><span data-stu-id="65c29-150">[deviceManagementExchangeDeviceClass](../resources/intune-onboarding-devicemanagementexchangedeviceclass.md) collection</span></span>|<span data-ttu-id="65c29-151">Exchange 已知的设备类列表</span><span class="sxs-lookup"><span data-stu-id="65c29-151">The list of device classes known to Exchange</span></span>|



## <a name="response"></a><span data-ttu-id="65c29-152">响应</span><span class="sxs-lookup"><span data-stu-id="65c29-152">Response</span></span>
<span data-ttu-id="65c29-153">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="65c29-153">If successful, this method returns a `200 OK` response code and an updated [deviceManagementExchangeOnPremisesPolicy](../resources/intune-onboarding-devicemanagementexchangeonpremisespolicy.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="65c29-154">示例</span><span class="sxs-lookup"><span data-stu-id="65c29-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="65c29-155">请求</span><span class="sxs-lookup"><span data-stu-id="65c29-155">Request</span></span>
<span data-ttu-id="65c29-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="65c29-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="65c29-157">响应</span><span class="sxs-lookup"><span data-stu-id="65c29-157">Response</span></span>
<span data-ttu-id="65c29-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="65c29-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




