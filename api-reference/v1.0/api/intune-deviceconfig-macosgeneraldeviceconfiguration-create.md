---
title: 创建 macOSGeneralDeviceConfiguration
description: 创建新的 macOSGeneralDeviceConfiguration 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e02159e9f577e001a675de5ee64768f63d1090c0
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32584255"
---
# <a name="create-macosgeneraldeviceconfiguration"></a><span data-ttu-id="19ab0-103">创建 macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="19ab0-103">Create macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="19ab0-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="19ab0-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="19ab0-105">创建新的 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="19ab0-105">Create a new [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="19ab0-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="19ab0-106">Prerequisites</span></span>
<span data-ttu-id="19ab0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="19ab0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="19ab0-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="19ab0-109">Permission type</span></span>|<span data-ttu-id="19ab0-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="19ab0-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="19ab0-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="19ab0-111">Delegated (work or school account)</span></span>|<span data-ttu-id="19ab0-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="19ab0-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="19ab0-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="19ab0-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="19ab0-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="19ab0-114">Not supported.</span></span>|
|<span data-ttu-id="19ab0-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="19ab0-115">Application</span></span>|<span data-ttu-id="19ab0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="19ab0-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="19ab0-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="19ab0-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="19ab0-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="19ab0-118">Request headers</span></span>
|<span data-ttu-id="19ab0-119">标头</span><span class="sxs-lookup"><span data-stu-id="19ab0-119">Header</span></span>|<span data-ttu-id="19ab0-120">值</span><span class="sxs-lookup"><span data-stu-id="19ab0-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="19ab0-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="19ab0-121">Authorization</span></span>|<span data-ttu-id="19ab0-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="19ab0-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="19ab0-123">接受</span><span class="sxs-lookup"><span data-stu-id="19ab0-123">Accept</span></span>|<span data-ttu-id="19ab0-124">application/json</span><span class="sxs-lookup"><span data-stu-id="19ab0-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="19ab0-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="19ab0-125">Request body</span></span>
<span data-ttu-id="19ab0-126">在请求正文中，提供 macOSGeneralDeviceConfiguration 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="19ab0-126">In the request body, supply a JSON representation for the macOSGeneralDeviceConfiguration object.</span></span>

<span data-ttu-id="19ab0-127">下表显示创建 macOSGeneralDeviceConfiguration 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="19ab0-127">The following table shows the properties that are required when you create the macOSGeneralDeviceConfiguration.</span></span>

|<span data-ttu-id="19ab0-128">属性</span><span class="sxs-lookup"><span data-stu-id="19ab0-128">Property</span></span>|<span data-ttu-id="19ab0-129">类型</span><span class="sxs-lookup"><span data-stu-id="19ab0-129">Type</span></span>|<span data-ttu-id="19ab0-130">说明</span><span class="sxs-lookup"><span data-stu-id="19ab0-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="19ab0-131">id</span><span class="sxs-lookup"><span data-stu-id="19ab0-131">id</span></span>|<span data-ttu-id="19ab0-132">字符串</span><span class="sxs-lookup"><span data-stu-id="19ab0-132">String</span></span>|<span data-ttu-id="19ab0-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="19ab0-133">Key of the entity.</span></span> <span data-ttu-id="19ab0-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19ab0-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19ab0-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="19ab0-135">lastModifiedDateTime</span></span>|<span data-ttu-id="19ab0-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19ab0-136">DateTimeOffset</span></span>|<span data-ttu-id="19ab0-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="19ab0-137">DateTime the object was last modified.</span></span> <span data-ttu-id="19ab0-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19ab0-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19ab0-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="19ab0-139">createdDateTime</span></span>|<span data-ttu-id="19ab0-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="19ab0-140">DateTimeOffset</span></span>|<span data-ttu-id="19ab0-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="19ab0-141">DateTime the object was created.</span></span> <span data-ttu-id="19ab0-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19ab0-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19ab0-143">说明</span><span class="sxs-lookup"><span data-stu-id="19ab0-143">description</span></span>|<span data-ttu-id="19ab0-144">String</span><span class="sxs-lookup"><span data-stu-id="19ab0-144">String</span></span>|<span data-ttu-id="19ab0-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="19ab0-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="19ab0-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19ab0-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19ab0-147">displayName</span><span class="sxs-lookup"><span data-stu-id="19ab0-147">displayName</span></span>|<span data-ttu-id="19ab0-148">String</span><span class="sxs-lookup"><span data-stu-id="19ab0-148">String</span></span>|<span data-ttu-id="19ab0-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="19ab0-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="19ab0-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19ab0-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19ab0-151">version</span><span class="sxs-lookup"><span data-stu-id="19ab0-151">version</span></span>|<span data-ttu-id="19ab0-152">Int32</span><span class="sxs-lookup"><span data-stu-id="19ab0-152">Int32</span></span>|<span data-ttu-id="19ab0-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="19ab0-153">Version of the device configuration.</span></span> <span data-ttu-id="19ab0-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="19ab0-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="19ab0-155">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="19ab0-155">compliantAppsList</span></span>|<span data-ttu-id="19ab0-156">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="19ab0-156">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="19ab0-157">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="19ab0-157">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="19ab0-158">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="19ab0-158">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="19ab0-159">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="19ab0-159">compliantAppListType</span></span>|[<span data-ttu-id="19ab0-160">appListType</span><span class="sxs-lookup"><span data-stu-id="19ab0-160">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="19ab0-161">位于 CompliantAppsList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="19ab0-161">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="19ab0-162">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="19ab0-162">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="19ab0-163">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="19ab0-163">emailInDomainSuffixes</span></span>|<span data-ttu-id="19ab0-164">String 集合</span><span class="sxs-lookup"><span data-stu-id="19ab0-164">String collection</span></span>|<span data-ttu-id="19ab0-165">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="19ab0-165">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="19ab0-166">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="19ab0-166">passwordBlockSimple</span></span>|<span data-ttu-id="19ab0-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="19ab0-167">Boolean</span></span>|<span data-ttu-id="19ab0-168">阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="19ab0-168">Block simple passwords.</span></span>|
|<span data-ttu-id="19ab0-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="19ab0-169">passwordExpirationDays</span></span>|<span data-ttu-id="19ab0-170">Int32</span><span class="sxs-lookup"><span data-stu-id="19ab0-170">Int32</span></span>|<span data-ttu-id="19ab0-171">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="19ab0-171">Number of days before the password expires.</span></span>|
|<span data-ttu-id="19ab0-172">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="19ab0-172">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="19ab0-173">Int32</span><span class="sxs-lookup"><span data-stu-id="19ab0-173">Int32</span></span>|<span data-ttu-id="19ab0-174">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="19ab0-174">Number of character sets a password must contain.</span></span> <span data-ttu-id="19ab0-175">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="19ab0-175">Valid values 0 to 4</span></span>|
|<span data-ttu-id="19ab0-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="19ab0-176">passwordMinimumLength</span></span>|<span data-ttu-id="19ab0-177">Int32</span><span class="sxs-lookup"><span data-stu-id="19ab0-177">Int32</span></span>|<span data-ttu-id="19ab0-178">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="19ab0-178">Minimum length of passwords.</span></span>|
|<span data-ttu-id="19ab0-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="19ab0-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="19ab0-180">Int32</span><span class="sxs-lookup"><span data-stu-id="19ab0-180">Int32</span></span>|<span data-ttu-id="19ab0-181">在需要密码之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="19ab0-181">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="19ab0-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="19ab0-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="19ab0-183">Int32</span><span class="sxs-lookup"><span data-stu-id="19ab0-183">Int32</span></span>|<span data-ttu-id="19ab0-184">在屏幕超时之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="19ab0-184">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="19ab0-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="19ab0-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="19ab0-186">Int32</span><span class="sxs-lookup"><span data-stu-id="19ab0-186">Int32</span></span>|<span data-ttu-id="19ab0-187">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="19ab0-187">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="19ab0-188">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="19ab0-188">passwordRequiredType</span></span>|[<span data-ttu-id="19ab0-189">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="19ab0-189">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="19ab0-190">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="19ab0-190">Type of password that is required.</span></span> <span data-ttu-id="19ab0-191">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="19ab0-191">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="19ab0-192">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="19ab0-192">passwordRequired</span></span>|<span data-ttu-id="19ab0-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="19ab0-193">Boolean</span></span>|<span data-ttu-id="19ab0-194">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="19ab0-194">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="19ab0-195">响应</span><span class="sxs-lookup"><span data-stu-id="19ab0-195">Response</span></span>
<span data-ttu-id="19ab0-196">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="19ab0-196">If successful, this method returns a `201 Created` response code and a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="19ab0-197">示例</span><span class="sxs-lookup"><span data-stu-id="19ab0-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="19ab0-198">请求</span><span class="sxs-lookup"><span data-stu-id="19ab0-198">Request</span></span>
<span data-ttu-id="19ab0-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="19ab0-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="19ab0-200">响应</span><span class="sxs-lookup"><span data-stu-id="19ab0-200">Response</span></span>
<span data-ttu-id="19ab0-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="19ab0-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



