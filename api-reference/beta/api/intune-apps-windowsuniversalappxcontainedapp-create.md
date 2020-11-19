---
title: 创建 windowsUniversalAppXContainedApp
description: 创建新的 windowsUniversalAppXContainedApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 3cf163d05e084d17b5f46df6f78d731db9561c2b
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49245933"
---
# <a name="create-windowsuniversalappxcontainedapp"></a><span data-ttu-id="9ddc0-103">创建 windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="9ddc0-103">Create windowsUniversalAppXContainedApp</span></span>

<span data-ttu-id="9ddc0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9ddc0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9ddc0-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9ddc0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9ddc0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9ddc0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9ddc0-107">创建新的 [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ddc0-107">Create a new [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9ddc0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9ddc0-108">Prerequisites</span></span>
<span data-ttu-id="9ddc0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9ddc0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9ddc0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9ddc0-111">Permission type</span></span>|<span data-ttu-id="9ddc0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9ddc0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9ddc0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9ddc0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9ddc0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ddc0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="9ddc0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9ddc0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9ddc0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9ddc0-116">Not supported.</span></span>|
|<span data-ttu-id="9ddc0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9ddc0-117">Application</span></span>|<span data-ttu-id="9ddc0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9ddc0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9ddc0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9ddc0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="9ddc0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9ddc0-120">Request headers</span></span>
|<span data-ttu-id="9ddc0-121">标头</span><span class="sxs-lookup"><span data-stu-id="9ddc0-121">Header</span></span>|<span data-ttu-id="9ddc0-122">值</span><span class="sxs-lookup"><span data-stu-id="9ddc0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9ddc0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9ddc0-123">Authorization</span></span>|<span data-ttu-id="9ddc0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9ddc0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9ddc0-125">接受</span><span class="sxs-lookup"><span data-stu-id="9ddc0-125">Accept</span></span>|<span data-ttu-id="9ddc0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9ddc0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9ddc0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9ddc0-127">Request body</span></span>
<span data-ttu-id="9ddc0-128">在请求正文中，提供 windowsUniversalAppXContainedApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="9ddc0-128">In the request body, supply a JSON representation for the windowsUniversalAppXContainedApp object.</span></span>

<span data-ttu-id="9ddc0-129">下表显示创建 windowsUniversalAppXContainedApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="9ddc0-129">The following table shows the properties that are required when you create the windowsUniversalAppXContainedApp.</span></span>

|<span data-ttu-id="9ddc0-130">属性</span><span class="sxs-lookup"><span data-stu-id="9ddc0-130">Property</span></span>|<span data-ttu-id="9ddc0-131">类型</span><span class="sxs-lookup"><span data-stu-id="9ddc0-131">Type</span></span>|<span data-ttu-id="9ddc0-132">说明</span><span class="sxs-lookup"><span data-stu-id="9ddc0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="9ddc0-133">id</span><span class="sxs-lookup"><span data-stu-id="9ddc0-133">id</span></span>|<span data-ttu-id="9ddc0-134">String</span><span class="sxs-lookup"><span data-stu-id="9ddc0-134">String</span></span>|<span data-ttu-id="9ddc0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="9ddc0-135">Key of the entity.</span></span> <span data-ttu-id="9ddc0-136">继承自 [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="9ddc0-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="9ddc0-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="9ddc0-137">appUserModelId</span></span>|<span data-ttu-id="9ddc0-138">String</span><span class="sxs-lookup"><span data-stu-id="9ddc0-138">String</span></span>|<span data-ttu-id="9ddc0-139">WindowsUniversalAppX 应用程序包含的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="9ddc0-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="9ddc0-140">响应</span><span class="sxs-lookup"><span data-stu-id="9ddc0-140">Response</span></span>
<span data-ttu-id="9ddc0-141">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="9ddc0-141">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9ddc0-142">示例</span><span class="sxs-lookup"><span data-stu-id="9ddc0-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="9ddc0-143">请求</span><span class="sxs-lookup"><span data-stu-id="9ddc0-143">Request</span></span>
<span data-ttu-id="9ddc0-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9ddc0-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="9ddc0-145">响应</span><span class="sxs-lookup"><span data-stu-id="9ddc0-145">Response</span></span>
<span data-ttu-id="9ddc0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9ddc0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 171

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
  "appUserModelId": "App User Model Id value"
}
```




