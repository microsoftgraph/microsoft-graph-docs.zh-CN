---
title: 更新 windowsPrivacyDataAccessControlItem
description: 更新 windowsPrivacyDataAccessControlItem 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 85c912c244d2554fd9a05ccaedf16bf60cfc565d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51147082"
---
# <a name="update-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="2a70e-103">更新 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="2a70e-103">Update windowsPrivacyDataAccessControlItem</span></span>

<span data-ttu-id="2a70e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2a70e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2a70e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2a70e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2a70e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2a70e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2a70e-107">更新 [windowsPrivacyDataAccessControlItem 对象](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="2a70e-107">Update the properties of a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2a70e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2a70e-108">Prerequisites</span></span>
<span data-ttu-id="2a70e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2a70e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2a70e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2a70e-111">Permission type</span></span>|<span data-ttu-id="2a70e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2a70e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2a70e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2a70e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2a70e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a70e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2a70e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2a70e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2a70e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2a70e-116">Not supported.</span></span>|
|<span data-ttu-id="2a70e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2a70e-117">Application</span></span>|<span data-ttu-id="2a70e-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2a70e-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2a70e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2a70e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls/{windowsPrivacyDataAccessControlItemId}
```

## <a name="request-headers"></a><span data-ttu-id="2a70e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2a70e-120">Request headers</span></span>
|<span data-ttu-id="2a70e-121">标头</span><span class="sxs-lookup"><span data-stu-id="2a70e-121">Header</span></span>|<span data-ttu-id="2a70e-122">值</span><span class="sxs-lookup"><span data-stu-id="2a70e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2a70e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2a70e-123">Authorization</span></span>|<span data-ttu-id="2a70e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2a70e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2a70e-125">接受</span><span class="sxs-lookup"><span data-stu-id="2a70e-125">Accept</span></span>|<span data-ttu-id="2a70e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2a70e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2a70e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2a70e-127">Request body</span></span>
<span data-ttu-id="2a70e-128">在请求正文中，提供 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2a70e-128">In the request body, supply a JSON representation for the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

<span data-ttu-id="2a70e-129">下表显示创建 [windowsPrivacyDataAccessControlItem 时所需的属性](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)。</span><span class="sxs-lookup"><span data-stu-id="2a70e-129">The following table shows the properties that are required when you create the [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md).</span></span>

|<span data-ttu-id="2a70e-130">属性</span><span class="sxs-lookup"><span data-stu-id="2a70e-130">Property</span></span>|<span data-ttu-id="2a70e-131">类型</span><span class="sxs-lookup"><span data-stu-id="2a70e-131">Type</span></span>|<span data-ttu-id="2a70e-132">说明</span><span class="sxs-lookup"><span data-stu-id="2a70e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2a70e-133">id</span><span class="sxs-lookup"><span data-stu-id="2a70e-133">id</span></span>|<span data-ttu-id="2a70e-134">String</span><span class="sxs-lookup"><span data-stu-id="2a70e-134">String</span></span>|<span data-ttu-id="2a70e-135">WindowsPrivacyDataAccessControlItem 的键。</span><span class="sxs-lookup"><span data-stu-id="2a70e-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="2a70e-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="2a70e-136">accessLevel</span></span>|[<span data-ttu-id="2a70e-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="2a70e-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="2a70e-138">这表示指定应用程序将进入的隐私数据类别的访问级别。</span><span class="sxs-lookup"><span data-stu-id="2a70e-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="2a70e-139">可取值为：`notConfigured`、`forceAllow`、`forceDeny`、`userInControl`。</span><span class="sxs-lookup"><span data-stu-id="2a70e-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="2a70e-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="2a70e-140">dataCategory</span></span>|[<span data-ttu-id="2a70e-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="2a70e-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="2a70e-142">这表示将应用特定访问控制的隐私数据类别。</span><span class="sxs-lookup"><span data-stu-id="2a70e-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="2a70e-143">可能的值是 `notConfigured` `accountInfo` `appsRunInBackground` ：、、、、、、、、 `calendar` `callHistory` `camera` `contacts` `diagnosticsInfo` `email` `location` `messaging` `microphone` `motion` `notifications` `phone` `radios` `tasks` `syncWithDevices` `trustedDevices` 。</span><span class="sxs-lookup"><span data-stu-id="2a70e-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="2a70e-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="2a70e-144">appPackageFamilyName</span></span>|<span data-ttu-id="2a70e-145">String</span><span class="sxs-lookup"><span data-stu-id="2a70e-145">String</span></span>|<span data-ttu-id="2a70e-146">Windows 应用的程序包系列名称。</span><span class="sxs-lookup"><span data-stu-id="2a70e-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="2a70e-147">设置后，访问级别将应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="2a70e-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="2a70e-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="2a70e-148">appDisplayName</span></span>|<span data-ttu-id="2a70e-149">String</span><span class="sxs-lookup"><span data-stu-id="2a70e-149">String</span></span>|<span data-ttu-id="2a70e-150">Windows 应用的程序包系列名称。</span><span class="sxs-lookup"><span data-stu-id="2a70e-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="2a70e-151">设置后，访问级别将应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="2a70e-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="2a70e-152">响应</span><span class="sxs-lookup"><span data-stu-id="2a70e-152">Response</span></span>
<span data-ttu-id="2a70e-153">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2a70e-153">If successful, this method returns a `200 OK` response code and an updated [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2a70e-154">示例</span><span class="sxs-lookup"><span data-stu-id="2a70e-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="2a70e-155">请求</span><span class="sxs-lookup"><span data-stu-id="2a70e-155">Request</span></span>
<span data-ttu-id="2a70e-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2a70e-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="2a70e-157">响应</span><span class="sxs-lookup"><span data-stu-id="2a70e-157">Response</span></span>
<span data-ttu-id="2a70e-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2a70e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




