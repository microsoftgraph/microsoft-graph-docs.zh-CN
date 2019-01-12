---
title: 创建 editionUpgradeConfiguration
description: 创建新的 editionUpgradeConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: c32873ffe50a4a35f94324d782e055508389e7e4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27937920"
---
# <a name="create-editionupgradeconfiguration"></a><span data-ttu-id="7dd73-103">创建 editionUpgradeConfiguration</span><span class="sxs-lookup"><span data-stu-id="7dd73-103">Create editionUpgradeConfiguration</span></span>

> <span data-ttu-id="7dd73-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="7dd73-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7dd73-105">创建新的 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7dd73-105">Create a new [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7dd73-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="7dd73-106">Prerequisites</span></span>
<span data-ttu-id="7dd73-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="7dd73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7dd73-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7dd73-109">Permission type</span></span>|<span data-ttu-id="7dd73-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7dd73-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7dd73-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7dd73-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7dd73-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7dd73-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="7dd73-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7dd73-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7dd73-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7dd73-114">Not supported.</span></span>|
|<span data-ttu-id="7dd73-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7dd73-115">Application</span></span>|<span data-ttu-id="7dd73-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7dd73-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7dd73-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7dd73-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7dd73-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7dd73-118">Request headers</span></span>
|<span data-ttu-id="7dd73-119">标头</span><span class="sxs-lookup"><span data-stu-id="7dd73-119">Header</span></span>|<span data-ttu-id="7dd73-120">值</span><span class="sxs-lookup"><span data-stu-id="7dd73-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7dd73-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7dd73-121">Authorization</span></span>|<span data-ttu-id="7dd73-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7dd73-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7dd73-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7dd73-123">Accept</span></span>|<span data-ttu-id="7dd73-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7dd73-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7dd73-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7dd73-125">Request body</span></span>
<span data-ttu-id="7dd73-126">在请求正文中，提供 editionUpgradeConfiguration对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7dd73-126">In the request body, supply a JSON representation for the editionUpgradeConfiguration object.</span></span>

<span data-ttu-id="7dd73-127">下表显示创建 editionUpgradeConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7dd73-127">The following table shows the properties that are required when you create the editionUpgradeConfiguration.</span></span>

|<span data-ttu-id="7dd73-128">属性</span><span class="sxs-lookup"><span data-stu-id="7dd73-128">Property</span></span>|<span data-ttu-id="7dd73-129">类型</span><span class="sxs-lookup"><span data-stu-id="7dd73-129">Type</span></span>|<span data-ttu-id="7dd73-130">说明</span><span class="sxs-lookup"><span data-stu-id="7dd73-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7dd73-131">id</span><span class="sxs-lookup"><span data-stu-id="7dd73-131">id</span></span>|<span data-ttu-id="7dd73-132">String</span><span class="sxs-lookup"><span data-stu-id="7dd73-132">String</span></span>|<span data-ttu-id="7dd73-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7dd73-133">Key of the entity.</span></span> <span data-ttu-id="7dd73-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dd73-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dd73-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="7dd73-135">lastModifiedDateTime</span></span>|<span data-ttu-id="7dd73-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dd73-136">DateTimeOffset</span></span>|<span data-ttu-id="7dd73-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7dd73-137">DateTime the object was last modified.</span></span> <span data-ttu-id="7dd73-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dd73-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dd73-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="7dd73-139">createdDateTime</span></span>|<span data-ttu-id="7dd73-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7dd73-140">DateTimeOffset</span></span>|<span data-ttu-id="7dd73-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="7dd73-141">DateTime the object was created.</span></span> <span data-ttu-id="7dd73-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dd73-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dd73-143">description</span><span class="sxs-lookup"><span data-stu-id="7dd73-143">description</span></span>|<span data-ttu-id="7dd73-144">String</span><span class="sxs-lookup"><span data-stu-id="7dd73-144">String</span></span>|<span data-ttu-id="7dd73-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="7dd73-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="7dd73-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dd73-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dd73-147">displayName</span><span class="sxs-lookup"><span data-stu-id="7dd73-147">displayName</span></span>|<span data-ttu-id="7dd73-148">String</span><span class="sxs-lookup"><span data-stu-id="7dd73-148">String</span></span>|<span data-ttu-id="7dd73-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="7dd73-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="7dd73-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dd73-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dd73-151">version</span><span class="sxs-lookup"><span data-stu-id="7dd73-151">version</span></span>|<span data-ttu-id="7dd73-152">Int32</span><span class="sxs-lookup"><span data-stu-id="7dd73-152">Int32</span></span>|<span data-ttu-id="7dd73-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="7dd73-153">Version of the device configuration.</span></span> <span data-ttu-id="7dd73-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="7dd73-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="7dd73-155">licenseType</span><span class="sxs-lookup"><span data-stu-id="7dd73-155">licenseType</span></span>|[<span data-ttu-id="7dd73-156">editionUpgradeLicenseType</span><span class="sxs-lookup"><span data-stu-id="7dd73-156">editionUpgradeLicenseType</span></span>](../resources/intune-deviceconfig-editionupgradelicensetype.md)|<span data-ttu-id="7dd73-157">版本升级许可证类型。</span><span class="sxs-lookup"><span data-stu-id="7dd73-157">Edition Upgrade License Type.</span></span> <span data-ttu-id="7dd73-158">可取值为：`productKey`、`licenseFile`。</span><span class="sxs-lookup"><span data-stu-id="7dd73-158">Possible values are: `productKey`, `licenseFile`.</span></span>|
|<span data-ttu-id="7dd73-159">targetEdition</span><span class="sxs-lookup"><span data-stu-id="7dd73-159">targetEdition</span></span>|[<span data-ttu-id="7dd73-160">windows10EditionType</span><span class="sxs-lookup"><span data-stu-id="7dd73-160">windows10EditionType</span></span>](../resources/intune-deviceconfig-windows10editiontype.md)|<span data-ttu-id="7dd73-161">版本升级目标版本。</span><span class="sxs-lookup"><span data-stu-id="7dd73-161">Edition Upgrade Target Edition.</span></span> <span data-ttu-id="7dd73-162">可取值为：`windows10Enterprise`、`windows10EnterpriseN`、`windows10Education`、`windows10EducationN`、`windows10MobileEnterprise`、`windows10HolographicEnterprise`、`windows10Professional`、`windows10ProfessionalN`、`windows10ProfessionalEducation`、`windows10ProfessionalEducationN`、`windows10ProfessionalWorkstation`、`windows10ProfessionalWorkstationN`。</span><span class="sxs-lookup"><span data-stu-id="7dd73-162">Possible values are: `windows10Enterprise`, `windows10EnterpriseN`, `windows10Education`, `windows10EducationN`, `windows10MobileEnterprise`, `windows10HolographicEnterprise`, `windows10Professional`, `windows10ProfessionalN`, `windows10ProfessionalEducation`, `windows10ProfessionalEducationN`, `windows10ProfessionalWorkstation`, `windows10ProfessionalWorkstationN`.</span></span>|
|<span data-ttu-id="7dd73-163">license</span><span class="sxs-lookup"><span data-stu-id="7dd73-163">license</span></span>|<span data-ttu-id="7dd73-164">String</span><span class="sxs-lookup"><span data-stu-id="7dd73-164">String</span></span>|<span data-ttu-id="7dd73-165">版本升级许可证文件内容。</span><span class="sxs-lookup"><span data-stu-id="7dd73-165">Edition Upgrade License File Content.</span></span>|
|<span data-ttu-id="7dd73-166">productKey</span><span class="sxs-lookup"><span data-stu-id="7dd73-166">productKey</span></span>|<span data-ttu-id="7dd73-167">String</span><span class="sxs-lookup"><span data-stu-id="7dd73-167">String</span></span>|<span data-ttu-id="7dd73-168">版本升级产品密钥。</span><span class="sxs-lookup"><span data-stu-id="7dd73-168">Edition Upgrade Product Key.</span></span>|



## <a name="response"></a><span data-ttu-id="7dd73-169">响应</span><span class="sxs-lookup"><span data-stu-id="7dd73-169">Response</span></span>
<span data-ttu-id="7dd73-170">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7dd73-170">If successful, this method returns a `201 Created` response code and a [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7dd73-171">示例</span><span class="sxs-lookup"><span data-stu-id="7dd73-171">Example</span></span>
### <a name="request"></a><span data-ttu-id="7dd73-172">请求</span><span class="sxs-lookup"><span data-stu-id="7dd73-172">Request</span></span>
<span data-ttu-id="7dd73-173">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7dd73-173">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7dd73-174">响应</span><span class="sxs-lookup"><span data-stu-id="7dd73-174">Response</span></span>
<span data-ttu-id="7dd73-p110">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7dd73-p110">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



