---
title: 创建 windowsQualityUpdateProfile
description: 创建新的 windowsQualityUpdateProfile 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cb1f1e20460c1bb9e109b45dea555ef0f475bd70
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160243"
---
# <a name="create-windowsqualityupdateprofile"></a><span data-ttu-id="dd586-103">创建 windowsQualityUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="dd586-103">Create windowsQualityUpdateProfile</span></span>

<span data-ttu-id="dd586-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="dd586-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="dd586-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="dd586-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="dd586-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="dd586-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="dd586-107">创建新的 [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dd586-107">Create a new [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="dd586-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="dd586-108">Prerequisites</span></span>
<span data-ttu-id="dd586-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="dd586-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="dd586-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="dd586-111">Permission type</span></span>|<span data-ttu-id="dd586-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="dd586-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="dd586-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="dd586-113">Delegated (work or school account)</span></span>|<span data-ttu-id="dd586-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd586-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="dd586-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="dd586-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="dd586-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="dd586-116">Not supported.</span></span>|
|<span data-ttu-id="dd586-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="dd586-117">Application</span></span>|<span data-ttu-id="dd586-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="dd586-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="dd586-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="dd586-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsQualityUpdateProfiles
```

## <a name="request-headers"></a><span data-ttu-id="dd586-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="dd586-120">Request headers</span></span>
|<span data-ttu-id="dd586-121">标头</span><span class="sxs-lookup"><span data-stu-id="dd586-121">Header</span></span>|<span data-ttu-id="dd586-122">值</span><span class="sxs-lookup"><span data-stu-id="dd586-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="dd586-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="dd586-123">Authorization</span></span>|<span data-ttu-id="dd586-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="dd586-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="dd586-125">接受</span><span class="sxs-lookup"><span data-stu-id="dd586-125">Accept</span></span>|<span data-ttu-id="dd586-126">application/json</span><span class="sxs-lookup"><span data-stu-id="dd586-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="dd586-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="dd586-127">Request body</span></span>
<span data-ttu-id="dd586-128">在请求正文中，提供 windowsQualityUpdateProfile 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="dd586-128">In the request body, supply a JSON representation for the windowsQualityUpdateProfile object.</span></span>

<span data-ttu-id="dd586-129">下表显示创建 windowsQualityUpdateProfile 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="dd586-129">The following table shows the properties that are required when you create the windowsQualityUpdateProfile.</span></span>

|<span data-ttu-id="dd586-130">属性</span><span class="sxs-lookup"><span data-stu-id="dd586-130">Property</span></span>|<span data-ttu-id="dd586-131">类型</span><span class="sxs-lookup"><span data-stu-id="dd586-131">Type</span></span>|<span data-ttu-id="dd586-132">说明</span><span class="sxs-lookup"><span data-stu-id="dd586-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="dd586-133">id</span><span class="sxs-lookup"><span data-stu-id="dd586-133">id</span></span>|<span data-ttu-id="dd586-134">String</span><span class="sxs-lookup"><span data-stu-id="dd586-134">String</span></span>|<span data-ttu-id="dd586-135">Intune 策略 ID。</span><span class="sxs-lookup"><span data-stu-id="dd586-135">The Intune policy id.</span></span>|
|<span data-ttu-id="dd586-136">displayName</span><span class="sxs-lookup"><span data-stu-id="dd586-136">displayName</span></span>|<span data-ttu-id="dd586-137">String</span><span class="sxs-lookup"><span data-stu-id="dd586-137">String</span></span>|<span data-ttu-id="dd586-138">配置文件显示名称的配置文件。</span><span class="sxs-lookup"><span data-stu-id="dd586-138">The display name for the profile.</span></span>|
|<span data-ttu-id="dd586-139">说明</span><span class="sxs-lookup"><span data-stu-id="dd586-139">description</span></span>|<span data-ttu-id="dd586-140">String</span><span class="sxs-lookup"><span data-stu-id="dd586-140">String</span></span>|<span data-ttu-id="dd586-141">由用户指定的配置文件的说明。</span><span class="sxs-lookup"><span data-stu-id="dd586-141">The description of the profile which is specified by the user.</span></span>|
|<span data-ttu-id="dd586-142">expeditedUpdateSettings</span><span class="sxs-lookup"><span data-stu-id="dd586-142">expeditedUpdateSettings</span></span>|[<span data-ttu-id="dd586-143">expeditedWindowsQualityUpdateSettings</span><span class="sxs-lookup"><span data-stu-id="dd586-143">expeditedWindowsQualityUpdateSettings</span></span>](../resources/intune-softwareupdate-expeditedwindowsqualityupdatesettings.md)|<span data-ttu-id="dd586-144">加速更新设置。</span><span class="sxs-lookup"><span data-stu-id="dd586-144">Expedited update settings.</span></span>|
|<span data-ttu-id="dd586-145">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="dd586-145">createdDateTime</span></span>|<span data-ttu-id="dd586-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd586-146">DateTimeOffset</span></span>|<span data-ttu-id="dd586-147">配置文件的创建日期时间。</span><span class="sxs-lookup"><span data-stu-id="dd586-147">The date time that the profile was created.</span></span>|
|<span data-ttu-id="dd586-148">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="dd586-148">lastModifiedDateTime</span></span>|<span data-ttu-id="dd586-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="dd586-149">DateTimeOffset</span></span>|<span data-ttu-id="dd586-150">上次修改配置文件的日期时间。</span><span class="sxs-lookup"><span data-stu-id="dd586-150">The date time that the profile was last modified.</span></span>|
|<span data-ttu-id="dd586-151">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="dd586-151">roleScopeTagIds</span></span>|<span data-ttu-id="dd586-152">字符串集合</span><span class="sxs-lookup"><span data-stu-id="dd586-152">String collection</span></span>|<span data-ttu-id="dd586-153">此质量更新实体的范围标记列表。</span><span class="sxs-lookup"><span data-stu-id="dd586-153">List of Scope Tags for this Quality Update entity.</span></span>|



## <a name="response"></a><span data-ttu-id="dd586-154">响应</span><span class="sxs-lookup"><span data-stu-id="dd586-154">Response</span></span>
<span data-ttu-id="dd586-155">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="dd586-155">If successful, this method returns a `201 Created` response code and a [windowsQualityUpdateProfile](../resources/intune-softwareupdate-windowsqualityupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="dd586-156">示例</span><span class="sxs-lookup"><span data-stu-id="dd586-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="dd586-157">请求</span><span class="sxs-lookup"><span data-stu-id="dd586-157">Request</span></span>
<span data-ttu-id="dd586-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="dd586-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsQualityUpdateProfiles
Content-type: application/json
Content-length: 418

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
  ]
}
```

### <a name="response"></a><span data-ttu-id="dd586-159">响应</span><span class="sxs-lookup"><span data-stu-id="dd586-159">Response</span></span>
<span data-ttu-id="dd586-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="dd586-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 590

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
  ]
}
```




