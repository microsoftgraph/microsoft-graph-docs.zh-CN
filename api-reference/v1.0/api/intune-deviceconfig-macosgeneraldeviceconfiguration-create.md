---
title: 创建 macOSGeneralDeviceConfiguration
description: 创建新的 macOSGeneralDeviceConfiguration 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2067ff6847f2419f7aa6885129c64dbeb097290f
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43387853"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="4c9f7-103">创建 macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="4c9f7-103">Create macOSGeneralDeviceConfiguration</span></span>

<span data-ttu-id="4c9f7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4c9f7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4c9f7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c9f7-106">创建新的 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-106">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c9f7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4c9f7-107">Prerequisites</span></span>
<span data-ttu-id="4c9f7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c9f7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4c9f7-110">Permission type</span></span>|<span data-ttu-id="4c9f7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4c9f7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c9f7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4c9f7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c9f7-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c9f7-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c9f7-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4c9f7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c9f7-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-115">Not supported.</span></span>|
|<span data-ttu-id="4c9f7-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="4c9f7-116">Application</span></span>|<span data-ttu-id="4c9f7-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c9f7-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4c9f7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="4c9f7-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4c9f7-119">Request headers</span></span>
|<span data-ttu-id="4c9f7-120">标头</span><span class="sxs-lookup"><span data-stu-id="4c9f7-120">Header</span></span>|<span data-ttu-id="4c9f7-121">值</span><span class="sxs-lookup"><span data-stu-id="4c9f7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c9f7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c9f7-122">Authorization</span></span>|<span data-ttu-id="4c9f7-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c9f7-124">接受</span><span class="sxs-lookup"><span data-stu-id="4c9f7-124">Accept</span></span>|<span data-ttu-id="4c9f7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c9f7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c9f7-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4c9f7-126">Request body</span></span>
<span data-ttu-id="4c9f7-127">在请求正文中，提供 macOSGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-127">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="4c9f7-128">下表显示创建 macOSGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-128">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="4c9f7-129">属性</span><span class="sxs-lookup"><span data-stu-id="4c9f7-129">Property</span></span>|<span data-ttu-id="4c9f7-130">类型</span><span class="sxs-lookup"><span data-stu-id="4c9f7-130">Type</span></span>|<span data-ttu-id="4c9f7-131">说明</span><span class="sxs-lookup"><span data-stu-id="4c9f7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c9f7-132">id</span><span class="sxs-lookup"><span data-stu-id="4c9f7-132">id</span></span>|<span data-ttu-id="4c9f7-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4c9f7-133">String</span></span>|<span data-ttu-id="4c9f7-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-134">Key of the entity.</span></span> <span data-ttu-id="4c9f7-135">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c9f7-135">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c9f7-136">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4c9f7-136">lastModifiedDateTime</span></span>|<span data-ttu-id="4c9f7-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c9f7-137">DateTimeOffset</span></span>|<span data-ttu-id="4c9f7-138">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-138">DateTime the object was last modified.</span></span> <span data-ttu-id="4c9f7-139">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c9f7-139">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c9f7-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4c9f7-140">createdDateTime</span></span>|<span data-ttu-id="4c9f7-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4c9f7-141">DateTimeOffset</span></span>|<span data-ttu-id="4c9f7-142">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-142">DateTime the object was created.</span></span> <span data-ttu-id="4c9f7-143">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c9f7-143">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c9f7-144">description</span><span class="sxs-lookup"><span data-stu-id="4c9f7-144">description</span></span>|<span data-ttu-id="4c9f7-145">String</span><span class="sxs-lookup"><span data-stu-id="4c9f7-145">String</span></span>|<span data-ttu-id="4c9f7-146">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-146">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="4c9f7-147">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c9f7-147">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c9f7-148">displayName</span><span class="sxs-lookup"><span data-stu-id="4c9f7-148">displayName</span></span>|<span data-ttu-id="4c9f7-149">String</span><span class="sxs-lookup"><span data-stu-id="4c9f7-149">String</span></span>|<span data-ttu-id="4c9f7-150">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-150">Admin provided name of the device configuration.</span></span> <span data-ttu-id="4c9f7-151">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c9f7-151">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c9f7-152">version</span><span class="sxs-lookup"><span data-stu-id="4c9f7-152">version</span></span>|<span data-ttu-id="4c9f7-153">Int32</span><span class="sxs-lookup"><span data-stu-id="4c9f7-153">Int32</span></span>|<span data-ttu-id="4c9f7-154">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-154">Version of the device configuration.</span></span> <span data-ttu-id="4c9f7-155">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="4c9f7-155">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="4c9f7-156">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="4c9f7-156">compliantAppsList</span></span>|<span data-ttu-id="4c9f7-157">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="4c9f7-157">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="4c9f7-158">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-158">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="4c9f7-159">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-159">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="4c9f7-160">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="4c9f7-160">compliantAppListType</span></span>|[<span data-ttu-id="4c9f7-161">appListType</span><span class="sxs-lookup"><span data-stu-id="4c9f7-161">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="4c9f7-162">位于 CompliantAppsList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-162">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="4c9f7-163">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-163">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="4c9f7-164">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="4c9f7-164">emailInDomainSuffixes</span></span>|<span data-ttu-id="4c9f7-165">String 集合</span><span class="sxs-lookup"><span data-stu-id="4c9f7-165">String collection</span></span>|<span data-ttu-id="4c9f7-166">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-166">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="4c9f7-167">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="4c9f7-167">passwordBlockSimple</span></span>|<span data-ttu-id="4c9f7-168">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c9f7-168">Boolean</span></span>|<span data-ttu-id="4c9f7-169">阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-169">Block simple passwords.</span></span>|
|<span data-ttu-id="4c9f7-170">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="4c9f7-170">passwordExpirationDays</span></span>|<span data-ttu-id="4c9f7-171">Int32</span><span class="sxs-lookup"><span data-stu-id="4c9f7-171">Int32</span></span>|<span data-ttu-id="4c9f7-172">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-172">Number of days before the password expires.</span></span>|
|<span data-ttu-id="4c9f7-173">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="4c9f7-173">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="4c9f7-174">Int32</span><span class="sxs-lookup"><span data-stu-id="4c9f7-174">Int32</span></span>|<span data-ttu-id="4c9f7-175">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-175">Number of character sets a password must contain.</span></span> <span data-ttu-id="4c9f7-176">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="4c9f7-176">Valid values 0 to 4</span></span>|
|<span data-ttu-id="4c9f7-177">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="4c9f7-177">passwordMinimumLength</span></span>|<span data-ttu-id="4c9f7-178">Int32</span><span class="sxs-lookup"><span data-stu-id="4c9f7-178">Int32</span></span>|<span data-ttu-id="4c9f7-179">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-179">Minimum length of passwords.</span></span>|
|<span data-ttu-id="4c9f7-180">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="4c9f7-180">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="4c9f7-181">Int32</span><span class="sxs-lookup"><span data-stu-id="4c9f7-181">Int32</span></span>|<span data-ttu-id="4c9f7-182">在需要密码之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-182">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="4c9f7-183">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="4c9f7-183">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="4c9f7-184">Int32</span><span class="sxs-lookup"><span data-stu-id="4c9f7-184">Int32</span></span>|<span data-ttu-id="4c9f7-185">在屏幕超时之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-185">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="4c9f7-186">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="4c9f7-186">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="4c9f7-187">Int32</span><span class="sxs-lookup"><span data-stu-id="4c9f7-187">Int32</span></span>|<span data-ttu-id="4c9f7-188">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-188">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="4c9f7-189">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="4c9f7-189">passwordRequiredType</span></span>|[<span data-ttu-id="4c9f7-190">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="4c9f7-190">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="4c9f7-191">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-191">Type of password that is required.</span></span> <span data-ttu-id="4c9f7-192">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-192">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="4c9f7-193">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="4c9f7-193">passwordRequired</span></span>|<span data-ttu-id="4c9f7-194">Boolean</span><span class="sxs-lookup"><span data-stu-id="4c9f7-194">Boolean</span></span>|<span data-ttu-id="4c9f7-195">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-195">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="4c9f7-196">响应</span><span class="sxs-lookup"><span data-stu-id="4c9f7-196">Response</span></span>
<span data-ttu-id="4c9f7-197">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-197">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c9f7-198">示例</span><span class="sxs-lookup"><span data-stu-id="4c9f7-198">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c9f7-199">请求</span><span class="sxs-lookup"><span data-stu-id="4c9f7-199">Request</span></span>
<span data-ttu-id="4c9f7-200">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-200">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
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

### <a name="response"></a><span data-ttu-id="4c9f7-201">响应</span><span class="sxs-lookup"><span data-stu-id="4c9f7-201">Response</span></span>
<span data-ttu-id="4c9f7-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4c9f7-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






