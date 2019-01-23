---
title: 创建 windowsUniversalAppXContainedApp
description: 创建新的 windowsUniversalAppXContainedApp 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: a86c8c329bac55b6497a28f0aaa6096d6e9f4e94
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418433"
---
# <a name="create-windowsuniversalappxcontainedapp"></a><span data-ttu-id="73dfc-103">创建 windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="73dfc-103">Create windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="73dfc-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="73dfc-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="73dfc-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="73dfc-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="73dfc-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="73dfc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73dfc-107">创建新的[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="73dfc-107">Create a new [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73dfc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="73dfc-108">Prerequisites</span></span>
<span data-ttu-id="73dfc-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="73dfc-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="73dfc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="73dfc-111">Permission type</span></span>|<span data-ttu-id="73dfc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="73dfc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73dfc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="73dfc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="73dfc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73dfc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="73dfc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="73dfc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73dfc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="73dfc-116">Not supported.</span></span>|
|<span data-ttu-id="73dfc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="73dfc-117">Application</span></span>|<span data-ttu-id="73dfc-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="73dfc-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73dfc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="73dfc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="73dfc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="73dfc-120">Request headers</span></span>
|<span data-ttu-id="73dfc-121">标头</span><span class="sxs-lookup"><span data-stu-id="73dfc-121">Header</span></span>|<span data-ttu-id="73dfc-122">值</span><span class="sxs-lookup"><span data-stu-id="73dfc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73dfc-123">授权</span><span class="sxs-lookup"><span data-stu-id="73dfc-123">Authorization</span></span>|<span data-ttu-id="73dfc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="73dfc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73dfc-125">Accept</span><span class="sxs-lookup"><span data-stu-id="73dfc-125">Accept</span></span>|<span data-ttu-id="73dfc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="73dfc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73dfc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="73dfc-127">Request body</span></span>
<span data-ttu-id="73dfc-128">在请求正文中，提供 windowsUniversalAppXContainedApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73dfc-128">In the request body, supply a JSON representation for the windowsUniversalAppXContainedApp object.</span></span>

<span data-ttu-id="73dfc-129">下表显示时创建 windowsUniversalAppXContainedApp 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="73dfc-129">The following table shows the properties that are required when you create the windowsUniversalAppXContainedApp.</span></span>

|<span data-ttu-id="73dfc-130">属性</span><span class="sxs-lookup"><span data-stu-id="73dfc-130">Property</span></span>|<span data-ttu-id="73dfc-131">类型</span><span class="sxs-lookup"><span data-stu-id="73dfc-131">Type</span></span>|<span data-ttu-id="73dfc-132">说明</span><span class="sxs-lookup"><span data-stu-id="73dfc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="73dfc-133">id</span><span class="sxs-lookup"><span data-stu-id="73dfc-133">id</span></span>|<span data-ttu-id="73dfc-134">String</span><span class="sxs-lookup"><span data-stu-id="73dfc-134">String</span></span>|<span data-ttu-id="73dfc-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="73dfc-135">Key of the entity.</span></span> <span data-ttu-id="73dfc-136">继承自[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="73dfc-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="73dfc-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="73dfc-137">appUserModelId</span></span>|<span data-ttu-id="73dfc-138">String</span><span class="sxs-lookup"><span data-stu-id="73dfc-138">String</span></span>|<span data-ttu-id="73dfc-139">包含 WindowsUniversalAppX 应用程序的应用程序的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="73dfc-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="73dfc-140">响应</span><span class="sxs-lookup"><span data-stu-id="73dfc-140">Response</span></span>
<span data-ttu-id="73dfc-141">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="73dfc-141">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="73dfc-142">示例</span><span class="sxs-lookup"><span data-stu-id="73dfc-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="73dfc-143">请求</span><span class="sxs-lookup"><span data-stu-id="73dfc-143">Request</span></span>
<span data-ttu-id="73dfc-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="73dfc-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="73dfc-145">响应</span><span class="sxs-lookup"><span data-stu-id="73dfc-145">Response</span></span>
<span data-ttu-id="73dfc-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="73dfc-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




