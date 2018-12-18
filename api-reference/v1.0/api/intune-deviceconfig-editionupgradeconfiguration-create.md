---
title: 创建 editionUpgradeConfiguration
description: 创建新的 editionUpgradeConfiguration 对象。
author: tfitzmac
ms.openlocfilehash: 9ea7bb6206b882f81cad3cfd62419dc887f04898
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27332737"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="ddfeb-103">创建 editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="ddfeb-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="ddfeb-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ddfeb-105">创建新的 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-105">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ddfeb-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="ddfeb-106">Prerequisites</span></span>
<span data-ttu-id="ddfeb-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ddfeb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddfeb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ddfeb-109">Permission type</span></span>|<span data-ttu-id="ddfeb-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ddfeb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ddfeb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ddfeb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="ddfeb-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ddfeb-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ddfeb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ddfeb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ddfeb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-114">Not supported.</span></span>|
|<span data-ttu-id="ddfeb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ddfeb-115">Application</span></span>|<span data-ttu-id="ddfeb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ddfeb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ddfeb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="ddfeb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ddfeb-118">Request headers</span></span>
|<span data-ttu-id="ddfeb-119">标头</span><span class="sxs-lookup"><span data-stu-id="ddfeb-119">Header</span></span>|<span data-ttu-id="ddfeb-120">值</span><span class="sxs-lookup"><span data-stu-id="ddfeb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ddfeb-121">授权</span><span class="sxs-lookup"><span data-stu-id="ddfeb-121">Authorization</span></span>|<span data-ttu-id="ddfeb-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ddfeb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="ddfeb-123">Accept</span></span>|<span data-ttu-id="ddfeb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="ddfeb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ddfeb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="ddfeb-125">Request body</span></span>
<span data-ttu-id="ddfeb-126">在请求正文中，提供 editionUpgradeConfiguration对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-126">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="ddfeb-127">下表显示创建 editionUpgradeConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-127">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="ddfeb-128">属性</span><span class="sxs-lookup"><span data-stu-id="ddfeb-128">Property</span></span>|<span data-ttu-id="ddfeb-129">类型</span><span class="sxs-lookup"><span data-stu-id="ddfeb-129">Type</span></span>|<span data-ttu-id="ddfeb-130">说明</span><span class="sxs-lookup"><span data-stu-id="ddfeb-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ddfeb-131">id</span><span class="sxs-lookup"><span data-stu-id="ddfeb-131">id</span></span>|<span data-ttu-id="ddfeb-132">String</span><span class="sxs-lookup"><span data-stu-id="ddfeb-132">String</span></span>|<span data-ttu-id="ddfeb-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-133">Key of the entity.</span></span> <span data-ttu-id="ddfeb-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddfeb-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddfeb-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="ddfeb-135">lastModifiedDateTime</span></span>|<span data-ttu-id="ddfeb-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddfeb-136">DateTimeOffset</span></span>|<span data-ttu-id="ddfeb-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-137">DateTime the object was last modified.</span></span> <span data-ttu-id="ddfeb-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddfeb-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddfeb-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="ddfeb-139">createdDateTime</span></span>|<span data-ttu-id="ddfeb-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ddfeb-140">DateTimeOffset</span></span>|<span data-ttu-id="ddfeb-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-141">DateTime the object was created.</span></span> <span data-ttu-id="ddfeb-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddfeb-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddfeb-143">description</span><span class="sxs-lookup"><span data-stu-id="ddfeb-143">description</span></span>|<span data-ttu-id="ddfeb-144">String</span><span class="sxs-lookup"><span data-stu-id="ddfeb-144">String</span></span>|<span data-ttu-id="ddfeb-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="ddfeb-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddfeb-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddfeb-147">displayName</span><span class="sxs-lookup"><span data-stu-id="ddfeb-147">displayName</span></span>|<span data-ttu-id="ddfeb-148">String</span><span class="sxs-lookup"><span data-stu-id="ddfeb-148">String</span></span>|<span data-ttu-id="ddfeb-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="ddfeb-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddfeb-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddfeb-151">version</span><span class="sxs-lookup"><span data-stu-id="ddfeb-151">version</span></span>|<span data-ttu-id="ddfeb-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ddfeb-152">Int32</span></span>|<span data-ttu-id="ddfeb-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-153">Version of the device configuration.</span></span> <span data-ttu-id="ddfeb-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="ddfeb-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="ddfeb-155">licenseType</span><span class="sxs-lookup"><span data-stu-id="ddfeb-155">licenseType</span></span>|[<span data-ttu-id="ddfeb-156">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="ddfeb-156">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="ddfeb-157">版本升级许可证类型。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-157">Edition Upgrade License Type.</span></span> <span data-ttu-id="ddfeb-158">可取值为：`productKey`、`licenseFile`。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-158">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="ddfeb-159">targetEdition</span><span class="sxs-lookup"><span data-stu-id="ddfeb-159">targetEdition</span></span>|[<span data-ttu-id="ddfeb-160">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="ddfeb-160">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="ddfeb-161">版本升级目标版本。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-161">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="ddfeb-162">可取值为：`windows10Enterprise`、`windows10EnterpriseN`、`windows10Education`、`windows10EducationN`、`windows10MobileEnterprise`、`windows10HolographicEnterprise`、`windows10Professional`、`windows10ProfessionalN`、`windows10ProfessionalEducation`、`windows10ProfessionalEducationN`、`windows10ProfessionalWorkstation`、`windows10ProfessionalWorkstationN`。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-162">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="ddfeb-163">license</span><span class="sxs-lookup"><span data-stu-id="ddfeb-163">license</span></span>|<span data-ttu-id="ddfeb-164">String</span><span class="sxs-lookup"><span data-stu-id="ddfeb-164">String</span></span>|<span data-ttu-id="ddfeb-165">版本升级许可证文件内容。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-165">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="ddfeb-166">productKey</span><span class="sxs-lookup"><span data-stu-id="ddfeb-166">productKey</span></span>|<span data-ttu-id="ddfeb-167">String</span><span class="sxs-lookup"><span data-stu-id="ddfeb-167">String</span></span>|<span data-ttu-id="ddfeb-168">版本升级产品密钥。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-168">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="ddfeb-169">响应</span><span class="sxs-lookup"><span data-stu-id="ddfeb-169">Response</span></span>
<span data-ttu-id="ddfeb-170">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-170">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ddfeb-171">示例</span><span class="sxs-lookup"><span data-stu-id="ddfeb-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="ddfeb-172">请求</span><span class="sxs-lookup"><span data-stu-id="ddfeb-172">Request</span></span>
<span data-ttu-id="ddfeb-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ddfeb-174">响应</span><span class="sxs-lookup"><span data-stu-id="ddfeb-174">Response</span></span>
<span data-ttu-id="ddfeb-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ddfeb-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



