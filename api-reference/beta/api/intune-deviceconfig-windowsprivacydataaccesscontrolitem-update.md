---
title: 更新 windowsPrivacyDataAccessControlItem
description: 更新 windowsPrivacyDataAccessControlItem 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: e380085a91a7e02ce729d28888a563932c54be17
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30166120"
---
# <a name="update-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="963df-103">更新 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="963df-103">Update windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="963df-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="963df-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="963df-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="963df-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="963df-106">更新[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="963df-106">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="963df-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="963df-107">Prerequisites</span></span>
<span data-ttu-id="963df-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="963df-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="963df-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="963df-110">Permission type</span></span>|<span data-ttu-id="963df-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="963df-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="963df-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="963df-112">Delegated (work or school account)</span></span>|<span data-ttu-id="963df-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="963df-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="963df-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="963df-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="963df-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="963df-115">Not supported.</span></span>|
|<span data-ttu-id="963df-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="963df-116">Application</span></span>|<span data-ttu-id="963df-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="963df-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="963df-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="963df-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="request-headers"></a><span data-ttu-id="963df-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="963df-119">Request headers</span></span>
|<span data-ttu-id="963df-120">标头</span><span class="sxs-lookup"><span data-stu-id="963df-120">Header</span></span>|<span data-ttu-id="963df-121">值</span><span class="sxs-lookup"><span data-stu-id="963df-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="963df-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="963df-122">Authorization</span></span>|<span data-ttu-id="963df-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="963df-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="963df-124">Accept</span><span class="sxs-lookup"><span data-stu-id="963df-124">Accept</span></span>|<span data-ttu-id="963df-125">application/json</span><span class="sxs-lookup"><span data-stu-id="963df-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="963df-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="963df-126">Request body</span></span>
<span data-ttu-id="963df-127">在请求正文中, 提供[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="963df-127">In the request body, supply a JSON representation for the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

<span data-ttu-id="963df-128">下表显示创建[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="963df-128">The following table shows the properties that are required when you create the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>

|<span data-ttu-id="963df-129">属性</span><span class="sxs-lookup"><span data-stu-id="963df-129">Property</span></span>|<span data-ttu-id="963df-130">类型</span><span class="sxs-lookup"><span data-stu-id="963df-130">Type</span></span>|<span data-ttu-id="963df-131">说明</span><span class="sxs-lookup"><span data-stu-id="963df-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="963df-132">id</span><span class="sxs-lookup"><span data-stu-id="963df-132">id</span></span>|<span data-ttu-id="963df-133">字符串</span><span class="sxs-lookup"><span data-stu-id="963df-133">String</span></span>|<span data-ttu-id="963df-134">WindowsPrivacyDataAccessControlItem 的键。</span><span class="sxs-lookup"><span data-stu-id="963df-134">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="963df-135">accessLevel</span><span class="sxs-lookup"><span data-stu-id="963df-135">accessLevel</span></span>|[<span data-ttu-id="963df-136">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="963df-136">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="963df-137">这表示将向其授予指定应用程序的隐私数据类别的访问级别。</span><span class="sxs-lookup"><span data-stu-id="963df-137">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="963df-138">可取值为：`notConfigured`、`forceAllow`、`forceDeny`、`userInControl`。</span><span class="sxs-lookup"><span data-stu-id="963df-138">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="963df-139">dataCategory</span><span class="sxs-lookup"><span data-stu-id="963df-139">dataCategory</span></span>|[<span data-ttu-id="963df-140">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="963df-140">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="963df-141">这表示将应用特定访问控制的隐私数据类别。</span><span class="sxs-lookup"><span data-stu-id="963df-141">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="963df-142">可能的值为`notConfigured`: `accountInfo`、 `appsRunInBackground`、 `calendar` `callHistory` `camera` `contacts` `diagnosticsInfo` `email` `location` `messaging` `microphone` `motion`、、、、、、、、、、、、、、、、 `notifications` `phone` `radios` `tasks` `syncWithDevices` `trustedDevices`.</span><span class="sxs-lookup"><span data-stu-id="963df-142">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="963df-143">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="963df-143">appPackageFamilyName</span></span>|<span data-ttu-id="963df-144">String</span><span class="sxs-lookup"><span data-stu-id="963df-144">String</span></span>|<span data-ttu-id="963df-145">Windows 应用的程序包系列名称。</span><span class="sxs-lookup"><span data-stu-id="963df-145">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="963df-146">设置后, 该访问级别将应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="963df-146">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="963df-147">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="963df-147">appDisplayName</span></span>|<span data-ttu-id="963df-148">String</span><span class="sxs-lookup"><span data-stu-id="963df-148">String</span></span>|<span data-ttu-id="963df-149">Windows 应用的程序包系列名称。</span><span class="sxs-lookup"><span data-stu-id="963df-149">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="963df-150">设置后, 该访问级别将应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="963df-150">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="963df-151">响应</span><span class="sxs-lookup"><span data-stu-id="963df-151">Response</span></span>
<span data-ttu-id="963df-152">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="963df-152">If successful, this method returns a `200 OK` response code and an updated [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="963df-153">示例</span><span class="sxs-lookup"><span data-stu-id="963df-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="963df-154">请求</span><span class="sxs-lookup"><span data-stu-id="963df-154">Request</span></span>
<span data-ttu-id="963df-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="963df-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
Content-type: application/json
Content-length: 250

{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "accessLevel": "forceAllow",
  "dataCategory": "accountInfo",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="963df-156">响应</span><span class="sxs-lookup"><span data-stu-id="963df-156">Response</span></span>
<span data-ttu-id="963df-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="963df-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 299

{
  "@odata.type": "#microsoft.graph.windowsPrivacyDataAccessControlItem",
  "id": "03b15556-5556-03b1-5655-b1035655b103",
  "accessLevel": "forceAllow",
  "dataCategory": "accountInfo",
  "appPackageFamilyName": "App Package Family Name value",
  "appDisplayName": "App Display Name value"
}
```




