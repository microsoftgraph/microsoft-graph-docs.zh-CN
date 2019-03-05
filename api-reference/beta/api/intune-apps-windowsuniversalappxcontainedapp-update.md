---
title: 更新 windowsUniversalAppXContainedApp
description: 更新 windowsUniversalAppXContainedApp 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 8a3bacf74734fefe8255da981f0f71f4389db610
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30159834"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="d8339-103">更新 windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="d8339-103">Update windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="d8339-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d8339-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8339-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d8339-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8339-106">更新[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d8339-106">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8339-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d8339-107">Prerequisites</span></span>
<span data-ttu-id="d8339-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d8339-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d8339-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8339-110">Permission type</span></span>|<span data-ttu-id="d8339-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d8339-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8339-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8339-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d8339-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8339-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d8339-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8339-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8339-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8339-115">Not supported.</span></span>|
|<span data-ttu-id="d8339-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8339-116">Application</span></span>|<span data-ttu-id="d8339-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8339-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8339-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8339-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="d8339-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8339-119">Request headers</span></span>
|<span data-ttu-id="d8339-120">标头</span><span class="sxs-lookup"><span data-stu-id="d8339-120">Header</span></span>|<span data-ttu-id="d8339-121">值</span><span class="sxs-lookup"><span data-stu-id="d8339-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8339-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8339-122">Authorization</span></span>|<span data-ttu-id="d8339-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d8339-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8339-124">Accept</span><span class="sxs-lookup"><span data-stu-id="d8339-124">Accept</span></span>|<span data-ttu-id="d8339-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d8339-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8339-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8339-126">Request body</span></span>
<span data-ttu-id="d8339-127">在请求正文中, 提供[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8339-127">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="d8339-128">下表显示创建[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d8339-128">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="d8339-129">属性</span><span class="sxs-lookup"><span data-stu-id="d8339-129">Property</span></span>|<span data-ttu-id="d8339-130">类型</span><span class="sxs-lookup"><span data-stu-id="d8339-130">Type</span></span>|<span data-ttu-id="d8339-131">说明</span><span class="sxs-lookup"><span data-stu-id="d8339-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8339-132">id</span><span class="sxs-lookup"><span data-stu-id="d8339-132">id</span></span>|<span data-ttu-id="d8339-133">String</span><span class="sxs-lookup"><span data-stu-id="d8339-133">String</span></span>|<span data-ttu-id="d8339-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d8339-134">Key of the entity.</span></span> <span data-ttu-id="d8339-135">继承自[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="d8339-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="d8339-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="d8339-136">appUserModelId</span></span>|<span data-ttu-id="d8339-137">String</span><span class="sxs-lookup"><span data-stu-id="d8339-137">String</span></span>|<span data-ttu-id="d8339-138">WindowsUniversalAppX 应用程序包含的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="d8339-138">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="d8339-139">响应</span><span class="sxs-lookup"><span data-stu-id="d8339-139">Response</span></span>
<span data-ttu-id="d8339-140">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d8339-140">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8339-141">示例</span><span class="sxs-lookup"><span data-stu-id="d8339-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8339-142">请求</span><span class="sxs-lookup"><span data-stu-id="d8339-142">Request</span></span>
<span data-ttu-id="d8339-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d8339-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="d8339-144">响应</span><span class="sxs-lookup"><span data-stu-id="d8339-144">Response</span></span>
<span data-ttu-id="d8339-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d8339-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 171

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
  "appUserModelId": "App User Model Id value"
}
```




