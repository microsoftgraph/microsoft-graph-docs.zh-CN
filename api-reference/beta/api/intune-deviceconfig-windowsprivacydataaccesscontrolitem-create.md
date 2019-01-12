---
title: 创建 windowsPrivacyDataAccessControlItem
description: 创建新的 windowsPrivacyDataAccessControlItem 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 3ec9aa9f4b8351c4f64ce468027f1f46e7d139a2
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27948931"
---
# <a name="create-windowsprivacydataaccesscontrolitem"></a><span data-ttu-id="ab471-103">创建 windowsPrivacyDataAccessControlItem</span><span class="sxs-lookup"><span data-stu-id="ab471-103">Create windowsPrivacyDataAccessControlItem</span></span>

> <span data-ttu-id="ab471-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ab471-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ab471-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ab471-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ab471-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ab471-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ab471-107">创建新的[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ab471-107">Create a new [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ab471-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ab471-108">Prerequisites</span></span>
<span data-ttu-id="ab471-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ab471-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ab471-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ab471-111">Permission type</span></span>|<span data-ttu-id="ab471-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ab471-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ab471-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ab471-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ab471-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ab471-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ab471-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ab471-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ab471-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab471-116">Not supported.</span></span>|
|<span data-ttu-id="ab471-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ab471-117">Application</span></span>|<span data-ttu-id="ab471-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ab471-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ab471-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ab471-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/privacyAccessControls
```

## <a name="request-headers"></a><span data-ttu-id="ab471-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ab471-120">Request headers</span></span>
|<span data-ttu-id="ab471-121">标头</span><span class="sxs-lookup"><span data-stu-id="ab471-121">Header</span></span>|<span data-ttu-id="ab471-122">值</span><span class="sxs-lookup"><span data-stu-id="ab471-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ab471-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ab471-123">Authorization</span></span>|<span data-ttu-id="ab471-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ab471-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ab471-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ab471-125">Accept</span></span>|<span data-ttu-id="ab471-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ab471-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ab471-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ab471-127">Request body</span></span>
<span data-ttu-id="ab471-128">在请求正文中，提供 windowsPrivacyDataAccessControlItem 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ab471-128">In the request body, supply a JSON representation for the windowsPrivacyDataAccessControlItem object.</span></span>

<span data-ttu-id="ab471-129">下表显示时创建 windowsPrivacyDataAccessControlItem 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ab471-129">The following table shows the properties that are required when you create the windowsPrivacyDataAccessControlItem.</span></span>

|<span data-ttu-id="ab471-130">属性</span><span class="sxs-lookup"><span data-stu-id="ab471-130">Property</span></span>|<span data-ttu-id="ab471-131">类型</span><span class="sxs-lookup"><span data-stu-id="ab471-131">Type</span></span>|<span data-ttu-id="ab471-132">说明</span><span class="sxs-lookup"><span data-stu-id="ab471-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ab471-133">id</span><span class="sxs-lookup"><span data-stu-id="ab471-133">id</span></span>|<span data-ttu-id="ab471-134">字符串</span><span class="sxs-lookup"><span data-stu-id="ab471-134">String</span></span>|<span data-ttu-id="ab471-135">WindowsPrivacyDataAccessControlItem 键。</span><span class="sxs-lookup"><span data-stu-id="ab471-135">The key of WindowsPrivacyDataAccessControlItem.</span></span>|
|<span data-ttu-id="ab471-136">accessLevel</span><span class="sxs-lookup"><span data-stu-id="ab471-136">accessLevel</span></span>|[<span data-ttu-id="ab471-137">windowsPrivacyDataAccessLevel</span><span class="sxs-lookup"><span data-stu-id="ab471-137">windowsPrivacyDataAccessLevel</span></span>](../resources/intune-deviceconfig-windowsprivacydataaccesslevel.md)|<span data-ttu-id="ab471-138">这指示到指定的应用程序会授予对隐私数据类别的访问级别。</span><span class="sxs-lookup"><span data-stu-id="ab471-138">This indicates an access level for the privacy data category to which the specified application will be given to.</span></span> <span data-ttu-id="ab471-139">可取值为：`notConfigured`、`forceAllow`、`forceDeny`、`userInControl`。</span><span class="sxs-lookup"><span data-stu-id="ab471-139">Possible values are: `notConfigured`, `forceAllow`, `forceDeny`, `userInControl`.</span></span>|
|<span data-ttu-id="ab471-140">dataCategory</span><span class="sxs-lookup"><span data-stu-id="ab471-140">dataCategory</span></span>|[<span data-ttu-id="ab471-141">windowsPrivacyDataCategory</span><span class="sxs-lookup"><span data-stu-id="ab471-141">windowsPrivacyDataCategory</span></span>](../resources/intune-deviceconfig-windowsprivacydatacategory.md)|<span data-ttu-id="ab471-142">这指示特定的访问控制将应用于哪个隐私数据类别。</span><span class="sxs-lookup"><span data-stu-id="ab471-142">This indicates a privacy data category to which the specific access control will apply.</span></span> <span data-ttu-id="ab471-143">可能的值为： `notConfigured`， `accountInfo`， `appsRunInBackground`， `calendar`， `callHistory`， `camera`， `contacts`， `diagnosticsInfo`， `email`， `location`， `messaging`， `microphone`， `motion`， `notifications`， `phone`， `radios`， `tasks`， `syncWithDevices`， `trustedDevices`.</span><span class="sxs-lookup"><span data-stu-id="ab471-143">Possible values are: `notConfigured`, `accountInfo`, `appsRunInBackground`, `calendar`, `callHistory`, `camera`, `contacts`, `diagnosticsInfo`, `email`, `location`, `messaging`, `microphone`, `motion`, `notifications`, `phone`, `radios`, `tasks`, `syncWithDevices`, `trustedDevices`.</span></span>|
|<span data-ttu-id="ab471-144">appPackageFamilyName</span><span class="sxs-lookup"><span data-stu-id="ab471-144">appPackageFamilyName</span></span>|<span data-ttu-id="ab471-145">字符串</span><span class="sxs-lookup"><span data-stu-id="ab471-145">String</span></span>|<span data-ttu-id="ab471-146">包系列 Windows 应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="ab471-146">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="ab471-147">设置时，访问级别应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="ab471-147">When set, the access level applies to the specified application.</span></span>|
|<span data-ttu-id="ab471-148">appDisplayName</span><span class="sxs-lookup"><span data-stu-id="ab471-148">appDisplayName</span></span>|<span data-ttu-id="ab471-149">字符串</span><span class="sxs-lookup"><span data-stu-id="ab471-149">String</span></span>|<span data-ttu-id="ab471-150">包系列 Windows 应用程序的名称。</span><span class="sxs-lookup"><span data-stu-id="ab471-150">The Package Family Name of a Windows app.</span></span> <span data-ttu-id="ab471-151">设置时，访问级别应用于指定的应用程序。</span><span class="sxs-lookup"><span data-stu-id="ab471-151">When set, the access level applies to the specified application.</span></span>|



## <a name="response"></a><span data-ttu-id="ab471-152">响应</span><span class="sxs-lookup"><span data-stu-id="ab471-152">Response</span></span>
<span data-ttu-id="ab471-153">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ab471-153">If successful, this method returns a `201 Created` response code and a [windowsPrivacyDataAccessControlItem](../resources/intune-deviceconfig-windowsprivacydataaccesscontrolitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ab471-154">示例</span><span class="sxs-lookup"><span data-stu-id="ab471-154">Example</span></span>
### <a name="request"></a><span data-ttu-id="ab471-155">请求</span><span class="sxs-lookup"><span data-stu-id="ab471-155">Request</span></span>
<span data-ttu-id="ab471-156">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ab471-156">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ab471-157">响应</span><span class="sxs-lookup"><span data-stu-id="ab471-157">Response</span></span>
<span data-ttu-id="ab471-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ab471-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





