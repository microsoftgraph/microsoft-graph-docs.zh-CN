---
title: 更新 windowsQualityUpdateProfile
description: 更新 windowsQualityUpdateProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 62932ae10bc64ecf63ece2648527d7babad8731e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156175"
---
# <a name="update-windowsqualityupdateprofile"></a><span data-ttu-id="0735c-103">更新 windowsQualityUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="0735c-103">Update windowsQualityUpdateProfile</span></span>

<span data-ttu-id="0735c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0735c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0735c-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0735c-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0735c-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0735c-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0735c-107">更新 [windowsQualityUpdateProfile 对象](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="0735c-107">Update the properties of a [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0735c-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0735c-108">Prerequisites</span></span>
<span data-ttu-id="0735c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0735c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0735c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0735c-111">Permission type</span></span>|<span data-ttu-id="0735c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0735c-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0735c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0735c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0735c-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0735c-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0735c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0735c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0735c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0735c-116">Not supported.</span></span>|
|<span data-ttu-id="0735c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0735c-117">Application</span></span>|<span data-ttu-id="0735c-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0735c-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0735c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0735c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="0735c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0735c-120">Request headers</span></span>
|<span data-ttu-id="0735c-121">标头</span><span class="sxs-lookup"><span data-stu-id="0735c-121">Header</span></span>|<span data-ttu-id="0735c-122">值</span><span class="sxs-lookup"><span data-stu-id="0735c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0735c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="0735c-123">Authorization</span></span>|<span data-ttu-id="0735c-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0735c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0735c-125">接受</span><span class="sxs-lookup"><span data-stu-id="0735c-125">Accept</span></span>|<span data-ttu-id="0735c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0735c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0735c-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0735c-127">Request body</span></span>
<span data-ttu-id="0735c-128">在请求正文中，提供 [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0735c-128">In the request body, supply a JSON representation for the [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object.</span></span>

<span data-ttu-id="0735c-129">下表显示创建 [windowsQualityUpdateProfile 时所需的属性](../resources/intune-softwareupdate-windowsqualityupdateprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="0735c-129">The following table shows the properties that are required when you create the [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md).</span></span>

|<span data-ttu-id="0735c-130">属性</span><span class="sxs-lookup"><span data-stu-id="0735c-130">Property</span></span>|<span data-ttu-id="0735c-131">类型</span><span class="sxs-lookup"><span data-stu-id="0735c-131">Type</span></span>|<span data-ttu-id="0735c-132">说明</span><span class="sxs-lookup"><span data-stu-id="0735c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0735c-133">id</span><span class="sxs-lookup"><span data-stu-id="0735c-133">id</span></span>|<span data-ttu-id="0735c-134">String</span><span class="sxs-lookup"><span data-stu-id="0735c-134">String</span></span>|<span data-ttu-id="0735c-135">Intune 策略 ID。</span><span class="sxs-lookup"><span data-stu-id="0735c-135">The Intune policy id.</span></span>|
|<span data-ttu-id="0735c-136">displayName</span><span class="sxs-lookup"><span data-stu-id="0735c-136">displayName</span></span>|<span data-ttu-id="0735c-137">String</span><span class="sxs-lookup"><span data-stu-id="0735c-137">String</span></span>|<span data-ttu-id="0735c-138">配置文件显示名称的配置文件。</span><span class="sxs-lookup"><span data-stu-id="0735c-138">The display name for the profile.</span></span>|
|<span data-ttu-id="0735c-139">说明</span><span class="sxs-lookup"><span data-stu-id="0735c-139">description</span></span>|<span data-ttu-id="0735c-140">String</span><span class="sxs-lookup"><span data-stu-id="0735c-140">String</span></span>|<span data-ttu-id="0735c-141">由用户指定的配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="0735c-141">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="0735c-142">expeditedUpdateSettings</span><span class="sxs-lookup"><span data-stu-id="0735c-142">expeditedUpdateSettings</span></span>|[<span data-ttu-id="0735c-143">expeditedWindowsQualityUpdateSettings</span><span class="sxs-lookup"><span data-stu-id="0735c-143">expeditedWindowsQualityUpdateSettings</span></span>](../resources/intune-softwareupdate-expeditedwindowsqualityupdatesettings.md)|<span data-ttu-id="0735c-144">加速更新设置。</span><span class="sxs-lookup"><span data-stu-id="0735c-144">Expedited update settings.</span></span>|
|<span data-ttu-id="0735c-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="0735c-145">createdDateTime</span></span>|<span data-ttu-id="0735c-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0735c-146">DateTimeOffset</span></span>|<span data-ttu-id="0735c-147">创建配置文件的日期时间。</span><span class="sxs-lookup"><span data-stu-id="0735c-147">The date time that the profile was created.</span></span>|
|<span data-ttu-id="0735c-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="0735c-148">lastModifiedDateTime</span></span>|<span data-ttu-id="0735c-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="0735c-149">DateTimeOffset</span></span>|<span data-ttu-id="0735c-150">上次修改配置文件的日期时间。</span><span class="sxs-lookup"><span data-stu-id="0735c-150">The date time that the profile was last modified.</span></span>|
|<span data-ttu-id="0735c-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="0735c-151">roleScopeTagIds</span></span>|<span data-ttu-id="0735c-152">String collection</span><span class="sxs-lookup"><span data-stu-id="0735c-152">String collection</span></span>|<span data-ttu-id="0735c-153">此质量更新实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="0735c-153">List of Scope Tags for this Quality Update entity.</span></span>|
|<span data-ttu-id="0735c-154">releaseDateDisplayName</span><span class="sxs-lookup"><span data-stu-id="0735c-154">releaseDateDisplayName</span></span>|<span data-ttu-id="0735c-155">String</span><span class="sxs-lookup"><span data-stu-id="0735c-155">String</span></span>|<span data-ttu-id="0735c-156">为质量更新版本显示的友好发布日期</span><span class="sxs-lookup"><span data-stu-id="0735c-156">Friendly release date to display for a Quality Update release</span></span>|
|<span data-ttu-id="0735c-157">deployableContentDisplayName</span><span class="sxs-lookup"><span data-stu-id="0735c-157">deployableContentDisplayName</span></span>|<span data-ttu-id="0735c-158">String</span><span class="sxs-lookup"><span data-stu-id="0735c-158">String</span></span>|<span data-ttu-id="0735c-159">质量显示名称配置文件可部署内容的友好解决方案</span><span class="sxs-lookup"><span data-stu-id="0735c-159">Friendly display name of the quality update profile deployable content</span></span>|



## <a name="response"></a><span data-ttu-id="0735c-160">响应</span><span class="sxs-lookup"><span data-stu-id="0735c-160">Response</span></span>
<span data-ttu-id="0735c-161">如果成功，此方法在响应正文中返回 响应代码和更新 `200 OK` 的 [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0735c-161">If successful, this method returns a `200 OK` response code and an updated [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0735c-162">示例</span><span class="sxs-lookup"><span data-stu-id="0735c-162">Example</span></span>

### <a name="request"></a><span data-ttu-id="0735c-163">请求</span><span class="sxs-lookup"><span data-stu-id="0735c-163">Request</span></span>
<span data-ttu-id="0735c-164">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0735c-164">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsQualityUpdateProfiles/{windowsQualityUpdateProfileId}
Content-type: application/json
Content-length: 558

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "expeditedUpdateSettings": {
    "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings",
    "qualityUpdateRelease": "Quality Update Release value",
    "daysUntilForcedReboot": 5
  },
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "releaseDateDisplayName": "Release Date Display Name value",
  "deployableContentDisplayName": "Deployable Content Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="0735c-165">响应</span><span class="sxs-lookup"><span data-stu-id="0735c-165">Response</span></span>
<span data-ttu-id="0735c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0735c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 730

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateProfile",
  "id": "76fc7b65-7b65-76fc-657b-fc76657bfc76",
  "displayName": "Display Name value",
  "description": "Description value",
  "expeditedUpdateSettings": {
    "@odata.type": "microsoft.graph.expeditedWindowsQualityUpdateSettings",
    "qualityUpdateRelease": "Quality Update Release value",
    "daysUntilForcedReboot": 5
  },
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "releaseDateDisplayName": "Release Date Display Name value",
  "deployableContentDisplayName": "Deployable Content Display Name value"
}
```




