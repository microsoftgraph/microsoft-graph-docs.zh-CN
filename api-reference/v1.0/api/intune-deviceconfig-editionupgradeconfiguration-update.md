---
title: 更新 editionUpgradeConfiguration
description: 更新 editionUpgradeConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7af5d21805b09565d2370fe283ae4b3dc8c3e54a
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48092242"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="a1a50-103">更新 editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="a1a50-103">Update editionUpgradeConfiguration</span></span>

<span data-ttu-id="a1a50-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a1a50-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a1a50-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a1a50-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a1a50-106">更新 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a1a50-106">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a1a50-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="a1a50-107">Prerequisites</span></span>
<span data-ttu-id="a1a50-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a1a50-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1a50-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1a50-110">Permission type</span></span>|<span data-ttu-id="a1a50-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a1a50-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1a50-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1a50-112">Delegated (work or school account)</span></span>|<span data-ttu-id="a1a50-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1a50-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a1a50-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1a50-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1a50-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1a50-115">Not supported.</span></span>|
|<span data-ttu-id="a1a50-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1a50-116">Application</span></span>|<span data-ttu-id="a1a50-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1a50-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1a50-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1a50-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="a1a50-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1a50-119">Request headers</span></span>
|<span data-ttu-id="a1a50-120">标头</span><span class="sxs-lookup"><span data-stu-id="a1a50-120">Header</span></span>|<span data-ttu-id="a1a50-121">值</span><span class="sxs-lookup"><span data-stu-id="a1a50-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1a50-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="a1a50-122">Authorization</span></span>|<span data-ttu-id="a1a50-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a1a50-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1a50-124">接受</span><span class="sxs-lookup"><span data-stu-id="a1a50-124">Accept</span></span>|<span data-ttu-id="a1a50-125">application/json</span><span class="sxs-lookup"><span data-stu-id="a1a50-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1a50-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1a50-126">Request body</span></span>
<span data-ttu-id="a1a50-127">在请求正文中，提供 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1a50-127">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="a1a50-128">下表显示创建 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a1a50-128">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="a1a50-129">属性</span><span class="sxs-lookup"><span data-stu-id="a1a50-129">Property</span></span>|<span data-ttu-id="a1a50-130">类型</span><span class="sxs-lookup"><span data-stu-id="a1a50-130">Type</span></span>|<span data-ttu-id="a1a50-131">说明</span><span class="sxs-lookup"><span data-stu-id="a1a50-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1a50-132">id</span><span class="sxs-lookup"><span data-stu-id="a1a50-132">id</span></span>|<span data-ttu-id="a1a50-133">String</span><span class="sxs-lookup"><span data-stu-id="a1a50-133">String</span></span>|<span data-ttu-id="a1a50-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a1a50-134">Key of the entity.</span></span> <span data-ttu-id="a1a50-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1a50-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1a50-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a1a50-136">lastModifiedDateTime</span></span>|<span data-ttu-id="a1a50-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1a50-137">DateTimeOffset</span></span>|<span data-ttu-id="a1a50-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a1a50-138">DateTime the object was last modified.</span></span> <span data-ttu-id="a1a50-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1a50-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1a50-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a1a50-140">createdDateTime</span></span>|<span data-ttu-id="a1a50-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a1a50-141">DateTimeOffset</span></span>|<span data-ttu-id="a1a50-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="a1a50-142">DateTime the object was created.</span></span> <span data-ttu-id="a1a50-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1a50-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1a50-144">description</span><span class="sxs-lookup"><span data-stu-id="a1a50-144">description</span></span>|<span data-ttu-id="a1a50-145">String</span><span class="sxs-lookup"><span data-stu-id="a1a50-145">String</span></span>|<span data-ttu-id="a1a50-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="a1a50-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="a1a50-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1a50-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1a50-148">displayName</span><span class="sxs-lookup"><span data-stu-id="a1a50-148">displayName</span></span>|<span data-ttu-id="a1a50-149">String</span><span class="sxs-lookup"><span data-stu-id="a1a50-149">String</span></span>|<span data-ttu-id="a1a50-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="a1a50-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="a1a50-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1a50-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1a50-152">version</span><span class="sxs-lookup"><span data-stu-id="a1a50-152">version</span></span>|<span data-ttu-id="a1a50-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a1a50-153">Int32</span></span>|<span data-ttu-id="a1a50-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="a1a50-154">Version of the device configuration.</span></span> <span data-ttu-id="a1a50-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="a1a50-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="a1a50-156">licenseType</span><span class="sxs-lookup"><span data-stu-id="a1a50-156">licenseType</span></span>|[<span data-ttu-id="a1a50-157">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="a1a50-157">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="a1a50-158">版本升级许可证类型。</span><span class="sxs-lookup"><span data-stu-id="a1a50-158">Edition Upgrade License Type.</span></span> <span data-ttu-id="a1a50-159">可取值为：`productKey`、`licenseFile`。</span><span class="sxs-lookup"><span data-stu-id="a1a50-159">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="a1a50-160">targetEdition</span><span class="sxs-lookup"><span data-stu-id="a1a50-160">targetEdition</span></span>|[<span data-ttu-id="a1a50-161">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="a1a50-161">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="a1a50-162">版本升级目标版本。</span><span class="sxs-lookup"><span data-stu-id="a1a50-162">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="a1a50-163">可取值为：`windows10Enterprise`、`windows10EnterpriseN`、`windows10Education`、`windows10EducationN`、`windows10MobileEnterprise`、`windows10HolographicEnterprise`、`windows10Professional`、`windows10ProfessionalN`、`windows10ProfessionalEducation`、`windows10ProfessionalEducationN`、`windows10ProfessionalWorkstation`、`windows10ProfessionalWorkstationN`。</span><span class="sxs-lookup"><span data-stu-id="a1a50-163">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="a1a50-164">license</span><span class="sxs-lookup"><span data-stu-id="a1a50-164">license</span></span>|<span data-ttu-id="a1a50-165">String</span><span class="sxs-lookup"><span data-stu-id="a1a50-165">String</span></span>|<span data-ttu-id="a1a50-166">版本升级许可证文件内容。</span><span class="sxs-lookup"><span data-stu-id="a1a50-166">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="a1a50-167">productKey</span><span class="sxs-lookup"><span data-stu-id="a1a50-167">productKey</span></span>|<span data-ttu-id="a1a50-168">String</span><span class="sxs-lookup"><span data-stu-id="a1a50-168">String</span></span>|<span data-ttu-id="a1a50-169">版本升级产品密钥。</span><span class="sxs-lookup"><span data-stu-id="a1a50-169">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="a1a50-170">响应</span><span class="sxs-lookup"><span data-stu-id="a1a50-170">Response</span></span>
<span data-ttu-id="a1a50-171">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a1a50-171">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1a50-172">示例</span><span class="sxs-lookup"><span data-stu-id="a1a50-172">Example</span></span>

### <a name="request"></a><span data-ttu-id="a1a50-173">请求</span><span class="sxs-lookup"><span data-stu-id="a1a50-173">Request</span></span>
<span data-ttu-id="a1a50-174">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1a50-174">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 311

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```

### <a name="response"></a><span data-ttu-id="a1a50-175">响应</span><span class="sxs-lookup"><span data-stu-id="a1a50-175">Response</span></span>
<span data-ttu-id="a1a50-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1a50-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 483

{
  "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
  "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "licenseType": "licenseFile",
  "targetEdition": "windows10EnterpriseN",
  "license": "License value",
  "productKey": "Product Key value"
}
```









