---
title: 创建 windowsFeatureUpdateProfile
description: 创建新的 windowsFeatureUpdateProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b2f5b68a0cb3f2773b2ea6ab933cbf341515811e
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45124007"
---
# <a name="create-windowsfeatureupdateprofile"></a><span data-ttu-id="2ba45-103">创建 windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="2ba45-103">Create windowsFeatureUpdateProfile</span></span>

<span data-ttu-id="2ba45-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ba45-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2ba45-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2ba45-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2ba45-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2ba45-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ba45-107">创建新的[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2ba45-107">Create a new [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ba45-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2ba45-108">Prerequisites</span></span>
<span data-ttu-id="2ba45-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="2ba45-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="2ba45-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="2ba45-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ba45-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ba45-111">Permission type</span></span>|<span data-ttu-id="2ba45-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2ba45-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ba45-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ba45-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ba45-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ba45-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2ba45-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ba45-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ba45-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ba45-116">Not supported.</span></span>|
|<span data-ttu-id="2ba45-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ba45-117">Application</span></span>|<span data-ttu-id="2ba45-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ba45-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ba45-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ba45-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsFeatureUpdateProfiles
```

## <a name="request-headers"></a><span data-ttu-id="2ba45-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ba45-120">Request headers</span></span>
|<span data-ttu-id="2ba45-121">标头</span><span class="sxs-lookup"><span data-stu-id="2ba45-121">Header</span></span>|<span data-ttu-id="2ba45-122">值</span><span class="sxs-lookup"><span data-stu-id="2ba45-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ba45-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ba45-123">Authorization</span></span>|<span data-ttu-id="2ba45-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2ba45-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ba45-125">接受</span><span class="sxs-lookup"><span data-stu-id="2ba45-125">Accept</span></span>|<span data-ttu-id="2ba45-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ba45-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ba45-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ba45-127">Request body</span></span>
<span data-ttu-id="2ba45-128">在请求正文中，提供 windowsFeatureUpdateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ba45-128">In the request body, supply a JSON representation for the windowsFeatureUpdateProfile object.</span></span>

<span data-ttu-id="2ba45-129">下表显示创建 windowsFeatureUpdateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2ba45-129">The following table shows the properties that are required when you create the windowsFeatureUpdateProfile.</span></span>

|<span data-ttu-id="2ba45-130">属性</span><span class="sxs-lookup"><span data-stu-id="2ba45-130">Property</span></span>|<span data-ttu-id="2ba45-131">类型</span><span class="sxs-lookup"><span data-stu-id="2ba45-131">Type</span></span>|<span data-ttu-id="2ba45-132">说明</span><span class="sxs-lookup"><span data-stu-id="2ba45-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ba45-133">id</span><span class="sxs-lookup"><span data-stu-id="2ba45-133">id</span></span>|<span data-ttu-id="2ba45-134">字符串</span><span class="sxs-lookup"><span data-stu-id="2ba45-134">String</span></span>|<span data-ttu-id="2ba45-135">实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="2ba45-135">The Identifier of the entity.</span></span>|
|<span data-ttu-id="2ba45-136">displayName</span><span class="sxs-lookup"><span data-stu-id="2ba45-136">displayName</span></span>|<span data-ttu-id="2ba45-137">String</span><span class="sxs-lookup"><span data-stu-id="2ba45-137">String</span></span>|<span data-ttu-id="2ba45-138">配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2ba45-138">The display name of the profile.</span></span>|
|<span data-ttu-id="2ba45-139">说明</span><span class="sxs-lookup"><span data-stu-id="2ba45-139">description</span></span>|<span data-ttu-id="2ba45-140">String</span><span class="sxs-lookup"><span data-stu-id="2ba45-140">String</span></span>|<span data-ttu-id="2ba45-141">用户指定的配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="2ba45-141">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="2ba45-142">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="2ba45-142">featureUpdateVersion</span></span>|<span data-ttu-id="2ba45-143">String</span><span class="sxs-lookup"><span data-stu-id="2ba45-143">String</span></span>|<span data-ttu-id="2ba45-144">将部署到此配置文件目标的设备的功能更新版本。</span><span class="sxs-lookup"><span data-stu-id="2ba45-144">The feature update version that will be deployed to the devices targeted by this profile.</span></span> <span data-ttu-id="2ba45-145">版本可以是任何受支持的版本，例如，1709、1803或1809等。</span><span class="sxs-lookup"><span data-stu-id="2ba45-145">The version could be any supported version for example 1709, 1803 or 1809 and so on.</span></span>|
|<span data-ttu-id="2ba45-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2ba45-146">createdDateTime</span></span>|<span data-ttu-id="2ba45-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ba45-147">DateTimeOffset</span></span>|<span data-ttu-id="2ba45-148">创建配置文件的日期时间。</span><span class="sxs-lookup"><span data-stu-id="2ba45-148">The date time that the profile was created.</span></span>|
|<span data-ttu-id="2ba45-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ba45-149">lastModifiedDateTime</span></span>|<span data-ttu-id="2ba45-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ba45-150">DateTimeOffset</span></span>|<span data-ttu-id="2ba45-151">上次修改配置文件的日期时间。</span><span class="sxs-lookup"><span data-stu-id="2ba45-151">The date time that the profile was last modified.</span></span>|
|<span data-ttu-id="2ba45-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="2ba45-152">roleScopeTagIds</span></span>|<span data-ttu-id="2ba45-153">String collection</span><span class="sxs-lookup"><span data-stu-id="2ba45-153">String collection</span></span>|<span data-ttu-id="2ba45-154">此功能更新实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="2ba45-154">List of Scope Tags for this Feature Update entity.</span></span>|



## <a name="response"></a><span data-ttu-id="2ba45-155">响应</span><span class="sxs-lookup"><span data-stu-id="2ba45-155">Response</span></span>
<span data-ttu-id="2ba45-156">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2ba45-156">If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2ba45-157">示例</span><span class="sxs-lookup"><span data-stu-id="2ba45-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ba45-158">请求</span><span class="sxs-lookup"><span data-stu-id="2ba45-158">Request</span></span>
<span data-ttu-id="2ba45-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2ba45-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles
Content-type: application/json
Content-length: 269

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value",
  "roleScopeTagIds": [
    "Role Scope Tag Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="2ba45-160">响应</span><span class="sxs-lookup"><span data-stu-id="2ba45-160">Response</span></span>
<span data-ttu-id="2ba45-161">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="2ba45-161">Here is an example of the response.</span></span> <span data-ttu-id="2ba45-162">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="2ba45-162">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="2ba45-163">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="2ba45-163">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 441

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
  ]
}
```



