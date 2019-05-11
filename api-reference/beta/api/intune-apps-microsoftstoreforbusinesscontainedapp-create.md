---
title: 创建 microsoftStoreForBusinessContainedApp
description: 创建新的 microsoftStoreForBusinessContainedApp 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: cbdea27ad63b3216df4e729d5f4fc3387a5ade5a
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33935403"
---
# <a name="create-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="ec0ac-103">创建 microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="ec0ac-103">Create microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="ec0ac-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ec0ac-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ec0ac-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ec0ac-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ec0ac-106">创建新的[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ec0ac-106">Create a new [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ec0ac-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="ec0ac-107">Prerequisites</span></span>
<span data-ttu-id="ec0ac-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ec0ac-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ec0ac-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ec0ac-110">Permission type</span></span>|<span data-ttu-id="ec0ac-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ec0ac-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ec0ac-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ec0ac-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ec0ac-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ec0ac-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ec0ac-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ec0ac-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ec0ac-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec0ac-115">Not supported.</span></span>|
|<span data-ttu-id="ec0ac-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ec0ac-116">Application</span></span>|<span data-ttu-id="ec0ac-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ec0ac-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ec0ac-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ec0ac-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="ec0ac-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ec0ac-119">Request headers</span></span>
|<span data-ttu-id="ec0ac-120">标头</span><span class="sxs-lookup"><span data-stu-id="ec0ac-120">Header</span></span>|<span data-ttu-id="ec0ac-121">值</span><span class="sxs-lookup"><span data-stu-id="ec0ac-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ec0ac-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ec0ac-122">Authorization</span></span>|<span data-ttu-id="ec0ac-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ec0ac-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ec0ac-124">接受</span><span class="sxs-lookup"><span data-stu-id="ec0ac-124">Accept</span></span>|<span data-ttu-id="ec0ac-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ec0ac-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ec0ac-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ec0ac-126">Request body</span></span>
<span data-ttu-id="ec0ac-127">在请求正文中, 提供 microsoftStoreForBusinessContainedApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ec0ac-127">In the request body, supply a JSON representation for the microsoftStoreForBusinessContainedApp object.</span></span>

<span data-ttu-id="ec0ac-128">下表显示创建 microsoftStoreForBusinessContainedApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ec0ac-128">The following table shows the properties that are required when you create the microsoftStoreForBusinessContainedApp.</span></span>

|<span data-ttu-id="ec0ac-129">属性</span><span class="sxs-lookup"><span data-stu-id="ec0ac-129">Property</span></span>|<span data-ttu-id="ec0ac-130">类型</span><span class="sxs-lookup"><span data-stu-id="ec0ac-130">Type</span></span>|<span data-ttu-id="ec0ac-131">说明</span><span class="sxs-lookup"><span data-stu-id="ec0ac-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ec0ac-132">id</span><span class="sxs-lookup"><span data-stu-id="ec0ac-132">id</span></span>|<span data-ttu-id="ec0ac-133">String</span><span class="sxs-lookup"><span data-stu-id="ec0ac-133">String</span></span>|<span data-ttu-id="ec0ac-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="ec0ac-134">Key of the entity.</span></span> <span data-ttu-id="ec0ac-135">继承自[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="ec0ac-135">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="ec0ac-136">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="ec0ac-136">appUserModelId</span></span>|<span data-ttu-id="ec0ac-137">String</span><span class="sxs-lookup"><span data-stu-id="ec0ac-137">String</span></span>|<span data-ttu-id="ec0ac-138">MicrosoftStoreForBusinessApp 的包含应用程序的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="ec0ac-138">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="ec0ac-139">响应</span><span class="sxs-lookup"><span data-stu-id="ec0ac-139">Response</span></span>
<span data-ttu-id="ec0ac-140">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ec0ac-140">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ec0ac-141">示例</span><span class="sxs-lookup"><span data-stu-id="ec0ac-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="ec0ac-142">请求</span><span class="sxs-lookup"><span data-stu-id="ec0ac-142">Request</span></span>
<span data-ttu-id="ec0ac-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ec0ac-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="ec0ac-144">响应</span><span class="sxs-lookup"><span data-stu-id="ec0ac-144">Response</span></span>
<span data-ttu-id="ec0ac-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ec0ac-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 176

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "bf1d79df-79df-bf1d-df79-1dbfdf791dbf",
  "appUserModelId": "App User Model Id value"
}
```




