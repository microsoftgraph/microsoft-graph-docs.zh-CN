---
title: 创建 windowsUniversalAppXContainedApp
description: 创建新的 windowsUniversalAppXContainedApp 对象。
author: tfitzmac
ms.openlocfilehash: 97f50a79194af878569327073ae8911bf08199f3
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27302812"
---
# <a name="create-windowsuniversalappxcontainedapp"></a><span data-ttu-id="569b6-103">创建 windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="569b6-103">Create windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="569b6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="569b6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="569b6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="569b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="569b6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="569b6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="569b6-107">创建新的[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="569b6-107">Create a new [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="569b6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="569b6-108">Prerequisites</span></span>
<span data-ttu-id="569b6-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="569b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="569b6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="569b6-111">Permission type</span></span>|<span data-ttu-id="569b6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="569b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="569b6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="569b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="569b6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="569b6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="569b6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="569b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="569b6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="569b6-116">Not supported.</span></span>|
|<span data-ttu-id="569b6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="569b6-117">Application</span></span>|<span data-ttu-id="569b6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="569b6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="569b6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="569b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="569b6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="569b6-120">Request headers</span></span>
|<span data-ttu-id="569b6-121">标头</span><span class="sxs-lookup"><span data-stu-id="569b6-121">Header</span></span>|<span data-ttu-id="569b6-122">值</span><span class="sxs-lookup"><span data-stu-id="569b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="569b6-123">授权</span><span class="sxs-lookup"><span data-stu-id="569b6-123">Authorization</span></span>|<span data-ttu-id="569b6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="569b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="569b6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="569b6-125">Accept</span></span>|<span data-ttu-id="569b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="569b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="569b6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="569b6-127">Request body</span></span>
<span data-ttu-id="569b6-128">在请求正文中，提供 windowsUniversalAppXContainedApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="569b6-128">In the request body, supply a JSON representation for the windowsUniversalAppXContainedApp object.</span></span>

<span data-ttu-id="569b6-129">下表显示时创建 windowsUniversalAppXContainedApp 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="569b6-129">The following table shows the properties that are required when you create the windowsUniversalAppXContainedApp.</span></span>

|<span data-ttu-id="569b6-130">属性</span><span class="sxs-lookup"><span data-stu-id="569b6-130">Property</span></span>|<span data-ttu-id="569b6-131">类型</span><span class="sxs-lookup"><span data-stu-id="569b6-131">Type</span></span>|<span data-ttu-id="569b6-132">说明</span><span class="sxs-lookup"><span data-stu-id="569b6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="569b6-133">id</span><span class="sxs-lookup"><span data-stu-id="569b6-133">id</span></span>|<span data-ttu-id="569b6-134">String</span><span class="sxs-lookup"><span data-stu-id="569b6-134">String</span></span>|<span data-ttu-id="569b6-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="569b6-135">Key of the entity.</span></span> <span data-ttu-id="569b6-136">继承自[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="569b6-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="569b6-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="569b6-137">appUserModelId</span></span>|<span data-ttu-id="569b6-138">字符串</span><span class="sxs-lookup"><span data-stu-id="569b6-138">String</span></span>|<span data-ttu-id="569b6-139">包含 WindowsUniversalAppX 应用程序的应用程序的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="569b6-139">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="569b6-140">响应</span><span class="sxs-lookup"><span data-stu-id="569b6-140">Response</span></span>
<span data-ttu-id="569b6-141">如果成功，此方法返回`201 Created`响应代码和响应正文中的[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="569b6-141">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="569b6-142">示例</span><span class="sxs-lookup"><span data-stu-id="569b6-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="569b6-143">请求</span><span class="sxs-lookup"><span data-stu-id="569b6-143">Request</span></span>
<span data-ttu-id="569b6-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="569b6-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="569b6-145">响应</span><span class="sxs-lookup"><span data-stu-id="569b6-145">Response</span></span>
<span data-ttu-id="569b6-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="569b6-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





