---
title: 更新 macOSGeneralDeviceConfiguration
description: 更新 macOSGeneralDeviceConfiguration 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 304e3c46ee496e9745ada16907281ed935f42e37
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43387785"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="72b94-103">更新 macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="72b94-103">Update macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="72b94-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="72b94-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="72b94-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="72b94-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="72b94-106">更新 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="72b94-106">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="72b94-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="72b94-107">Prerequisites</span></span>
<span data-ttu-id="72b94-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="72b94-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="72b94-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="72b94-110">Permission type</span></span>|<span data-ttu-id="72b94-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="72b94-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="72b94-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="72b94-112">Delegated (work or school account)</span></span>|<span data-ttu-id="72b94-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="72b94-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="72b94-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="72b94-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="72b94-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="72b94-115">Not supported.</span></span>|
|<span data-ttu-id="72b94-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="72b94-116">Application</span></span>|<span data-ttu-id="72b94-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="72b94-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="72b94-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="72b94-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="72b94-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="72b94-119">Request headers</span></span>
|<span data-ttu-id="72b94-120">标头</span><span class="sxs-lookup"><span data-stu-id="72b94-120">Header</span></span>|<span data-ttu-id="72b94-121">值</span><span class="sxs-lookup"><span data-stu-id="72b94-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="72b94-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="72b94-122">Authorization</span></span>|<span data-ttu-id="72b94-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="72b94-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="72b94-124">接受</span><span class="sxs-lookup"><span data-stu-id="72b94-124">Accept</span></span>|<span data-ttu-id="72b94-125">application/json</span><span class="sxs-lookup"><span data-stu-id="72b94-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="72b94-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="72b94-126">Request body</span></span>
<span data-ttu-id="72b94-127">在请求正文中，提供 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="72b94-127">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="72b94-128">下表显示创建 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="72b94-128">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="72b94-129">属性</span><span class="sxs-lookup"><span data-stu-id="72b94-129">Property</span></span>|<span data-ttu-id="72b94-130">类型</span><span class="sxs-lookup"><span data-stu-id="72b94-130">Type</span></span>|<span data-ttu-id="72b94-131">说明</span><span class="sxs-lookup"><span data-stu-id="72b94-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="72b94-132">id</span><span class="sxs-lookup"><span data-stu-id="72b94-132">id</span></span>|<span data-ttu-id="72b94-133">字符串</span><span class="sxs-lookup"><span data-stu-id="72b94-133">String</span></span>|<span data-ttu-id="72b94-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="72b94-134">Key of the entity.</span></span> <span data-ttu-id="72b94-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72b94-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72b94-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="72b94-136">lastModifiedDateTime</span></span>|<span data-ttu-id="72b94-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72b94-137">DateTimeOffset</span></span>|<span data-ttu-id="72b94-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="72b94-138">DateTime the object was last modified.</span></span> <span data-ttu-id="72b94-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72b94-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72b94-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="72b94-140">createdDateTime</span></span>|<span data-ttu-id="72b94-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="72b94-141">DateTimeOffset</span></span>|<span data-ttu-id="72b94-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="72b94-142">DateTime the object was created.</span></span> <span data-ttu-id="72b94-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72b94-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72b94-144">description</span><span class="sxs-lookup"><span data-stu-id="72b94-144">description</span></span>|<span data-ttu-id="72b94-145">String</span><span class="sxs-lookup"><span data-stu-id="72b94-145">String</span></span>|<span data-ttu-id="72b94-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="72b94-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="72b94-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72b94-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72b94-148">displayName</span><span class="sxs-lookup"><span data-stu-id="72b94-148">displayName</span></span>|<span data-ttu-id="72b94-149">String</span><span class="sxs-lookup"><span data-stu-id="72b94-149">String</span></span>|<span data-ttu-id="72b94-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="72b94-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="72b94-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72b94-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72b94-152">version</span><span class="sxs-lookup"><span data-stu-id="72b94-152">version</span></span>|<span data-ttu-id="72b94-153">Int32</span><span class="sxs-lookup"><span data-stu-id="72b94-153">Int32</span></span>|<span data-ttu-id="72b94-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="72b94-154">Version of the device configuration.</span></span> <span data-ttu-id="72b94-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="72b94-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="72b94-156">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="72b94-156">compliantAppsList</span></span>|<span data-ttu-id="72b94-157">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="72b94-157">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="72b94-158">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="72b94-158">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="72b94-159">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="72b94-159">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="72b94-160">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="72b94-160">compliantAppListType</span></span>|[<span data-ttu-id="72b94-161">appListType</span><span class="sxs-lookup"><span data-stu-id="72b94-161">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="72b94-162">位于 CompliantAppsList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="72b94-162">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="72b94-163">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="72b94-163">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="72b94-164">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="72b94-164">emailInDomainSuffixes</span></span>|<span data-ttu-id="72b94-165">String 集合</span><span class="sxs-lookup"><span data-stu-id="72b94-165">String collection</span></span>|<span data-ttu-id="72b94-166">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="72b94-166">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="72b94-167">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="72b94-167">passwordBlockSimple</span></span>|<span data-ttu-id="72b94-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="72b94-168">Boolean</span></span>|<span data-ttu-id="72b94-169">阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="72b94-169">Block simple passwords.</span></span>|
|<span data-ttu-id="72b94-170">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="72b94-170">passwordExpirationDays</span></span>|<span data-ttu-id="72b94-171">Int32</span><span class="sxs-lookup"><span data-stu-id="72b94-171">Int32</span></span>|<span data-ttu-id="72b94-172">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="72b94-172">Number of days before the password expires.</span></span>|
|<span data-ttu-id="72b94-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="72b94-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="72b94-174">Int32</span><span class="sxs-lookup"><span data-stu-id="72b94-174">Int32</span></span>|<span data-ttu-id="72b94-175">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="72b94-175">Number of character sets a password must contain.</span></span> <span data-ttu-id="72b94-176">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="72b94-176">Valid values 0 to 4</span></span>|
|<span data-ttu-id="72b94-177">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="72b94-177">passwordMinimumLength</span></span>|<span data-ttu-id="72b94-178">Int32</span><span class="sxs-lookup"><span data-stu-id="72b94-178">Int32</span></span>|<span data-ttu-id="72b94-179">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="72b94-179">Minimum length of passwords.</span></span>|
|<span data-ttu-id="72b94-180">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="72b94-180">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="72b94-181">Int32</span><span class="sxs-lookup"><span data-stu-id="72b94-181">Int32</span></span>|<span data-ttu-id="72b94-182">在需要密码之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="72b94-182">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="72b94-183">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="72b94-183">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="72b94-184">Int32</span><span class="sxs-lookup"><span data-stu-id="72b94-184">Int32</span></span>|<span data-ttu-id="72b94-185">在屏幕超时之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="72b94-185">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="72b94-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="72b94-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="72b94-187">Int32</span><span class="sxs-lookup"><span data-stu-id="72b94-187">Int32</span></span>|<span data-ttu-id="72b94-188">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="72b94-188">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="72b94-189">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="72b94-189">passwordRequiredType</span></span>|[<span data-ttu-id="72b94-190">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="72b94-190">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="72b94-191">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="72b94-191">Type of password that is required.</span></span> <span data-ttu-id="72b94-192">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="72b94-192">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="72b94-193">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="72b94-193">passwordRequired</span></span>|<span data-ttu-id="72b94-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="72b94-194">Boolean</span></span>|<span data-ttu-id="72b94-195">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="72b94-195">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="72b94-196">响应</span><span class="sxs-lookup"><span data-stu-id="72b94-196">Response</span></span>
<span data-ttu-id="72b94-197">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="72b94-197">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="72b94-198">示例</span><span class="sxs-lookup"><span data-stu-id="72b94-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="72b94-199">请求</span><span class="sxs-lookup"><span data-stu-id="72b94-199">Request</span></span>
<span data-ttu-id="72b94-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="72b94-200">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
Content-type: application/json
Content-length: 906

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```

### <a name="response"></a><span data-ttu-id="72b94-201">响应</span><span class="sxs-lookup"><span data-stu-id="72b94-201">Response</span></span>
<span data-ttu-id="72b94-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="72b94-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1078

{
  "@odata.type": "#microsoft.graph.macOSGeneralDeviceConfiguration",
  "id": "dc356aee-6aee-dc35-ee6a-35dcee6a35dc",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "description": "Description value",
  "displayName": "Display Name value",
  "version": 7,
  "compliantAppsList": [
    {
      "@odata.type": "microsoft.graph.appListItem",
      "name": "Name value",
      "publisher": "Publisher value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "appId": "App Id value"
    }
  ],
  "compliantAppListType": "appsInListCompliant",
  "emailInDomainSuffixes": [
    "Email In Domain Suffixes value"
  ],
  "passwordBlockSimple": true,
  "passwordExpirationDays": 6,
  "passwordMinimumCharacterSetCount": 0,
  "passwordMinimumLength": 5,
  "passwordMinutesOfInactivityBeforeLock": 5,
  "passwordMinutesOfInactivityBeforeScreenTimeout": 14,
  "passwordPreviousPasswordBlockCount": 2,
  "passwordRequiredType": "alphanumeric",
  "passwordRequired": true
}
```






