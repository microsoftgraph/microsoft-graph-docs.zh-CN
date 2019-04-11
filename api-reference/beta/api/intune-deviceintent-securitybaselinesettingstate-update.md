---
title: 更新 securityBaselineSettingState
description: 更新 securityBaselineSettingState 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: c65f3c49159f6025ae32ee9a12c7acc395742509
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31787741"
---
# <a name="update-securitybaselinesettingstate"></a><span data-ttu-id="dff35-103">更新 securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="dff35-103">Update securityBaselineSettingState</span></span>

> <span data-ttu-id="dff35-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dff35-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dff35-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dff35-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dff35-106">更新[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="dff35-106">Update the properties of a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dff35-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="dff35-107">Prerequisites</span></span>
<span data-ttu-id="dff35-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dff35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dff35-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="dff35-110">Permission type</span></span>|<span data-ttu-id="dff35-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dff35-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dff35-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dff35-112">Delegated (work or school account)</span></span>|<span data-ttu-id="dff35-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dff35-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dff35-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dff35-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dff35-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="dff35-115">Not supported.</span></span>|
|<span data-ttu-id="dff35-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="dff35-116">Application</span></span>|<span data-ttu-id="dff35-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="dff35-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="dff35-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dff35-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
```

## <a name="request-headers"></a><span data-ttu-id="dff35-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="dff35-119">Request headers</span></span>
|<span data-ttu-id="dff35-120">标头</span><span class="sxs-lookup"><span data-stu-id="dff35-120">Header</span></span>|<span data-ttu-id="dff35-121">值</span><span class="sxs-lookup"><span data-stu-id="dff35-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dff35-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="dff35-122">Authorization</span></span>|<span data-ttu-id="dff35-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dff35-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dff35-124">接受</span><span class="sxs-lookup"><span data-stu-id="dff35-124">Accept</span></span>|<span data-ttu-id="dff35-125">application/json</span><span class="sxs-lookup"><span data-stu-id="dff35-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dff35-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="dff35-126">Request body</span></span>
<span data-ttu-id="dff35-127">在请求正文中, 提供[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dff35-127">In the request body, supply a JSON representation for the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>

<span data-ttu-id="dff35-128">下表显示创建[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dff35-128">The following table shows the properties that are required when you create the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md).</span></span>

|<span data-ttu-id="dff35-129">属性</span><span class="sxs-lookup"><span data-stu-id="dff35-129">Property</span></span>|<span data-ttu-id="dff35-130">类型</span><span class="sxs-lookup"><span data-stu-id="dff35-130">Type</span></span>|<span data-ttu-id="dff35-131">说明</span><span class="sxs-lookup"><span data-stu-id="dff35-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dff35-132">id</span><span class="sxs-lookup"><span data-stu-id="dff35-132">id</span></span>|<span data-ttu-id="dff35-133">String</span><span class="sxs-lookup"><span data-stu-id="dff35-133">String</span></span>|<span data-ttu-id="dff35-134">实体的唯一标识符</span><span class="sxs-lookup"><span data-stu-id="dff35-134">Unique identifier of the entity</span></span>|
|<span data-ttu-id="dff35-135">settingName</span><span class="sxs-lookup"><span data-stu-id="dff35-135">settingName</span></span>|<span data-ttu-id="dff35-136">String</span><span class="sxs-lookup"><span data-stu-id="dff35-136">String</span></span>|<span data-ttu-id="dff35-137">报告的设置名称</span><span class="sxs-lookup"><span data-stu-id="dff35-137">The setting name that is being reported</span></span>|
|<span data-ttu-id="dff35-138">state</span><span class="sxs-lookup"><span data-stu-id="dff35-138">state</span></span>|[<span data-ttu-id="dff35-139">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="dff35-139">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="dff35-140">安全基准设置的符合性状态。</span><span class="sxs-lookup"><span data-stu-id="dff35-140">The compliance state of the security baseline setting.</span></span> <span data-ttu-id="dff35-141">可取值为：`unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict`。</span><span class="sxs-lookup"><span data-stu-id="dff35-141">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="dff35-142">settingCategoryId</span><span class="sxs-lookup"><span data-stu-id="dff35-142">settingCategoryId</span></span>|<span data-ttu-id="dff35-143">String</span><span class="sxs-lookup"><span data-stu-id="dff35-143">String</span></span>|<span data-ttu-id="dff35-144">此设置所属的设置类别 id</span><span class="sxs-lookup"><span data-stu-id="dff35-144">The setting category id which this setting belongs to</span></span>|



## <a name="response"></a><span data-ttu-id="dff35-145">响应</span><span class="sxs-lookup"><span data-stu-id="dff35-145">Response</span></span>
<span data-ttu-id="dff35-146">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)对象。</span><span class="sxs-lookup"><span data-stu-id="dff35-146">If successful, this method returns a `200 OK` response code and an updated [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dff35-147">示例</span><span class="sxs-lookup"><span data-stu-id="dff35-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="dff35-148">请求</span><span class="sxs-lookup"><span data-stu-id="dff35-148">Request</span></span>
<span data-ttu-id="dff35-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dff35-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managedDevices/{managedDeviceId}/securityBaselineStates/{securityBaselineStateId}/settingStates/{securityBaselineSettingStateId}
Content-type: application/json
Content-length: 185

{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "settingName": "Setting Name value",
  "state": "secure",
  "settingCategoryId": "Setting Category Id value"
}
```

### <a name="response"></a><span data-ttu-id="dff35-150">响应</span><span class="sxs-lookup"><span data-stu-id="dff35-150">Response</span></span>
<span data-ttu-id="dff35-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dff35-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 234

{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "id": "798e520d-520d-798e-0d52-8e790d528e79",
  "settingName": "Setting Name value",
  "state": "secure",
  "settingCategoryId": "Setting Category Id value"
}
```



