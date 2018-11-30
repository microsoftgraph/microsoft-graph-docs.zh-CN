---
title: 更新 windowsAssignedAccessProfile
description: 更新 windowsAssignedAccessProfile 对象的属性。
ms.openlocfilehash: bbe3aab584ff19af07728d4ebe594238ef8439f9
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27043769"
---
# <a name="update-windowsassignedaccessprofile"></a><span data-ttu-id="6eb29-103">更新 windowsAssignedAccessProfile</span><span class="sxs-lookup"><span data-stu-id="6eb29-103">Update windowsAssignedAccessProfile</span></span>

> <span data-ttu-id="6eb29-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6eb29-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6eb29-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6eb29-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="6eb29-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="6eb29-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6eb29-107">更新[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6eb29-107">Update the properties of a [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="6eb29-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6eb29-108">Prerequisites</span></span>
<span data-ttu-id="6eb29-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="6eb29-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6eb29-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6eb29-111">Permission type</span></span>|<span data-ttu-id="6eb29-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6eb29-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6eb29-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6eb29-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6eb29-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6eb29-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6eb29-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6eb29-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6eb29-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6eb29-116">Not supported.</span></span>|
|<span data-ttu-id="6eb29-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6eb29-117">Application</span></span>|<span data-ttu-id="6eb29-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="6eb29-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6eb29-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6eb29-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles/{windowsAssignedAccessProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="6eb29-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6eb29-120">Request headers</span></span>
|<span data-ttu-id="6eb29-121">标头</span><span class="sxs-lookup"><span data-stu-id="6eb29-121">Header</span></span>|<span data-ttu-id="6eb29-122">值</span><span class="sxs-lookup"><span data-stu-id="6eb29-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6eb29-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6eb29-123">Authorization</span></span>|<span data-ttu-id="6eb29-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6eb29-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6eb29-125">Accept</span><span class="sxs-lookup"><span data-stu-id="6eb29-125">Accept</span></span>|<span data-ttu-id="6eb29-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6eb29-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6eb29-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6eb29-127">Request body</span></span>
<span data-ttu-id="6eb29-128">在请求正文中，提供[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6eb29-128">In the request body, supply a JSON representation for the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object.</span></span>

<span data-ttu-id="6eb29-129">下表显示时创建[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6eb29-129">The following table shows the properties that are required when you create the [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md).</span></span>

|<span data-ttu-id="6eb29-130">属性</span><span class="sxs-lookup"><span data-stu-id="6eb29-130">Property</span></span>|<span data-ttu-id="6eb29-131">类型</span><span class="sxs-lookup"><span data-stu-id="6eb29-131">Type</span></span>|<span data-ttu-id="6eb29-132">说明</span><span class="sxs-lookup"><span data-stu-id="6eb29-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6eb29-133">id</span><span class="sxs-lookup"><span data-stu-id="6eb29-133">id</span></span>|<span data-ttu-id="6eb29-134">String</span><span class="sxs-lookup"><span data-stu-id="6eb29-134">String</span></span>|<span data-ttu-id="6eb29-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="6eb29-135">Key of the entity.</span></span>|
|<span data-ttu-id="6eb29-136">profileName</span><span class="sxs-lookup"><span data-stu-id="6eb29-136">profileName</span></span>|<span data-ttu-id="6eb29-137">字符串</span><span class="sxs-lookup"><span data-stu-id="6eb29-137">String</span></span>|<span data-ttu-id="6eb29-138">这是用于标识一组应用程序，在开始菜单和用户为其分配此网亭配置这些应用程序的布局的友好名称。</span><span class="sxs-lookup"><span data-stu-id="6eb29-138">This is a friendly name used to identify a group of applications, the layout of these apps on the start menu and the users to whom this kiosk configuration is assigned.</span></span>|
|<span data-ttu-id="6eb29-139">showTaskBar</span><span class="sxs-lookup"><span data-stu-id="6eb29-139">showTaskBar</span></span>|<span data-ttu-id="6eb29-140">布尔</span><span class="sxs-lookup"><span data-stu-id="6eb29-140">Boolean</span></span>|<span data-ttu-id="6eb29-141">此设置，管理员可以指定任务条形图或不所示。</span><span class="sxs-lookup"><span data-stu-id="6eb29-141">This setting allows the admin to specify whether the Task Bar is shown or not.</span></span>|
|<span data-ttu-id="6eb29-142">appUserModelIds</span><span class="sxs-lookup"><span data-stu-id="6eb29-142">appUserModelIds</span></span>|<span data-ttu-id="6eb29-143">String 集合</span><span class="sxs-lookup"><span data-stu-id="6eb29-143">String collection</span></span>|<span data-ttu-id="6eb29-144">这些是唯一的 Windows 应用商店应用程序将可以从开始菜单启动。</span><span class="sxs-lookup"><span data-stu-id="6eb29-144">These are the only Windows Store Apps that will be available to launch from the Start menu.</span></span>|
|<span data-ttu-id="6eb29-145">desktopAppPaths</span><span class="sxs-lookup"><span data-stu-id="6eb29-145">desktopAppPaths</span></span>|<span data-ttu-id="6eb29-146">String 集合</span><span class="sxs-lookup"><span data-stu-id="6eb29-146">String collection</span></span>|<span data-ttu-id="6eb29-147">在开始菜单可用桌面应用程序的路径和仅应用程序用户都将能够启动。</span><span class="sxs-lookup"><span data-stu-id="6eb29-147">These are the paths of the Desktop Apps that will be available on the Start menu and the only apps the user will be able to launch.</span></span>|
|<span data-ttu-id="6eb29-148">用户帐户</span><span class="sxs-lookup"><span data-stu-id="6eb29-148">userAccounts</span></span>|<span data-ttu-id="6eb29-149">String 集合</span><span class="sxs-lookup"><span data-stu-id="6eb29-149">String collection</span></span>|<span data-ttu-id="6eb29-150">将锁定到此网亭配置用户帐户。</span><span class="sxs-lookup"><span data-stu-id="6eb29-150">The user accounts that will be locked to this kiosk configuration.</span></span>|
|<span data-ttu-id="6eb29-151">startMenuLayoutXml</span><span class="sxs-lookup"><span data-stu-id="6eb29-151">startMenuLayoutXml</span></span>|<span data-ttu-id="6eb29-152">Binary</span><span class="sxs-lookup"><span data-stu-id="6eb29-152">Binary</span></span>|<span data-ttu-id="6eb29-153">允许管理员可以重写默认开始布局，并禁止用户更改它。</span><span class="sxs-lookup"><span data-stu-id="6eb29-153">Allows admins to override the default Start layout and prevents the user from changing it.</span></span><span data-ttu-id="6eb29-154">通过基于布局修改模式指定 XML 文件来修改布局。</span><span class="sxs-lookup"><span data-stu-id="6eb29-154"> The layout is modified by specifying an XML file based on a layout modification schema.</span></span> <span data-ttu-id="6eb29-155">XML 需要以二进制格式。</span><span class="sxs-lookup"><span data-stu-id="6eb29-155">XML needs to be in Binary format.</span></span>|



## <a name="response"></a><span data-ttu-id="6eb29-156">响应</span><span class="sxs-lookup"><span data-stu-id="6eb29-156">Response</span></span>
<span data-ttu-id="6eb29-157">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6eb29-157">If successful, this method returns a `200 OK` response code and an updated [windowsAssignedAccessProfile](../resources/intune-deviceconfig-windowsassignedaccessprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6eb29-158">示例</span><span class="sxs-lookup"><span data-stu-id="6eb29-158">Example</span></span>
### <a name="request"></a><span data-ttu-id="6eb29-159">请求</span><span class="sxs-lookup"><span data-stu-id="6eb29-159">Request</span></span>
<span data-ttu-id="6eb29-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6eb29-160">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windows10GeneralConfiguration/assignedAccessMultiModeProfiles/{windowsAssignedAccessProfileId}
Content-type: application/json
Content-length: 297

{
  "profileName": "Profile Name value",
  "showTaskBar": true,
  "appUserModelIds": [
    "App User Model Ids value"
  ],
  "desktopAppPaths": [
    "Desktop App Paths value"
  ],
  "userAccounts": [
    "User Accounts value"
  ],
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
}
```

### <a name="response"></a><span data-ttu-id="6eb29-161">响应</span><span class="sxs-lookup"><span data-stu-id="6eb29-161">Response</span></span>
<span data-ttu-id="6eb29-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6eb29-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 413

{
  "@odata.type": "#microsoft.graph.windowsAssignedAccessProfile",
  "id": "cfa70299-0299-cfa7-9902-a7cf9902a7cf",
  "profileName": "Profile Name value",
  "showTaskBar": true,
  "appUserModelIds": [
    "App User Model Ids value"
  ],
  "desktopAppPaths": [
    "Desktop App Paths value"
  ],
  "userAccounts": [
    "User Accounts value"
  ],
  "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
}
```





