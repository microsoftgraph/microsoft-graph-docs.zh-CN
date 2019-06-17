---
title: 创建 windowsUniversalAppXContainedApp
description: 创建新的 windowsUniversalAppXContainedApp 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 4294a45fabb46781f1f4483f2607a9d2ad5a8835
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/14/2019
ms.locfileid: "34972702"
---
# <a name="create-windowsuniversalappxcontainedapp"></a><span data-ttu-id="67b8e-103">创建 windowsUniversalAppXContainedApp</span><span class="sxs-lookup"><span data-stu-id="67b8e-103">Create windowsUniversalAppXContainedApp</span></span>

> <span data-ttu-id="67b8e-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="67b8e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="67b8e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="67b8e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="67b8e-106">创建新的[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="67b8e-106">Create a new [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="67b8e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="67b8e-107">Prerequisites</span></span>
<span data-ttu-id="67b8e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="67b8e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="67b8e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="67b8e-110">Permission type</span></span>|<span data-ttu-id="67b8e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="67b8e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="67b8e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="67b8e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="67b8e-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="67b8e-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="67b8e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="67b8e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="67b8e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="67b8e-115">Not supported.</span></span>|
|<span data-ttu-id="67b8e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="67b8e-116">Application</span></span>|<span data-ttu-id="67b8e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="67b8e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="67b8e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="67b8e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="67b8e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="67b8e-119">Request headers</span></span>
|<span data-ttu-id="67b8e-120">标头</span><span class="sxs-lookup"><span data-stu-id="67b8e-120">Header</span></span>|<span data-ttu-id="67b8e-121">值</span><span class="sxs-lookup"><span data-stu-id="67b8e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="67b8e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="67b8e-122">Authorization</span></span>|<span data-ttu-id="67b8e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="67b8e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="67b8e-124">接受</span><span class="sxs-lookup"><span data-stu-id="67b8e-124">Accept</span></span>|<span data-ttu-id="67b8e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="67b8e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="67b8e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="67b8e-126">Request body</span></span>
<span data-ttu-id="67b8e-127">在请求正文中, 提供 windowsUniversalAppXContainedApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="67b8e-127">In the request body, supply a JSON representation for the windowsUniversalAppXContainedApp object.</span></span>

<span data-ttu-id="67b8e-128">下表显示创建 windowsUniversalAppXContainedApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="67b8e-128">The following table shows the properties that are required when you create the windowsUniversalAppXContainedApp.</span></span>

|<span data-ttu-id="67b8e-129">属性</span><span class="sxs-lookup"><span data-stu-id="67b8e-129">Property</span></span>|<span data-ttu-id="67b8e-130">类型</span><span class="sxs-lookup"><span data-stu-id="67b8e-130">Type</span></span>|<span data-ttu-id="67b8e-131">说明</span><span class="sxs-lookup"><span data-stu-id="67b8e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="67b8e-132">id</span><span class="sxs-lookup"><span data-stu-id="67b8e-132">id</span></span>|<span data-ttu-id="67b8e-133">String</span><span class="sxs-lookup"><span data-stu-id="67b8e-133">String</span></span>|<span data-ttu-id="67b8e-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="67b8e-134">Key of the entity.</span></span> <span data-ttu-id="67b8e-135">继承自[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="67b8e-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="67b8e-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="67b8e-136">appUserModelId</span></span>|<span data-ttu-id="67b8e-137">String</span><span class="sxs-lookup"><span data-stu-id="67b8e-137">String</span></span>|<span data-ttu-id="67b8e-138">WindowsUniversalAppX 应用程序包含的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="67b8e-138">The app user model ID of the contained app of a WindowsUniversalAppX app.</span></span>|



## <a name="response"></a><span data-ttu-id="67b8e-139">响应</span><span class="sxs-lookup"><span data-stu-id="67b8e-139">Response</span></span>
<span data-ttu-id="67b8e-140">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="67b8e-140">If successful, this method returns a `201 Created` response code and a [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="67b8e-141">示例</span><span class="sxs-lookup"><span data-stu-id="67b8e-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="67b8e-142">请求</span><span class="sxs-lookup"><span data-stu-id="67b8e-142">Request</span></span>
<span data-ttu-id="67b8e-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="67b8e-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 122

{
  "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="67b8e-144">响应</span><span class="sxs-lookup"><span data-stu-id="67b8e-144">Response</span></span>
<span data-ttu-id="67b8e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="67b8e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





