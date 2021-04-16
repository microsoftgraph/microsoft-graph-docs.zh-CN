---
title: 更新 windowsFeatureUpdateProfile
description: 更新 windowsFeatureUpdateProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8242e83025f030341c23be7f81daadf6f03fa66d
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51866179"
---
# <a name="update-windowsfeatureupdateprofile"></a><span data-ttu-id="297a1-103">更新 windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="297a1-103">Update windowsFeatureUpdateProfile</span></span>

<span data-ttu-id="297a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="297a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="297a1-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="297a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="297a1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="297a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="297a1-107">更新 [windowsFeatureUpdateProfile 对象](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="297a1-107">Update the properties of a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="297a1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="297a1-108">Prerequisites</span></span>
<span data-ttu-id="297a1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="297a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="297a1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="297a1-111">Permission type</span></span>|<span data-ttu-id="297a1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="297a1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="297a1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="297a1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="297a1-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="297a1-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="297a1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="297a1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="297a1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="297a1-116">Not supported.</span></span>|
|<span data-ttu-id="297a1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="297a1-117">Application</span></span>|<span data-ttu-id="297a1-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="297a1-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="297a1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="297a1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="297a1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="297a1-120">Request headers</span></span>
|<span data-ttu-id="297a1-121">标头</span><span class="sxs-lookup"><span data-stu-id="297a1-121">Header</span></span>|<span data-ttu-id="297a1-122">值</span><span class="sxs-lookup"><span data-stu-id="297a1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="297a1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="297a1-123">Authorization</span></span>|<span data-ttu-id="297a1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="297a1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="297a1-125">接受</span><span class="sxs-lookup"><span data-stu-id="297a1-125">Accept</span></span>|<span data-ttu-id="297a1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="297a1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="297a1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="297a1-127">Request body</span></span>
<span data-ttu-id="297a1-128">在请求正文中，提供 [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="297a1-128">In the request body, supply a JSON representation for the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

<span data-ttu-id="297a1-129">下表显示创建 [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="297a1-129">The following table shows the properties that are required when you create the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).</span></span>

|<span data-ttu-id="297a1-130">属性</span><span class="sxs-lookup"><span data-stu-id="297a1-130">Property</span></span>|<span data-ttu-id="297a1-131">类型</span><span class="sxs-lookup"><span data-stu-id="297a1-131">Type</span></span>|<span data-ttu-id="297a1-132">说明</span><span class="sxs-lookup"><span data-stu-id="297a1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="297a1-133">id</span><span class="sxs-lookup"><span data-stu-id="297a1-133">id</span></span>|<span data-ttu-id="297a1-134">String</span><span class="sxs-lookup"><span data-stu-id="297a1-134">String</span></span>|<span data-ttu-id="297a1-135">实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="297a1-135">The Identifier of the entity.</span></span>|
|<span data-ttu-id="297a1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="297a1-136">displayName</span></span>|<span data-ttu-id="297a1-137">String</span><span class="sxs-lookup"><span data-stu-id="297a1-137">String</span></span>|<span data-ttu-id="297a1-138">配置文件显示名称。</span><span class="sxs-lookup"><span data-stu-id="297a1-138">The display name of the profile.</span></span>|
|<span data-ttu-id="297a1-139">说明</span><span class="sxs-lookup"><span data-stu-id="297a1-139">description</span></span>|<span data-ttu-id="297a1-140">String</span><span class="sxs-lookup"><span data-stu-id="297a1-140">String</span></span>|<span data-ttu-id="297a1-141">由用户指定的配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="297a1-141">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="297a1-142">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="297a1-142">featureUpdateVersion</span></span>|<span data-ttu-id="297a1-143">String</span><span class="sxs-lookup"><span data-stu-id="297a1-143">String</span></span>|<span data-ttu-id="297a1-144">将部署到此配置文件所面向的设备的功能更新版本。</span><span class="sxs-lookup"><span data-stu-id="297a1-144">The feature update version that will be deployed to the devices targeted by this profile.</span></span> <span data-ttu-id="297a1-145">版本可以是任何受支持的版本，例如 1709、1803 或 1809 等。</span><span class="sxs-lookup"><span data-stu-id="297a1-145">The version could be any supported version for example 1709, 1803 or 1809 and so on.</span></span>|
|<span data-ttu-id="297a1-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="297a1-146">createdDateTime</span></span>|<span data-ttu-id="297a1-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="297a1-147">DateTimeOffset</span></span>|<span data-ttu-id="297a1-148">创建配置文件的日期时间。</span><span class="sxs-lookup"><span data-stu-id="297a1-148">The date time that the profile was created.</span></span>|
|<span data-ttu-id="297a1-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="297a1-149">lastModifiedDateTime</span></span>|<span data-ttu-id="297a1-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="297a1-150">DateTimeOffset</span></span>|<span data-ttu-id="297a1-151">上次修改配置文件的日期时间。</span><span class="sxs-lookup"><span data-stu-id="297a1-151">The date time that the profile was last modified.</span></span>|
|<span data-ttu-id="297a1-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="297a1-152">roleScopeTagIds</span></span>|<span data-ttu-id="297a1-153">String 集合</span><span class="sxs-lookup"><span data-stu-id="297a1-153">String collection</span></span>|<span data-ttu-id="297a1-154">此功能更新实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="297a1-154">List of Scope Tags for this Feature Update entity.</span></span>|
|<span data-ttu-id="297a1-155">deployableContentDisplayName</span><span class="sxs-lookup"><span data-stu-id="297a1-155">deployableContentDisplayName</span></span>|<span data-ttu-id="297a1-156">String</span><span class="sxs-lookup"><span data-stu-id="297a1-156">String</span></span>|<span data-ttu-id="297a1-157">质量显示名称配置文件可部署内容的友好解决方案</span><span class="sxs-lookup"><span data-stu-id="297a1-157">Friendly display name of the quality update profile deployable content</span></span>|
|<span data-ttu-id="297a1-158">endOfSupportDate</span><span class="sxs-lookup"><span data-stu-id="297a1-158">endOfSupportDate</span></span>|<span data-ttu-id="297a1-159">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="297a1-159">DateTimeOffset</span></span>|<span data-ttu-id="297a1-160">功能更新的上次支持日期</span><span class="sxs-lookup"><span data-stu-id="297a1-160">The last supported date for a feature update</span></span>|



## <a name="response"></a><span data-ttu-id="297a1-161">响应</span><span class="sxs-lookup"><span data-stu-id="297a1-161">Response</span></span>
<span data-ttu-id="297a1-162">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="297a1-162">If successful, this method returns a `200 OK` response code and an updated [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="297a1-163">示例</span><span class="sxs-lookup"><span data-stu-id="297a1-163">Example</span></span>

### <a name="request"></a><span data-ttu-id="297a1-164">请求</span><span class="sxs-lookup"><span data-stu-id="297a1-164">Request</span></span>
<span data-ttu-id="297a1-165">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="297a1-165">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
Content-type: application/json
Content-length: 405

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "deployableContentDisplayName": "Deployable Content Display Name value",
  "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00"
}
```

### <a name="response"></a><span data-ttu-id="297a1-166">响应</span><span class="sxs-lookup"><span data-stu-id="297a1-166">Response</span></span>
<span data-ttu-id="297a1-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="297a1-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 577

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "id": "885bd4ee-d4ee-885b-eed4-5b88eed45b88",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ],
  "deployableContentDisplayName": "Deployable Content Display Name value",
  "endOfSupportDate": "2017-01-01T00:02:08.3437725-08:00"
}
```




