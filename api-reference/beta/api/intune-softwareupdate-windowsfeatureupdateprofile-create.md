---
title: 创建 windowsFeatureUpdateProfile
description: 创建新的 windowsFeatureUpdateProfile 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: ac07264c3f0bfd8b99537882025e18be1a38f25a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37199834"
---
# <a name="create-windowsfeatureupdateprofile"></a><span data-ttu-id="d6e68-103">创建 windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="d6e68-103">Create windowsFeatureUpdateProfile</span></span>

> <span data-ttu-id="d6e68-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d6e68-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6e68-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d6e68-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6e68-106">创建新的[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d6e68-106">Create a new [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6e68-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d6e68-107">Prerequisites</span></span>
<span data-ttu-id="d6e68-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6e68-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6e68-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6e68-110">Permission type</span></span>|<span data-ttu-id="d6e68-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d6e68-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6e68-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6e68-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6e68-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6e68-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d6e68-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6e68-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6e68-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6e68-115">Not supported.</span></span>|
|<span data-ttu-id="d6e68-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6e68-116">Application</span></span>|<span data-ttu-id="d6e68-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6e68-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6e68-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6e68-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsFeatureUpdateProfiles
```

## <a name="request-headers"></a><span data-ttu-id="d6e68-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6e68-119">Request headers</span></span>
|<span data-ttu-id="d6e68-120">标头</span><span class="sxs-lookup"><span data-stu-id="d6e68-120">Header</span></span>|<span data-ttu-id="d6e68-121">值</span><span class="sxs-lookup"><span data-stu-id="d6e68-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6e68-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6e68-122">Authorization</span></span>|<span data-ttu-id="d6e68-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d6e68-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6e68-124">接受</span><span class="sxs-lookup"><span data-stu-id="d6e68-124">Accept</span></span>|<span data-ttu-id="d6e68-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d6e68-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6e68-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6e68-126">Request body</span></span>
<span data-ttu-id="d6e68-127">在请求正文中，提供 windowsFeatureUpdateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6e68-127">In the request body, supply a JSON representation for the windowsFeatureUpdateProfile object.</span></span>

<span data-ttu-id="d6e68-128">下表显示创建 windowsFeatureUpdateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d6e68-128">The following table shows the properties that are required when you create the windowsFeatureUpdateProfile.</span></span>

|<span data-ttu-id="d6e68-129">属性</span><span class="sxs-lookup"><span data-stu-id="d6e68-129">Property</span></span>|<span data-ttu-id="d6e68-130">类型</span><span class="sxs-lookup"><span data-stu-id="d6e68-130">Type</span></span>|<span data-ttu-id="d6e68-131">说明</span><span class="sxs-lookup"><span data-stu-id="d6e68-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6e68-132">id</span><span class="sxs-lookup"><span data-stu-id="d6e68-132">id</span></span>|<span data-ttu-id="d6e68-133">字符串</span><span class="sxs-lookup"><span data-stu-id="d6e68-133">String</span></span>|<span data-ttu-id="d6e68-134">实体的标识符。</span><span class="sxs-lookup"><span data-stu-id="d6e68-134">The Identifier of the entity.</span></span>|
|<span data-ttu-id="d6e68-135">displayName</span><span class="sxs-lookup"><span data-stu-id="d6e68-135">displayName</span></span>|<span data-ttu-id="d6e68-136">String</span><span class="sxs-lookup"><span data-stu-id="d6e68-136">String</span></span>|<span data-ttu-id="d6e68-137">配置文件的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d6e68-137">The display name of the profile.</span></span>|
|<span data-ttu-id="d6e68-138">说明</span><span class="sxs-lookup"><span data-stu-id="d6e68-138">description</span></span>|<span data-ttu-id="d6e68-139">String</span><span class="sxs-lookup"><span data-stu-id="d6e68-139">String</span></span>|<span data-ttu-id="d6e68-140">用户指定的配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="d6e68-140">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="d6e68-141">featureUpdateVersion</span><span class="sxs-lookup"><span data-stu-id="d6e68-141">featureUpdateVersion</span></span>|<span data-ttu-id="d6e68-142">String</span><span class="sxs-lookup"><span data-stu-id="d6e68-142">String</span></span>|<span data-ttu-id="d6e68-143">将部署到此配置文件目标的设备的功能更新版本。</span><span class="sxs-lookup"><span data-stu-id="d6e68-143">The feature update version that will be deployed to the devices targeted by this profile.</span></span> <span data-ttu-id="d6e68-144">版本可以是任何受支持的版本，例如，1709、1803或1809等。</span><span class="sxs-lookup"><span data-stu-id="d6e68-144">The version could be any supported version for example 1709, 1803 or 1809 and so on.</span></span>|
|<span data-ttu-id="d6e68-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d6e68-145">createdDateTime</span></span>|<span data-ttu-id="d6e68-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6e68-146">DateTimeOffset</span></span>|<span data-ttu-id="d6e68-147">创建配置文件的日期时间。</span><span class="sxs-lookup"><span data-stu-id="d6e68-147">The date time that the profile was created.</span></span>|
|<span data-ttu-id="d6e68-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d6e68-148">lastModifiedDateTime</span></span>|<span data-ttu-id="d6e68-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d6e68-149">DateTimeOffset</span></span>|<span data-ttu-id="d6e68-150">上次修改配置文件的日期时间。</span><span class="sxs-lookup"><span data-stu-id="d6e68-150">The date time that the profile was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="d6e68-151">响应</span><span class="sxs-lookup"><span data-stu-id="d6e68-151">Response</span></span>
<span data-ttu-id="d6e68-152">如果成功，此方法在响应`201 Created`正文中返回响应代码和[windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d6e68-152">If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6e68-153">示例</span><span class="sxs-lookup"><span data-stu-id="d6e68-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6e68-154">请求</span><span class="sxs-lookup"><span data-stu-id="d6e68-154">Request</span></span>
<span data-ttu-id="d6e68-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d6e68-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles
Content-type: application/json
Content-length: 207

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value"
}
```

### <a name="response"></a><span data-ttu-id="d6e68-156">响应</span><span class="sxs-lookup"><span data-stu-id="d6e68-156">Response</span></span>
<span data-ttu-id="d6e68-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d6e68-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 379

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
  "id": "885bd4ee-d4ee-885b-eed4-5b88eed45b88",
  "displayName": "Display Name value",
  "description": "Description value",
  "featureUpdateVersion": "Feature Update Version value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




