---
title: 更新 windowsFeatureUpdateProfile
description: 更新 windowsFeatureUpdateProfile 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 230d2dc672a1f0c24caa712eba77e0cd595dc12d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49295759"
---
# <a name="update-windowsfeatureupdateprofile"></a><span data-ttu-id="809c6-103">更新 windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="809c6-103">Update windowsFeatureUpdateProfile</span></span>

<span data-ttu-id="809c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="809c6-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="809c6-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="809c6-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="809c6-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="809c6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="809c6-107">更新 [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="809c6-107">Update the properties of a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="809c6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="809c6-108">Prerequisites</span></span>
<span data-ttu-id="809c6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="809c6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="809c6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="809c6-111">Permission type</span></span>|<span data-ttu-id="809c6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="809c6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="809c6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="809c6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="809c6-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="809c6-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="809c6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="809c6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="809c6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="809c6-116">Not supported.</span></span>|
|<span data-ttu-id="809c6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="809c6-117">Application</span></span>|<span data-ttu-id="809c6-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="809c6-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="809c6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="809c6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="809c6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="809c6-120">Request headers</span></span>
|<span data-ttu-id="809c6-121">标头</span><span class="sxs-lookup"><span data-stu-id="809c6-121">Header</span></span>|<span data-ttu-id="809c6-122">值</span><span class="sxs-lookup"><span data-stu-id="809c6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="809c6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="809c6-123">Authorization</span></span>|<span data-ttu-id="809c6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="809c6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="809c6-125">接受</span><span class="sxs-lookup"><span data-stu-id="809c6-125">Accept</span></span>|<span data-ttu-id="809c6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="809c6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="809c6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="809c6-127">Request body</span></span>
<span data-ttu-id="809c6-128">在请求正文中，提供 [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="809c6-128">In the request body, supply a JSON representation for the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

<span data-ttu-id="809c6-129">下表显示创建 [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="809c6-129">The following table shows the properties that are required when you create the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md).</span></span>

|<span data-ttu-id="809c6-130">属性</span><span class="sxs-lookup"><span data-stu-id="809c6-130">Property</span></span>|<span data-ttu-id="809c6-131">类型</span><span class="sxs-lookup"><span data-stu-id="809c6-131">Type</span></span>|<span data-ttu-id="809c6-132">说明</span><span class="sxs-lookup"><span data-stu-id="809c6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="809c6-133">id</span><span class="sxs-lookup"><span data-stu-id="809c6-133">id</span></span>|<span data-ttu-id="809c6-134">字符串</span><span class="sxs-lookup"><span data-stu-id="809c6-134">String</span></span>|<span data-ttu-id="809c6-135">实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="809c6-135">The Identifier of the entity.</span></span>|
|<span data-ttu-id="809c6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="809c6-136">displayName</span></span>|<span data-ttu-id="809c6-137">字符串</span><span class="sxs-lookup"><span data-stu-id="809c6-137">String</span></span>|<span data-ttu-id="809c6-138">配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="809c6-138">The display name of the profile.</span></span>|
|<span data-ttu-id="809c6-139">description</span><span class="sxs-lookup"><span data-stu-id="809c6-139">description</span></span>|<span data-ttu-id="809c6-140">字符串</span><span class="sxs-lookup"><span data-stu-id="809c6-140">String</span></span>|<span data-ttu-id="809c6-141">用户指定的配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="809c6-141">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="809c6-142">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="809c6-142">featureUpdateVersion</span></span>|<span data-ttu-id="809c6-143">字符串</span><span class="sxs-lookup"><span data-stu-id="809c6-143">String</span></span>|<span data-ttu-id="809c6-144">将部署到此配置文件目标的设备的功能更新版本。</span><span class="sxs-lookup"><span data-stu-id="809c6-144">The feature update version that will be deployed to the devices targeted by this profile.</span></span> <span data-ttu-id="809c6-145">版本可以是任何受支持的版本，例如，1709、1803或1809等。</span><span class="sxs-lookup"><span data-stu-id="809c6-145">The version could be any supported version for example 1709, 1803 or 1809 and so on.</span></span>|
|<span data-ttu-id="809c6-146">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="809c6-146">createdDateTime</span></span>|<span data-ttu-id="809c6-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="809c6-147">DateTimeOffset</span></span>|<span data-ttu-id="809c6-148">创建配置文件的日期时间。</span><span class="sxs-lookup"><span data-stu-id="809c6-148">The date time that the profile was created.</span></span>|
|<span data-ttu-id="809c6-149">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="809c6-149">lastModifiedDateTime</span></span>|<span data-ttu-id="809c6-150">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="809c6-150">DateTimeOffset</span></span>|<span data-ttu-id="809c6-151">上次修改配置文件的日期时间。</span><span class="sxs-lookup"><span data-stu-id="809c6-151">The date time that the profile was last modified.</span></span>|
|<span data-ttu-id="809c6-152">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="809c6-152">roleScopeTagIds</span></span>|<span data-ttu-id="809c6-153">String 集合</span><span class="sxs-lookup"><span data-stu-id="809c6-153">String collection</span></span>|<span data-ttu-id="809c6-154">此功能更新实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="809c6-154">List of Scope Tags for this Feature Update entity.</span></span>|



## <a name="response"></a><span data-ttu-id="809c6-155">响应</span><span class="sxs-lookup"><span data-stu-id="809c6-155">Response</span></span>
<span data-ttu-id="809c6-156">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="809c6-156">If successful, this method returns a `200 OK` response code and an updated [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="809c6-157">示例</span><span class="sxs-lookup"><span data-stu-id="809c6-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="809c6-158">请求</span><span class="sxs-lookup"><span data-stu-id="809c6-158">Request</span></span>
<span data-ttu-id="809c6-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="809c6-159">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
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

### <a name="response"></a><span data-ttu-id="809c6-160">响应</span><span class="sxs-lookup"><span data-stu-id="809c6-160">Response</span></span>
<span data-ttu-id="809c6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="809c6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




