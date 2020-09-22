---
title: 更新 windowsUniversalAppXContainedApp
description: 更新 windowsUniversalAppXContainedApp 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a399b0f2c591a232a4c778b6f86ca2bebe9e46aa
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47975967"
---
# <a name="update-windowsuniversalappxcontainedapp"></a><span data-ttu-id="37132-103">更新 windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="37132-103">Update windowsUniversalAppXContainedApp</span></span>

<span data-ttu-id="37132-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37132-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37132-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="37132-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37132-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="37132-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37132-107">更新 [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="37132-107">Update the properties of a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37132-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="37132-108">Prerequisites</span></span>
<span data-ttu-id="37132-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37132-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37132-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="37132-111">Permission type</span></span>|<span data-ttu-id="37132-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="37132-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37132-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37132-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37132-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37132-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="37132-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37132-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37132-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="37132-116">Not supported.</span></span>|
|<span data-ttu-id="37132-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="37132-117">Application</span></span>|<span data-ttu-id="37132-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37132-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37132-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37132-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="37132-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="37132-120">Request headers</span></span>
|<span data-ttu-id="37132-121">标头</span><span class="sxs-lookup"><span data-stu-id="37132-121">Header</span></span>|<span data-ttu-id="37132-122">值</span><span class="sxs-lookup"><span data-stu-id="37132-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37132-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="37132-123">Authorization</span></span>|<span data-ttu-id="37132-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="37132-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37132-125">接受</span><span class="sxs-lookup"><span data-stu-id="37132-125">Accept</span></span>|<span data-ttu-id="37132-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37132-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37132-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="37132-127">Request body</span></span>
<span data-ttu-id="37132-128">在请求正文中，提供 [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37132-128">In the request body, supply a JSON representation for the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

<span data-ttu-id="37132-129">下表显示创建 [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="37132-129">The following table shows the properties that are required when you create the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md).</span></span>

|<span data-ttu-id="37132-130">属性</span><span class="sxs-lookup"><span data-stu-id="37132-130">Property</span></span>|<span data-ttu-id="37132-131">类型</span><span class="sxs-lookup"><span data-stu-id="37132-131">Type</span></span>|<span data-ttu-id="37132-132">说明</span><span class="sxs-lookup"><span data-stu-id="37132-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37132-133">id</span><span class="sxs-lookup"><span data-stu-id="37132-133">id</span></span>|<span data-ttu-id="37132-134">String</span><span class="sxs-lookup"><span data-stu-id="37132-134">String</span></span>|<span data-ttu-id="37132-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="37132-135">Key of the entity.</span></span> <span data-ttu-id="37132-136">继承自 [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="37132-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="37132-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="37132-137">appUserModelId</span></span>|<span data-ttu-id="37132-138">String</span><span class="sxs-lookup"><span data-stu-id="37132-138">String</span></span>|<span data-ttu-id="37132-139">WindowsUniversalAppX 应用程序包含的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="37132-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="37132-140">响应</span><span class="sxs-lookup"><span data-stu-id="37132-140">Response</span></span>
<span data-ttu-id="37132-141">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="37132-141">If successful, this method returns a `200 OK` response code and an updated [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37132-142">示例</span><span class="sxs-lookup"><span data-stu-id="37132-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="37132-143">请求</span><span class="sxs-lookup"><span data-stu-id="37132-143">Request</span></span>
<span data-ttu-id="37132-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="37132-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="37132-145">响应</span><span class="sxs-lookup"><span data-stu-id="37132-145">Response</span></span>
<span data-ttu-id="37132-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="37132-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






