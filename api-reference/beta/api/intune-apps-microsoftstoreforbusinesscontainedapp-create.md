---
title: 创建 microsoftStoreForBusinessContainedApp
description: 创建新的 microsoftStoreForBusinessContainedApp 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 8b2d2dfd0b29816ce987e95ecbfb4dc1691124c1
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51139963"
---
# <a name="create-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="1a854-103">创建 microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="1a854-103">Create microsoftStoreForBusinessContainedApp</span></span>

<span data-ttu-id="1a854-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a854-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a854-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1a854-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a854-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a854-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a854-107">创建新的 [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a854-107">Create a new [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a854-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1a854-108">Prerequisites</span></span>
<span data-ttu-id="1a854-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a854-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a854-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a854-111">Permission type</span></span>|<span data-ttu-id="1a854-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a854-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a854-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a854-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a854-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a854-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1a854-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a854-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a854-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a854-116">Not supported.</span></span>|
|<span data-ttu-id="1a854-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a854-117">Application</span></span>|<span data-ttu-id="1a854-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a854-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a854-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a854-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="1a854-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a854-120">Request headers</span></span>
|<span data-ttu-id="1a854-121">标头</span><span class="sxs-lookup"><span data-stu-id="1a854-121">Header</span></span>|<span data-ttu-id="1a854-122">值</span><span class="sxs-lookup"><span data-stu-id="1a854-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a854-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a854-123">Authorization</span></span>|<span data-ttu-id="1a854-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1a854-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a854-125">接受</span><span class="sxs-lookup"><span data-stu-id="1a854-125">Accept</span></span>|<span data-ttu-id="1a854-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a854-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a854-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a854-127">Request body</span></span>
<span data-ttu-id="1a854-128">在请求正文中，提供 microsoftStoreForBusinessContainedApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1a854-128">In the request body, supply a JSON representation for the microsoftStoreForBusinessContainedApp object.</span></span>

<span data-ttu-id="1a854-129">下表显示创建 microsoftStoreForBusinessContainedApp 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1a854-129">The following table shows the properties that are required when you create the microsoftStoreForBusinessContainedApp.</span></span>

|<span data-ttu-id="1a854-130">属性</span><span class="sxs-lookup"><span data-stu-id="1a854-130">Property</span></span>|<span data-ttu-id="1a854-131">类型</span><span class="sxs-lookup"><span data-stu-id="1a854-131">Type</span></span>|<span data-ttu-id="1a854-132">说明</span><span class="sxs-lookup"><span data-stu-id="1a854-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1a854-133">id</span><span class="sxs-lookup"><span data-stu-id="1a854-133">id</span></span>|<span data-ttu-id="1a854-134">String</span><span class="sxs-lookup"><span data-stu-id="1a854-134">String</span></span>|<span data-ttu-id="1a854-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1a854-135">Key of the entity.</span></span> <span data-ttu-id="1a854-136">继承自 [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="1a854-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="1a854-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="1a854-137">appUserModelId</span></span>|<span data-ttu-id="1a854-138">String</span><span class="sxs-lookup"><span data-stu-id="1a854-138">String</span></span>|<span data-ttu-id="1a854-139">MicrosoftStoreForBusinessApp 包含的应用程序的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="1a854-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="1a854-140">响应</span><span class="sxs-lookup"><span data-stu-id="1a854-140">Response</span></span>
<span data-ttu-id="1a854-141">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1a854-141">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a854-142">示例</span><span class="sxs-lookup"><span data-stu-id="1a854-142">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a854-143">请求</span><span class="sxs-lookup"><span data-stu-id="1a854-143">Request</span></span>
<span data-ttu-id="1a854-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a854-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="1a854-145">响应</span><span class="sxs-lookup"><span data-stu-id="1a854-145">Response</span></span>
<span data-ttu-id="1a854-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1a854-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




