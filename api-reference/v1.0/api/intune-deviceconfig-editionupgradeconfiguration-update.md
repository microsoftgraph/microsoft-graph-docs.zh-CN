---
title: 更新 editionUpgradeConfiguration
description: 更新 editionUpgradeConfiguration 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a1e438153d6ecf75e49b33e638149dc4d7196d4d
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37368454"
---
# <a name="update-editionupgradeconfiguration"></a><span data-ttu-id="82290-103">更新 editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="82290-103">Update editionUpgradeConfiguration</span></span>

> <span data-ttu-id="82290-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="82290-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="82290-105">更新 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="82290-105">Update the properties of a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="82290-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="82290-106">Prerequisites</span></span>
<span data-ttu-id="82290-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="82290-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="82290-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="82290-109">Permission type</span></span>|<span data-ttu-id="82290-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="82290-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="82290-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="82290-111">Delegated (work or school account)</span></span>|<span data-ttu-id="82290-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="82290-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="82290-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="82290-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="82290-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="82290-114">Not supported.</span></span>|
|<span data-ttu-id="82290-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="82290-115">Application</span></span>|<span data-ttu-id="82290-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="82290-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="82290-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="82290-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="82290-118">请求头</span><span class="sxs-lookup"><span data-stu-id="82290-118">Request headers</span></span>
|<span data-ttu-id="82290-119">标头</span><span class="sxs-lookup"><span data-stu-id="82290-119">Header</span></span>|<span data-ttu-id="82290-120">值</span><span class="sxs-lookup"><span data-stu-id="82290-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="82290-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="82290-121">Authorization</span></span>|<span data-ttu-id="82290-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="82290-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="82290-123">接受</span><span class="sxs-lookup"><span data-stu-id="82290-123">Accept</span></span>|<span data-ttu-id="82290-124">application/json</span><span class="sxs-lookup"><span data-stu-id="82290-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="82290-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="82290-125">Request body</span></span>
<span data-ttu-id="82290-126">在请求正文中，提供 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="82290-126">In the request body, supply a JSON representation for the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

<span data-ttu-id="82290-127">下表显示创建 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="82290-127">The following table shows the properties that are required when you create the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md).</span></span>

|<span data-ttu-id="82290-128">属性</span><span class="sxs-lookup"><span data-stu-id="82290-128">Property</span></span>|<span data-ttu-id="82290-129">类型</span><span class="sxs-lookup"><span data-stu-id="82290-129">Type</span></span>|<span data-ttu-id="82290-130">说明</span><span class="sxs-lookup"><span data-stu-id="82290-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="82290-131">id</span><span class="sxs-lookup"><span data-stu-id="82290-131">id</span></span>|<span data-ttu-id="82290-132">字符串</span><span class="sxs-lookup"><span data-stu-id="82290-132">String</span></span>|<span data-ttu-id="82290-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="82290-133">Key of the entity.</span></span> <span data-ttu-id="82290-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82290-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82290-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="82290-135">lastModifiedDateTime</span></span>|<span data-ttu-id="82290-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82290-136">DateTimeOffset</span></span>|<span data-ttu-id="82290-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="82290-137">DateTime the object was last modified.</span></span> <span data-ttu-id="82290-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82290-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82290-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="82290-139">createdDateTime</span></span>|<span data-ttu-id="82290-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="82290-140">DateTimeOffset</span></span>|<span data-ttu-id="82290-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="82290-141">DateTime the object was created.</span></span> <span data-ttu-id="82290-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82290-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82290-143">说明</span><span class="sxs-lookup"><span data-stu-id="82290-143">description</span></span>|<span data-ttu-id="82290-144">String</span><span class="sxs-lookup"><span data-stu-id="82290-144">String</span></span>|<span data-ttu-id="82290-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="82290-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="82290-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82290-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82290-147">displayName</span><span class="sxs-lookup"><span data-stu-id="82290-147">displayName</span></span>|<span data-ttu-id="82290-148">String</span><span class="sxs-lookup"><span data-stu-id="82290-148">String</span></span>|<span data-ttu-id="82290-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="82290-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="82290-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82290-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82290-151">version</span><span class="sxs-lookup"><span data-stu-id="82290-151">version</span></span>|<span data-ttu-id="82290-152">Int32</span><span class="sxs-lookup"><span data-stu-id="82290-152">Int32</span></span>|<span data-ttu-id="82290-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="82290-153">Version of the device configuration.</span></span> <span data-ttu-id="82290-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="82290-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="82290-155">licenseType</span><span class="sxs-lookup"><span data-stu-id="82290-155">licenseType</span></span>|[<span data-ttu-id="82290-156">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="82290-156">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="82290-157">版本升级许可证类型。</span><span class="sxs-lookup"><span data-stu-id="82290-157">Edition Upgrade License Type.</span></span> <span data-ttu-id="82290-158">可取值为：`productKey`、`licenseFile`。</span><span class="sxs-lookup"><span data-stu-id="82290-158">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="82290-159">targetEdition</span><span class="sxs-lookup"><span data-stu-id="82290-159">targetEdition</span></span>|[<span data-ttu-id="82290-160">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="82290-160">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="82290-161">版本升级目标版本。</span><span class="sxs-lookup"><span data-stu-id="82290-161">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="82290-162">可取值为：`windows10Enterprise`、`windows10EnterpriseN`、`windows10Education`、`windows10EducationN`、`windows10MobileEnterprise`、`windows10HolographicEnterprise`、`windows10Professional`、`windows10ProfessionalN`、`windows10ProfessionalEducation`、`windows10ProfessionalEducationN`、`windows10ProfessionalWorkstation`、`windows10ProfessionalWorkstationN`。</span><span class="sxs-lookup"><span data-stu-id="82290-162">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="82290-163">license</span><span class="sxs-lookup"><span data-stu-id="82290-163">license</span></span>|<span data-ttu-id="82290-164">String</span><span class="sxs-lookup"><span data-stu-id="82290-164">String</span></span>|<span data-ttu-id="82290-165">版本升级许可证文件内容。</span><span class="sxs-lookup"><span data-stu-id="82290-165">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="82290-166">productKey</span><span class="sxs-lookup"><span data-stu-id="82290-166">productKey</span></span>|<span data-ttu-id="82290-167">String</span><span class="sxs-lookup"><span data-stu-id="82290-167">String</span></span>|<span data-ttu-id="82290-168">版本升级产品密钥。</span><span class="sxs-lookup"><span data-stu-id="82290-168">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="82290-169">响应</span><span class="sxs-lookup"><span data-stu-id="82290-169">Response</span></span>
<span data-ttu-id="82290-170">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="82290-170">If successful, this method returns a `200 OK` response code and an updated [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="82290-171">示例</span><span class="sxs-lookup"><span data-stu-id="82290-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="82290-172">请求</span><span class="sxs-lookup"><span data-stu-id="82290-172">Request</span></span>
<span data-ttu-id="82290-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="82290-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="82290-174">响应</span><span class="sxs-lookup"><span data-stu-id="82290-174">Response</span></span>
<span data-ttu-id="82290-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="82290-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




