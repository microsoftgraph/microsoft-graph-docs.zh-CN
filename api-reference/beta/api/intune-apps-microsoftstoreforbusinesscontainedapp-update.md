---
title: 更新 microsoftStoreForBusinessContainedApp
description: 更新 microsoftStoreForBusinessContainedApp 对象的属性。
author: tfitzmac
ms.openlocfilehash: e4b9e451e5632a8d4b923aae5de86c854febfa2a
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27324806"
---
# <a name="update-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="0e008-103">更新 microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="0e008-103">Update microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="0e008-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="0e008-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0e008-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0e008-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="0e008-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="0e008-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="0e008-107">更新[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="0e008-107">Update the properties of a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="0e008-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="0e008-108">Prerequisites</span></span>
<span data-ttu-id="0e008-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="0e008-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0e008-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="0e008-111">Permission type</span></span>|<span data-ttu-id="0e008-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0e008-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0e008-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0e008-113">Delegated (work or school account)</span></span>|<span data-ttu-id="0e008-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0e008-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0e008-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0e008-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0e008-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e008-116">Not supported.</span></span>|
|<span data-ttu-id="0e008-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="0e008-117">Application</span></span>|<span data-ttu-id="0e008-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="0e008-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0e008-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0e008-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps/{mobileContainedAppId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps/{mobileContainedAppId}
```

## <a name="request-headers"></a><span data-ttu-id="0e008-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="0e008-120">Request headers</span></span>
|<span data-ttu-id="0e008-121">标头</span><span class="sxs-lookup"><span data-stu-id="0e008-121">Header</span></span>|<span data-ttu-id="0e008-122">值</span><span class="sxs-lookup"><span data-stu-id="0e008-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0e008-123">授权</span><span class="sxs-lookup"><span data-stu-id="0e008-123">Authorization</span></span>|<span data-ttu-id="0e008-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0e008-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0e008-125">Accept</span><span class="sxs-lookup"><span data-stu-id="0e008-125">Accept</span></span>|<span data-ttu-id="0e008-126">application/json</span><span class="sxs-lookup"><span data-stu-id="0e008-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0e008-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0e008-127">Request body</span></span>
<span data-ttu-id="0e008-128">在请求正文中，提供[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0e008-128">In the request body, supply a JSON representation for the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>

<span data-ttu-id="0e008-129">下表显示时创建[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0e008-129">The following table shows the properties that are required when you create the [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md).</span></span>

|<span data-ttu-id="0e008-130">属性</span><span class="sxs-lookup"><span data-stu-id="0e008-130">Property</span></span>|<span data-ttu-id="0e008-131">类型</span><span class="sxs-lookup"><span data-stu-id="0e008-131">Type</span></span>|<span data-ttu-id="0e008-132">说明</span><span class="sxs-lookup"><span data-stu-id="0e008-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0e008-133">id</span><span class="sxs-lookup"><span data-stu-id="0e008-133">id</span></span>|<span data-ttu-id="0e008-134">String</span><span class="sxs-lookup"><span data-stu-id="0e008-134">String</span></span>|<span data-ttu-id="0e008-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="0e008-135">Key of the entity.</span></span> <span data-ttu-id="0e008-136">继承自[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="0e008-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="0e008-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="0e008-137">appUserModelId</span></span>|<span data-ttu-id="0e008-138">字符串</span><span class="sxs-lookup"><span data-stu-id="0e008-138">String</span></span>|<span data-ttu-id="0e008-139">MicrosoftStoreForBusinessApp 包含应用程序的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="0e008-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="0e008-140">响应</span><span class="sxs-lookup"><span data-stu-id="0e008-140">Response</span></span>
<span data-ttu-id="0e008-141">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0e008-141">If successful, this method returns a `200 OK` response code and an updated [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0e008-142">示例</span><span class="sxs-lookup"><span data-stu-id="0e008-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="0e008-143">请求</span><span class="sxs-lookup"><span data-stu-id="0e008-143">Request</span></span>
<span data-ttu-id="0e008-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0e008-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps/{mobileContainedAppId}
Content-type: application/json
Content-length: 51

{
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="0e008-145">响应</span><span class="sxs-lookup"><span data-stu-id="0e008-145">Response</span></span>
<span data-ttu-id="0e008-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0e008-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 176

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "id": "bf1d79df-79df-bf1d-df79-1dbfdf791dbf",
  "appUserModelId": "App User Model Id value"
}
```





