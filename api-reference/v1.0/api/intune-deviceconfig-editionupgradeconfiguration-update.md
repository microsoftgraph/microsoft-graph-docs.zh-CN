---
title: 更新 editionUpgradeConfiguration
description: 更新 editionUpgradeConfiguration 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a02bc5dae2d65101492f24fab577a9d242733334
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30250178"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="6b476-103">更新 editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="6b476-103">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="6b476-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6b476-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6b476-105">更新 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6b476-105">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6b476-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="6b476-106">Prerequisites</span></span>
<span data-ttu-id="6b476-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6b476-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="6b476-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b476-109">Permission type</span></span>|<span data-ttu-id="6b476-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6b476-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6b476-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b476-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6b476-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6b476-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6b476-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b476-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6b476-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b476-114">Not supported.</span></span>|
|<span data-ttu-id="6b476-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b476-115">Application</span></span>|<span data-ttu-id="6b476-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b476-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6b476-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b476-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6b476-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6b476-118">Request headers</span></span>
|<span data-ttu-id="6b476-119">标头</span><span class="sxs-lookup"><span data-stu-id="6b476-119">Header</span></span>|<span data-ttu-id="6b476-120">值</span><span class="sxs-lookup"><span data-stu-id="6b476-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6b476-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6b476-121">Authorization</span></span>|<span data-ttu-id="6b476-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6b476-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6b476-123">Accept</span><span class="sxs-lookup"><span data-stu-id="6b476-123">Accept</span></span>|<span data-ttu-id="6b476-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6b476-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6b476-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b476-125">Request body</span></span>
<span data-ttu-id="6b476-126">在请求正文中，提供 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b476-126">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="6b476-127">下表显示创建 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6b476-127">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="6b476-128">属性</span><span class="sxs-lookup"><span data-stu-id="6b476-128">Property</span></span>|<span data-ttu-id="6b476-129">类型</span><span class="sxs-lookup"><span data-stu-id="6b476-129">Type</span></span>|<span data-ttu-id="6b476-130">说明</span><span class="sxs-lookup"><span data-stu-id="6b476-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6b476-131">id</span><span class="sxs-lookup"><span data-stu-id="6b476-131">id</span></span>|<span data-ttu-id="6b476-132">字符串</span><span class="sxs-lookup"><span data-stu-id="6b476-132">String</span></span>|<span data-ttu-id="6b476-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6b476-133">Key of the entity.</span></span> <span data-ttu-id="6b476-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b476-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b476-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6b476-135">lastModifiedDateTime</span></span>|<span data-ttu-id="6b476-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b476-136">DateTimeOffset</span></span>|<span data-ttu-id="6b476-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6b476-137">DateTime the object was last modified.</span></span> <span data-ttu-id="6b476-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b476-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b476-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6b476-139">createdDateTime</span></span>|<span data-ttu-id="6b476-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6b476-140">DateTimeOffset</span></span>|<span data-ttu-id="6b476-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="6b476-141">DateTime the object was created.</span></span> <span data-ttu-id="6b476-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b476-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b476-143">description</span><span class="sxs-lookup"><span data-stu-id="6b476-143">description</span></span>|<span data-ttu-id="6b476-144">字符串</span><span class="sxs-lookup"><span data-stu-id="6b476-144">String</span></span>|<span data-ttu-id="6b476-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="6b476-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="6b476-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b476-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b476-147">displayName</span><span class="sxs-lookup"><span data-stu-id="6b476-147">displayName</span></span>|<span data-ttu-id="6b476-148">String</span><span class="sxs-lookup"><span data-stu-id="6b476-148">String</span></span>|<span data-ttu-id="6b476-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="6b476-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="6b476-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b476-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b476-151">version</span><span class="sxs-lookup"><span data-stu-id="6b476-151">version</span></span>|<span data-ttu-id="6b476-152">Int32</span><span class="sxs-lookup"><span data-stu-id="6b476-152">Int32</span></span>|<span data-ttu-id="6b476-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="6b476-153">Version of the device configuration.</span></span> <span data-ttu-id="6b476-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="6b476-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="6b476-155">licenseType</span><span class="sxs-lookup"><span data-stu-id="6b476-155">licenseType</span></span>|[<span data-ttu-id="6b476-156">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="6b476-156">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="6b476-157">版本升级许可证类型。</span><span class="sxs-lookup"><span data-stu-id="6b476-157">Edition Upgrade License Type.</span></span> <span data-ttu-id="6b476-158">可取值为：`productKey`、`licenseFile`。</span><span class="sxs-lookup"><span data-stu-id="6b476-158">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="6b476-159">targetEdition</span><span class="sxs-lookup"><span data-stu-id="6b476-159">targetEdition</span></span>|[<span data-ttu-id="6b476-160">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="6b476-160">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="6b476-161">版本升级目标版本。</span><span class="sxs-lookup"><span data-stu-id="6b476-161">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="6b476-162">可取值为：`windows10Enterprise`、`windows10EnterpriseN`、`windows10Education`、`windows10EducationN`、`windows10MobileEnterprise`、`windows10HolographicEnterprise`、`windows10Professional`、`windows10ProfessionalN`、`windows10ProfessionalEducation`、`windows10ProfessionalEducationN`、`windows10ProfessionalWorkstation`、`windows10ProfessionalWorkstationN`。</span><span class="sxs-lookup"><span data-stu-id="6b476-162">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="6b476-163">license</span><span class="sxs-lookup"><span data-stu-id="6b476-163">license</span></span>|<span data-ttu-id="6b476-164">String</span><span class="sxs-lookup"><span data-stu-id="6b476-164">String</span></span>|<span data-ttu-id="6b476-165">版本升级许可证文件内容。</span><span class="sxs-lookup"><span data-stu-id="6b476-165">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="6b476-166">productKey</span><span class="sxs-lookup"><span data-stu-id="6b476-166">productKey</span></span>|<span data-ttu-id="6b476-167">String</span><span class="sxs-lookup"><span data-stu-id="6b476-167">String</span></span>|<span data-ttu-id="6b476-168">版本升级产品密钥。</span><span class="sxs-lookup"><span data-stu-id="6b476-168">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="6b476-169">响应</span><span class="sxs-lookup"><span data-stu-id="6b476-169">Response</span></span>
<span data-ttu-id="6b476-170">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6b476-170">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b476-171">示例</span><span class="sxs-lookup"><span data-stu-id="6b476-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b476-172">请求</span><span class="sxs-lookup"><span data-stu-id="6b476-172">Request</span></span>
<span data-ttu-id="6b476-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6b476-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6b476-174">响应</span><span class="sxs-lookup"><span data-stu-id="6b476-174">Response</span></span>
<span data-ttu-id="6b476-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6b476-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



