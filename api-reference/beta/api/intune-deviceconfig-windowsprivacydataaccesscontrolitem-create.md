---
title: 创建 windowsPrivacyDataAccessControlItem
description: 创建新的 windowsPrivacyDataAccessControlItem 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d1c578bb603559d2e1de54d1d56095763cb50e6e
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42732886"
---
# <a name="create-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="f7fe4-103">创建 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="f7fe4-103">Create windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="f7fe4-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7fe4-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7fe4-106">创建新的[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-106">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7fe4-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f7fe4-107">Prerequisites</span></span>
<span data-ttu-id="f7fe4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7fe4-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7fe4-110">Permission type</span></span>|<span data-ttu-id="f7fe4-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f7fe4-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7fe4-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7fe4-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f7fe4-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7fe4-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f7fe4-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7fe4-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7fe4-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-115">Not supported.</span></span>|
|<span data-ttu-id="f7fe4-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7fe4-116">Application</span></span>|<span data-ttu-id="f7fe4-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f7fe4-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7fe4-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7fe4-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="f7fe4-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7fe4-119">Request headers</span></span>
|<span data-ttu-id="f7fe4-120">标头</span><span class="sxs-lookup"><span data-stu-id="f7fe4-120">Header</span></span>|<span data-ttu-id="f7fe4-121">值</span><span class="sxs-lookup"><span data-stu-id="f7fe4-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7fe4-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7fe4-122">Authorization</span></span>|<span data-ttu-id="f7fe4-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7fe4-124">接受</span><span class="sxs-lookup"><span data-stu-id="f7fe4-124">Accept</span></span>|<span data-ttu-id="f7fe4-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f7fe4-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7fe4-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7fe4-126">Request body</span></span>
<span data-ttu-id="f7fe4-127">在请求正文中，提供 windowsPrivacyDataAccessControlItem 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-127">In the request body, supply a JSON representation for the windowsPrivacyDataAccessControlItem object.</span></span>

<span data-ttu-id="f7fe4-128">下表显示创建 windowsPrivacyDataAccessControlItem 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-128">The following table shows the properties that are required when you create the windowsPrivacyDataAccessControlItem.</span></span>

|<span data-ttu-id="f7fe4-129">属性</span><span class="sxs-lookup"><span data-stu-id="f7fe4-129">Property</span></span>|<span data-ttu-id="f7fe4-130">类型</span><span class="sxs-lookup"><span data-stu-id="f7fe4-130">Type</span></span>|<span data-ttu-id="f7fe4-131">说明</span><span class="sxs-lookup"><span data-stu-id="f7fe4-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f7fe4-132">id</span><span class="sxs-lookup"><span data-stu-id="f7fe4-132">id</span></span>|<span data-ttu-id="f7fe4-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f7fe4-133">String</span></span>|<span data-ttu-id="f7fe4-134">WindowsPrivacyDataAccessControlItem 的键。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-134">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="f7fe4-135">accessLevel</span><span class="sxs-lookup"><span data-stu-id="f7fe4-135">accessLevel</span></span>|[<span data-ttu-id="f7fe4-136">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="f7fe4-136">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="f7fe4-137">这表示将向其授予指定应用程序的隐私数据类别的访问级别。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-137">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="f7fe4-138">可取值为：`notConfigured`、`forceAllow`、`forceDeny`、`userInControl`。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-138">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="f7fe4-139">dataCategory</span><span class="sxs-lookup"><span data-stu-id="f7fe4-139">dataCategory</span></span>|[<span data-ttu-id="f7fe4-140">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="f7fe4-140">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="f7fe4-141">这表示将应用特定访问控制的隐私数据类别。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-141">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="f7fe4-142">可能的值为`notConfigured`： `accountInfo`、 `appsRunInBackground`、 `calendar` `callHistory` `camera` `contacts` `diagnosticsInfo` `email` `location` `messaging` `trustedDevices`、、 `notifications`、、、、、、、、、、、、、、、。 `microphone` `motion` `phone` `radios` `tasks` `syncWithDevices`</span><span class="sxs-lookup"><span data-stu-id="f7fe4-142">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="f7fe4-143">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="f7fe4-143">appPackageFamilyName</span></span>|<span data-ttu-id="f7fe4-144">String</span><span class="sxs-lookup"><span data-stu-id="f7fe4-144">String</span></span>|<span data-ttu-id="f7fe4-145">Windows 应用的程序包系列名称。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-145">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="f7fe4-146">设置后，该访问级别将应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-146">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="f7fe4-147">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="f7fe4-147">appDisplayName</span></span>|<span data-ttu-id="f7fe4-148">String</span><span class="sxs-lookup"><span data-stu-id="f7fe4-148">String</span></span>|<span data-ttu-id="f7fe4-149">Windows 应用的程序包系列名称。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-149">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="f7fe4-150">设置后，该访问级别将应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-150">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="f7fe4-151">响应</span><span class="sxs-lookup"><span data-stu-id="f7fe4-151">Response</span></span>
<span data-ttu-id="f7fe4-152">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-152">If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7fe4-153">示例</span><span class="sxs-lookup"><span data-stu-id="f7fe4-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7fe4-154">请求</span><span class="sxs-lookup"><span data-stu-id="f7fe4-154">Request</span></span>
<span data-ttu-id="f7fe4-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
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

### <a name="response"></a><span data-ttu-id="f7fe4-156">响应</span><span class="sxs-lookup"><span data-stu-id="f7fe4-156">Response</span></span>
<span data-ttu-id="f7fe4-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f7fe4-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




