---
title: 更新 macOSGeneralDeviceConfiguration
description: 更新 macOSGeneralDeviceConfiguration 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 13bc10d91285f1f599b3ef33180867636cd0569f
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37365864"
---
# <a name="update-macosgeneraldeviceconfiguration"></a><span data-ttu-id="71298-103">更新 macOSGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="71298-103">Update macOSGeneralDeviceConfiguration</span></span>

> <span data-ttu-id="71298-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="71298-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="71298-105">更新 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="71298-105">Update the properties of a [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="71298-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="71298-106">Prerequisites</span></span>
<span data-ttu-id="71298-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71298-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="71298-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="71298-109">Permission type</span></span>|<span data-ttu-id="71298-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="71298-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="71298-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71298-111">Delegated (work or school account)</span></span>|<span data-ttu-id="71298-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71298-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="71298-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71298-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71298-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="71298-114">Not supported.</span></span>|
|<span data-ttu-id="71298-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="71298-115">Application</span></span>|<span data-ttu-id="71298-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="71298-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71298-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71298-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="71298-118">请求头</span><span class="sxs-lookup"><span data-stu-id="71298-118">Request headers</span></span>
|<span data-ttu-id="71298-119">标头</span><span class="sxs-lookup"><span data-stu-id="71298-119">Header</span></span>|<span data-ttu-id="71298-120">值</span><span class="sxs-lookup"><span data-stu-id="71298-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="71298-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="71298-121">Authorization</span></span>|<span data-ttu-id="71298-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="71298-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="71298-123">接受</span><span class="sxs-lookup"><span data-stu-id="71298-123">Accept</span></span>|<span data-ttu-id="71298-124">application/json</span><span class="sxs-lookup"><span data-stu-id="71298-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="71298-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="71298-125">Request body</span></span>
<span data-ttu-id="71298-126">在请求正文中，提供 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="71298-126">In the request body, supply a JSON representation for the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object.</span></span>

<span data-ttu-id="71298-127">下表显示创建 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="71298-127">The following table shows the properties that are required when you create the [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md).</span></span>

|<span data-ttu-id="71298-128">属性</span><span class="sxs-lookup"><span data-stu-id="71298-128">Property</span></span>|<span data-ttu-id="71298-129">类型</span><span class="sxs-lookup"><span data-stu-id="71298-129">Type</span></span>|<span data-ttu-id="71298-130">说明</span><span class="sxs-lookup"><span data-stu-id="71298-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="71298-131">id</span><span class="sxs-lookup"><span data-stu-id="71298-131">id</span></span>|<span data-ttu-id="71298-132">字符串</span><span class="sxs-lookup"><span data-stu-id="71298-132">String</span></span>|<span data-ttu-id="71298-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="71298-133">Key of the entity.</span></span> <span data-ttu-id="71298-134">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71298-134">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71298-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="71298-135">lastModifiedDateTime</span></span>|<span data-ttu-id="71298-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71298-136">DateTimeOffset</span></span>|<span data-ttu-id="71298-137">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="71298-137">DateTime the object was last modified.</span></span> <span data-ttu-id="71298-138">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71298-138">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71298-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="71298-139">createdDateTime</span></span>|<span data-ttu-id="71298-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="71298-140">DateTimeOffset</span></span>|<span data-ttu-id="71298-141">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="71298-141">DateTime the object was created.</span></span> <span data-ttu-id="71298-142">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71298-142">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71298-143">说明</span><span class="sxs-lookup"><span data-stu-id="71298-143">description</span></span>|<span data-ttu-id="71298-144">String</span><span class="sxs-lookup"><span data-stu-id="71298-144">String</span></span>|<span data-ttu-id="71298-145">管理员提供的设备配置的说明。</span><span class="sxs-lookup"><span data-stu-id="71298-145">Admin provided description of the Device Configuration.</span></span> <span data-ttu-id="71298-146">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71298-146">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71298-147">displayName</span><span class="sxs-lookup"><span data-stu-id="71298-147">displayName</span></span>|<span data-ttu-id="71298-148">String</span><span class="sxs-lookup"><span data-stu-id="71298-148">String</span></span>|<span data-ttu-id="71298-149">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="71298-149">Admin provided name of the device configuration.</span></span> <span data-ttu-id="71298-150">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71298-150">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71298-151">version</span><span class="sxs-lookup"><span data-stu-id="71298-151">version</span></span>|<span data-ttu-id="71298-152">Int32</span><span class="sxs-lookup"><span data-stu-id="71298-152">Int32</span></span>|<span data-ttu-id="71298-153">设备配置的版本。</span><span class="sxs-lookup"><span data-stu-id="71298-153">Version of the device configuration.</span></span> <span data-ttu-id="71298-154">继承自 [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span><span class="sxs-lookup"><span data-stu-id="71298-154">Inherited from [deviceConfiguration](../resources/intune-deviceconfig-deviceconfiguration.md)</span></span>|
|<span data-ttu-id="71298-155">compliantAppsList</span><span class="sxs-lookup"><span data-stu-id="71298-155">compliantAppsList</span></span>|<span data-ttu-id="71298-156">[appListItem](../resources/intune-deviceconfig-applistitem.md) 集合</span><span class="sxs-lookup"><span data-stu-id="71298-156">[appListItem](../resources/intune-deviceconfig-applistitem.md) collection</span></span>|<span data-ttu-id="71298-157">符合性中的应用列表（允许列表或阻止列表，由 CompliantAppListType 控制）。</span><span class="sxs-lookup"><span data-stu-id="71298-157">List of apps in the compliance (either allow list or block list, controlled by CompliantAppListType).</span></span> <span data-ttu-id="71298-158">该集合最多可包含 10000 个元素。</span><span class="sxs-lookup"><span data-stu-id="71298-158">This collection can contain a maximum of 10000 elements.</span></span>|
|<span data-ttu-id="71298-159">compliantAppListType</span><span class="sxs-lookup"><span data-stu-id="71298-159">compliantAppListType</span></span>|[<span data-ttu-id="71298-160">appListType</span><span class="sxs-lookup"><span data-stu-id="71298-160">appListType</span></span>](../resources/intune-deviceconfig-applisttype.md)|<span data-ttu-id="71298-161">位于 CompliantAppsList 中的列表。</span><span class="sxs-lookup"><span data-stu-id="71298-161">List that is in the CompliantAppsList.</span></span> <span data-ttu-id="71298-162">可取值为：`none`、`appsInListCompliant`、`appsNotInListCompliant`。</span><span class="sxs-lookup"><span data-stu-id="71298-162">Possible values are: `none`, `appsInListCompliant`, `appsNotInListCompliant`.</span></span>|
|<span data-ttu-id="71298-163">emailInDomainSuffixes</span><span class="sxs-lookup"><span data-stu-id="71298-163">emailInDomainSuffixes</span></span>|<span data-ttu-id="71298-164">String 集合</span><span class="sxs-lookup"><span data-stu-id="71298-164">String collection</span></span>|<span data-ttu-id="71298-165">缺少匹配任何这些字符串的后缀的电子邮件地址将被视为超出域范围。</span><span class="sxs-lookup"><span data-stu-id="71298-165">An email address lacking a suffix that matches any of these strings will be considered out-of-domain.</span></span>|
|<span data-ttu-id="71298-166">passwordBlockSimple</span><span class="sxs-lookup"><span data-stu-id="71298-166">passwordBlockSimple</span></span>|<span data-ttu-id="71298-167">Boolean</span><span class="sxs-lookup"><span data-stu-id="71298-167">Boolean</span></span>|<span data-ttu-id="71298-168">阻止简单密码。</span><span class="sxs-lookup"><span data-stu-id="71298-168">Block simple passwords.</span></span>|
|<span data-ttu-id="71298-169">passwordExpirationDays</span><span class="sxs-lookup"><span data-stu-id="71298-169">passwordExpirationDays</span></span>|<span data-ttu-id="71298-170">Int32</span><span class="sxs-lookup"><span data-stu-id="71298-170">Int32</span></span>|<span data-ttu-id="71298-171">密码过期前的天数。</span><span class="sxs-lookup"><span data-stu-id="71298-171">Number of days before the password expires.</span></span>|
|<span data-ttu-id="71298-172">passwordMinimumCharacterSetCount</span><span class="sxs-lookup"><span data-stu-id="71298-172">passwordMinimumCharacterSetCount</span></span>|<span data-ttu-id="71298-173">Int32</span><span class="sxs-lookup"><span data-stu-id="71298-173">Int32</span></span>|<span data-ttu-id="71298-174">密码必须包含的字符集数。</span><span class="sxs-lookup"><span data-stu-id="71298-174">Number of character sets a password must contain.</span></span> <span data-ttu-id="71298-175">有效值为 0 至 4</span><span class="sxs-lookup"><span data-stu-id="71298-175">Valid values 0 to 4</span></span>|
|<span data-ttu-id="71298-176">passwordMinimumLength</span><span class="sxs-lookup"><span data-stu-id="71298-176">passwordMinimumLength</span></span>|<span data-ttu-id="71298-177">Int32</span><span class="sxs-lookup"><span data-stu-id="71298-177">Int32</span></span>|<span data-ttu-id="71298-178">密码的最小长度。</span><span class="sxs-lookup"><span data-stu-id="71298-178">Minimum length of passwords.</span></span>|
|<span data-ttu-id="71298-179">passwordMinutesOfInactivityBeforeLock</span><span class="sxs-lookup"><span data-stu-id="71298-179">passwordMinutesOfInactivityBeforeLock</span></span>|<span data-ttu-id="71298-180">Int32</span><span class="sxs-lookup"><span data-stu-id="71298-180">Int32</span></span>|<span data-ttu-id="71298-181">在需要密码之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="71298-181">Minutes of inactivity required before a password is required.</span></span>|
|<span data-ttu-id="71298-182">passwordMinutesOfInactivityBeforeScreenTimeout</span><span class="sxs-lookup"><span data-stu-id="71298-182">passwordMinutesOfInactivityBeforeScreenTimeout</span></span>|<span data-ttu-id="71298-183">Int32</span><span class="sxs-lookup"><span data-stu-id="71298-183">Int32</span></span>|<span data-ttu-id="71298-184">在屏幕超时之前需要不活动的分钟数。</span><span class="sxs-lookup"><span data-stu-id="71298-184">Minutes of inactivity required before the screen times out.</span></span>|
|<span data-ttu-id="71298-185">passwordPreviousPasswordBlockCount</span><span class="sxs-lookup"><span data-stu-id="71298-185">passwordPreviousPasswordBlockCount</span></span>|<span data-ttu-id="71298-186">Int32</span><span class="sxs-lookup"><span data-stu-id="71298-186">Int32</span></span>|<span data-ttu-id="71298-187">要阻止的以前密码的数量。</span><span class="sxs-lookup"><span data-stu-id="71298-187">Number of previous passwords to block.</span></span>|
|<span data-ttu-id="71298-188">passwordRequiredType</span><span class="sxs-lookup"><span data-stu-id="71298-188">passwordRequiredType</span></span>|[<span data-ttu-id="71298-189">requiredPasswordType</span><span class="sxs-lookup"><span data-stu-id="71298-189">requiredPasswordType</span></span>](../resources/intune-deviceconfig-requiredpasswordtype.md)|<span data-ttu-id="71298-190">必需的密码类型。</span><span class="sxs-lookup"><span data-stu-id="71298-190">Type of password that is required.</span></span> <span data-ttu-id="71298-191">可取值为：`deviceDefault`、`alphanumeric`、`numeric`。</span><span class="sxs-lookup"><span data-stu-id="71298-191">Possible values are: `deviceDefault`, `alphanumeric`, `numeric`.</span></span>|
|<span data-ttu-id="71298-192">passwordRequired</span><span class="sxs-lookup"><span data-stu-id="71298-192">passwordRequired</span></span>|<span data-ttu-id="71298-193">Boolean</span><span class="sxs-lookup"><span data-stu-id="71298-193">Boolean</span></span>|<span data-ttu-id="71298-194">是否需要密码。</span><span class="sxs-lookup"><span data-stu-id="71298-194">Whether or not to require a password.</span></span>|



## <a name="response"></a><span data-ttu-id="71298-195">响应</span><span class="sxs-lookup"><span data-stu-id="71298-195">Response</span></span>
<span data-ttu-id="71298-196">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="71298-196">If successful, this method returns a `200 OK` response code and an updated [macOSGeneralDeviceConfiguration](../resources/intune-deviceconfig-macosgeneraldeviceconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71298-197">示例</span><span class="sxs-lookup"><span data-stu-id="71298-197">Example</span></span>

### <a name="request"></a><span data-ttu-id="71298-198">请求</span><span class="sxs-lookup"><span data-stu-id="71298-198">Request</span></span>
<span data-ttu-id="71298-199">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="71298-199">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="71298-200">响应</span><span class="sxs-lookup"><span data-stu-id="71298-200">Response</span></span>
<span data-ttu-id="71298-p112">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="71298-p112">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




