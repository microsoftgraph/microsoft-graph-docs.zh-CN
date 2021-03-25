---
title: 创建 windowsPrivacyDataAccessControlItem
description: 创建新的 windowsPrivacyDataAccessControlItem 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 01b052e50bede136d1c4cf3f8ea2b555ff5fae48
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154705"
---
# <a name="create-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="390d2-103">创建 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="390d2-103">Create windowsPrivacyDataAccessControlItem</span></span>

<span data-ttu-id="390d2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="390d2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="390d2-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="390d2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="390d2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="390d2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="390d2-107">创建新的 [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="390d2-107">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="390d2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="390d2-108">Prerequisites</span></span>
<span data-ttu-id="390d2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="390d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="390d2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="390d2-111">Permission type</span></span>|<span data-ttu-id="390d2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="390d2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="390d2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="390d2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="390d2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="390d2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="390d2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="390d2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="390d2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="390d2-116">Not supported.</span></span>|
|<span data-ttu-id="390d2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="390d2-117">Application</span></span>|<span data-ttu-id="390d2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="390d2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="390d2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="390d2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="390d2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="390d2-120">Request headers</span></span>
|<span data-ttu-id="390d2-121">标头</span><span class="sxs-lookup"><span data-stu-id="390d2-121">Header</span></span>|<span data-ttu-id="390d2-122">值</span><span class="sxs-lookup"><span data-stu-id="390d2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="390d2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="390d2-123">Authorization</span></span>|<span data-ttu-id="390d2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="390d2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="390d2-125">接受</span><span class="sxs-lookup"><span data-stu-id="390d2-125">Accept</span></span>|<span data-ttu-id="390d2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="390d2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="390d2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="390d2-127">Request body</span></span>
<span data-ttu-id="390d2-128">在请求正文中，提供 windowsPrivacyDataAccessControlItem 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="390d2-128">In the request body, supply a JSON representation for the windowsPrivacyDataAccessControlItem object.</span></span>

<span data-ttu-id="390d2-129">下表显示创建 windowsPrivacyDataAccessControlItem 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="390d2-129">The following table shows the properties that are required when you create the windowsPrivacyDataAccessControlItem.</span></span>

|<span data-ttu-id="390d2-130">属性</span><span class="sxs-lookup"><span data-stu-id="390d2-130">Property</span></span>|<span data-ttu-id="390d2-131">类型</span><span class="sxs-lookup"><span data-stu-id="390d2-131">Type</span></span>|<span data-ttu-id="390d2-132">说明</span><span class="sxs-lookup"><span data-stu-id="390d2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="390d2-133">id</span><span class="sxs-lookup"><span data-stu-id="390d2-133">id</span></span>|<span data-ttu-id="390d2-134">String</span><span class="sxs-lookup"><span data-stu-id="390d2-134">String</span></span>|<span data-ttu-id="390d2-135">WindowsPrivacyDataAccessControlItem 的键。</span><span class="sxs-lookup"><span data-stu-id="390d2-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="390d2-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="390d2-136">accessLevel</span></span>|[<span data-ttu-id="390d2-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="390d2-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="390d2-138">这表示指定应用程序将进入的隐私数据类别的访问级别。</span><span class="sxs-lookup"><span data-stu-id="390d2-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="390d2-139">可取值为：`notConfigured`、`forceAllow`、`forceDeny`、`userInControl`。</span><span class="sxs-lookup"><span data-stu-id="390d2-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="390d2-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="390d2-140">dataCategory</span></span>|[<span data-ttu-id="390d2-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="390d2-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="390d2-142">这表示将应用特定访问控制的隐私数据类别。</span><span class="sxs-lookup"><span data-stu-id="390d2-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="390d2-143">可能的值是 `notConfigured` `accountInfo` `appsRunInBackground` ：、、、、、、、、 `calendar` `callHistory` `camera` `contacts` `diagnosticsInfo` `email` `location` `messaging` `microphone` `motion` `notifications` `phone` `radios` `tasks` `syncWithDevices` `trustedDevices` 。</span><span class="sxs-lookup"><span data-stu-id="390d2-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="390d2-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="390d2-144">appPackageFamilyName</span></span>|<span data-ttu-id="390d2-145">String</span><span class="sxs-lookup"><span data-stu-id="390d2-145">String</span></span>|<span data-ttu-id="390d2-146">Windows 应用的程序包系列名称。</span><span class="sxs-lookup"><span data-stu-id="390d2-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="390d2-147">设置后，访问级别将应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="390d2-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="390d2-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="390d2-148">appDisplayName</span></span>|<span data-ttu-id="390d2-149">String</span><span class="sxs-lookup"><span data-stu-id="390d2-149">String</span></span>|<span data-ttu-id="390d2-150">Windows 应用的程序包系列名称。</span><span class="sxs-lookup"><span data-stu-id="390d2-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="390d2-151">设置后，访问级别将应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="390d2-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="390d2-152">响应</span><span class="sxs-lookup"><span data-stu-id="390d2-152">Response</span></span>
<span data-ttu-id="390d2-153">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="390d2-153">If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="390d2-154">示例</span><span class="sxs-lookup"><span data-stu-id="390d2-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="390d2-155">请求</span><span class="sxs-lookup"><span data-stu-id="390d2-155">Request</span></span>
<span data-ttu-id="390d2-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="390d2-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="390d2-157">响应</span><span class="sxs-lookup"><span data-stu-id="390d2-157">Response</span></span>
<span data-ttu-id="390d2-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="390d2-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




