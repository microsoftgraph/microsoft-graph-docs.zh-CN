---
title: 创建 editionUpgradeConfiguration
description: 创建新的 editionUpgradeConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 18349354e899b85cfb34975e899333c679c15c08
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32578895"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="7f1c0-103">创建 editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="7f1c0-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="7f1c0-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7f1c0-105">创建新的 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-105">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7f1c0-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="7f1c0-106">Prerequisites</span></span>
<span data-ttu-id="7f1c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7f1c0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7f1c0-109">Permission type</span></span>|<span data-ttu-id="7f1c0-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7f1c0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7f1c0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7f1c0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7f1c0-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7f1c0-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7f1c0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7f1c0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7f1c0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-114">Not supported.</span></span>|
|<span data-ttu-id="7f1c0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7f1c0-115">Application</span></span>|<span data-ttu-id="7f1c0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7f1c0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7f1c0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7f1c0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7f1c0-118">Request headers</span></span>
|<span data-ttu-id="7f1c0-119">标头</span><span class="sxs-lookup"><span data-stu-id="7f1c0-119">Header</span></span>|<span data-ttu-id="7f1c0-120">值</span><span class="sxs-lookup"><span data-stu-id="7f1c0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7f1c0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7f1c0-121">Authorization</span></span>|<span data-ttu-id="7f1c0-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7f1c0-123">接受</span><span class="sxs-lookup"><span data-stu-id="7f1c0-123">Accept</span></span>|<span data-ttu-id="7f1c0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7f1c0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7f1c0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7f1c0-125">Request body</span></span>
<span data-ttu-id="7f1c0-126">在请求正文中，提供 editionUpgradeConfiguration对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-126">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="7f1c0-127">下表显示创建 editionUpgradeConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-127">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="7f1c0-128">属性</span><span class="sxs-lookup"><span data-stu-id="7f1c0-128">Property</span></span>|<span data-ttu-id="7f1c0-129">类型</span><span class="sxs-lookup"><span data-stu-id="7f1c0-129">Type</span></span>|<span data-ttu-id="7f1c0-130">说明</span><span class="sxs-lookup"><span data-stu-id="7f1c0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7f1c0-131">id</span><span class="sxs-lookup"><span data-stu-id="7f1c0-131">id</span></span>|<span data-ttu-id="7f1c0-132">字符串</span><span class="sxs-lookup"><span data-stu-id="7f1c0-132">String</span></span>|<span data-ttu-id="7f1c0-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-133">Key of the entity.</span></span> <span data-ttu-id="7f1c0-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f1c0-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f1c0-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7f1c0-135">lastModifiedDateTime</span></span>|<span data-ttu-id="7f1c0-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f1c0-136">DateTimeOffset</span></span>|<span data-ttu-id="7f1c0-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-137">DateTime the object was last modified.</span></span> <span data-ttu-id="7f1c0-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f1c0-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f1c0-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7f1c0-139">createdDateTime</span></span>|<span data-ttu-id="7f1c0-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7f1c0-140">DateTimeOffset</span></span>|<span data-ttu-id="7f1c0-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-141">DateTime the object was created.</span></span> <span data-ttu-id="7f1c0-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f1c0-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f1c0-143">说明</span><span class="sxs-lookup"><span data-stu-id="7f1c0-143">description</span></span>|<span data-ttu-id="7f1c0-144">String</span><span class="sxs-lookup"><span data-stu-id="7f1c0-144">String</span></span>|<span data-ttu-id="7f1c0-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7f1c0-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f1c0-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f1c0-147">displayName</span><span class="sxs-lookup"><span data-stu-id="7f1c0-147">displayName</span></span>|<span data-ttu-id="7f1c0-148">String</span><span class="sxs-lookup"><span data-stu-id="7f1c0-148">String</span></span>|<span data-ttu-id="7f1c0-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7f1c0-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f1c0-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f1c0-151">version</span><span class="sxs-lookup"><span data-stu-id="7f1c0-151">version</span></span>|<span data-ttu-id="7f1c0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7f1c0-152">Int32</span></span>|<span data-ttu-id="7f1c0-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-153">Version of the device configuration.</span></span> <span data-ttu-id="7f1c0-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7f1c0-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7f1c0-155">licenseType</span><span class="sxs-lookup"><span data-stu-id="7f1c0-155">licenseType</span></span>|[<span data-ttu-id="7f1c0-156">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="7f1c0-156">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="7f1c0-157">版本升级许可证类型。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-157">Edition Upgrade License Type.</span></span> <span data-ttu-id="7f1c0-158">可取值为：`productKey`、`licenseFile`。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-158">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="7f1c0-159">targetEdition</span><span class="sxs-lookup"><span data-stu-id="7f1c0-159">targetEdition</span></span>|[<span data-ttu-id="7f1c0-160">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="7f1c0-160">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="7f1c0-161">版本升级目标版本。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-161">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="7f1c0-162">可取值为：`windows10Enterprise`、`windows10EnterpriseN`、`windows10Education`、`windows10EducationN`、`windows10MobileEnterprise`、`windows10HolographicEnterprise`、`windows10Professional`、`windows10ProfessionalN`、`windows10ProfessionalEducation`、`windows10ProfessionalEducationN`、`windows10ProfessionalWorkstation`、`windows10ProfessionalWorkstationN`。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-162">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="7f1c0-163">license</span><span class="sxs-lookup"><span data-stu-id="7f1c0-163">license</span></span>|<span data-ttu-id="7f1c0-164">String</span><span class="sxs-lookup"><span data-stu-id="7f1c0-164">String</span></span>|<span data-ttu-id="7f1c0-165">版本升级许可证文件内容。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-165">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="7f1c0-166">productKey</span><span class="sxs-lookup"><span data-stu-id="7f1c0-166">productKey</span></span>|<span data-ttu-id="7f1c0-167">String</span><span class="sxs-lookup"><span data-stu-id="7f1c0-167">String</span></span>|<span data-ttu-id="7f1c0-168">版本升级产品密钥。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-168">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="7f1c0-169">响应</span><span class="sxs-lookup"><span data-stu-id="7f1c0-169">Response</span></span>
<span data-ttu-id="7f1c0-170">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-170">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7f1c0-171">示例</span><span class="sxs-lookup"><span data-stu-id="7f1c0-171">Example</span></span>

### <a name="request"></a><span data-ttu-id="7f1c0-172">请求</span><span class="sxs-lookup"><span data-stu-id="7f1c0-172">Request</span></span>
<span data-ttu-id="7f1c0-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-173">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="7f1c0-174">响应</span><span class="sxs-lookup"><span data-stu-id="7f1c0-174">Response</span></span>
<span data-ttu-id="7f1c0-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7f1c0-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



