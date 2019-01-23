---
title: 创建 windowsPrivacyDataAccessControlItem
description: 创建新的 windowsPrivacyDataAccessControlItem 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: e7b78a113134b4d268df3c759dfd7dc700759a35
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405581"
---
# <a name="create-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="e4670-103">创建 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="e4670-103">Create windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="e4670-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="e4670-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e4670-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e4670-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e4670-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e4670-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e4670-107">创建新的[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e4670-107">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e4670-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e4670-108">Prerequisites</span></span>
<span data-ttu-id="e4670-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="e4670-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e4670-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e4670-111">Permission type</span></span>|<span data-ttu-id="e4670-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e4670-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e4670-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e4670-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e4670-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e4670-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e4670-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e4670-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e4670-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4670-116">Not supported.</span></span>|
|<span data-ttu-id="e4670-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e4670-117">Application</span></span>|<span data-ttu-id="e4670-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e4670-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e4670-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e4670-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="e4670-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e4670-120">Request headers</span></span>
|<span data-ttu-id="e4670-121">标头</span><span class="sxs-lookup"><span data-stu-id="e4670-121">Header</span></span>|<span data-ttu-id="e4670-122">值</span><span class="sxs-lookup"><span data-stu-id="e4670-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e4670-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e4670-123">Authorization</span></span>|<span data-ttu-id="e4670-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e4670-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e4670-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e4670-125">Accept</span></span>|<span data-ttu-id="e4670-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e4670-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e4670-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e4670-127">Request body</span></span>
<span data-ttu-id="e4670-128">在请求正文中，提供 windowsPrivacyDataAccessControlItem 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e4670-128">In the request body, supply a JSON representation for the windowsPrivacyDataAccessControlItem object.</span></span>

<span data-ttu-id="e4670-129">下表显示时创建 windowsPrivacyDataAccessControlItem 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e4670-129">The following table shows the properties that are required when you create the windowsPrivacyDataAccessControlItem.</span></span>

|<span data-ttu-id="e4670-130">属性</span><span class="sxs-lookup"><span data-stu-id="e4670-130">Property</span></span>|<span data-ttu-id="e4670-131">类型</span><span class="sxs-lookup"><span data-stu-id="e4670-131">Type</span></span>|<span data-ttu-id="e4670-132">说明</span><span class="sxs-lookup"><span data-stu-id="e4670-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e4670-133">id</span><span class="sxs-lookup"><span data-stu-id="e4670-133">id</span></span>|<span data-ttu-id="e4670-134">String</span><span class="sxs-lookup"><span data-stu-id="e4670-134">String</span></span>|<span data-ttu-id="e4670-135">WindowsPrivacyDataAccessControlItem 键。</span><span class="sxs-lookup"><span data-stu-id="e4670-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="e4670-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="e4670-136">accessLevel</span></span>|[<span data-ttu-id="e4670-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="e4670-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="e4670-138">这指示到指定的应用程序会授予对隐私数据类别的访问级别。</span><span class="sxs-lookup"><span data-stu-id="e4670-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="e4670-139">可取值为：`notConfigured`、`forceAllow`、`forceDeny`、`userInControl`。</span><span class="sxs-lookup"><span data-stu-id="e4670-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="e4670-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="e4670-140">dataCategory</span></span>|[<span data-ttu-id="e4670-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="e4670-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="e4670-142">这指示特定的访问控制将应用于哪个隐私数据类别。</span><span class="sxs-lookup"><span data-stu-id="e4670-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="e4670-143">可能的值为： `notConfigured`， `accountInfo`， `appsRunInBackground`， `calendar`， `callHistory`， `camera`， `contacts`， `diagnosticsInfo`， `email`， `location`， `messaging`， `microphone`， `motion`， `notifications`， `phone`， `radios`， `tasks`， `syncWithDevices`， `trustedDevices`.</span><span class="sxs-lookup"><span data-stu-id="e4670-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="e4670-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="e4670-144">appPackageFamilyName</span></span>|<span data-ttu-id="e4670-145">String</span><span class="sxs-lookup"><span data-stu-id="e4670-145">String</span></span>|<span data-ttu-id="e4670-146">包系列 Windows 应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="e4670-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="e4670-147">设置时，访问级别应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="e4670-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="e4670-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="e4670-148">appDisplayName</span></span>|<span data-ttu-id="e4670-149">String</span><span class="sxs-lookup"><span data-stu-id="e4670-149">String</span></span>|<span data-ttu-id="e4670-150">包系列 Windows 应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="e4670-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="e4670-151">设置时，访问级别应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="e4670-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="e4670-152">响应</span><span class="sxs-lookup"><span data-stu-id="e4670-152">Response</span></span>
<span data-ttu-id="e4670-153">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e4670-153">If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e4670-154">示例</span><span class="sxs-lookup"><span data-stu-id="e4670-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="e4670-155">请求</span><span class="sxs-lookup"><span data-stu-id="e4670-155">Request</span></span>
<span data-ttu-id="e4670-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e4670-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e4670-157">响应</span><span class="sxs-lookup"><span data-stu-id="e4670-157">Response</span></span>
<span data-ttu-id="e4670-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e4670-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




