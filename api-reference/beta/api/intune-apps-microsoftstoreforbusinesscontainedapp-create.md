---
title: 创建 microsoftStoreForBusinessContainedApp
description: 创建新的 microsoftStoreForBusinessContainedApp 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ac782261c00008bf9b4ab552932f8f841a9965bc
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27843293"
---
# <a name="create-microsoftstoreforbusinesscontainedapp"></a><span data-ttu-id="2388b-103">创建 microsoftStoreForBusinessContainedApp</span><span class="sxs-lookup"><span data-stu-id="2388b-103">Create microsoftStoreForBusinessContainedApp</span></span>

> <span data-ttu-id="2388b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="2388b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2388b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2388b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2388b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="2388b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="2388b-107">创建新的[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2388b-107">Create a new [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="2388b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2388b-108">Prerequisites</span></span>
<span data-ttu-id="2388b-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="2388b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2388b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2388b-111">Permission type</span></span>|<span data-ttu-id="2388b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2388b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2388b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2388b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2388b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2388b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2388b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2388b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2388b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2388b-116">Not supported.</span></span>|
|<span data-ttu-id="2388b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2388b-117">Application</span></span>|<span data-ttu-id="2388b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2388b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2388b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2388b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="2388b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2388b-120">Request headers</span></span>
|<span data-ttu-id="2388b-121">标头</span><span class="sxs-lookup"><span data-stu-id="2388b-121">Header</span></span>|<span data-ttu-id="2388b-122">值</span><span class="sxs-lookup"><span data-stu-id="2388b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2388b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2388b-123">Authorization</span></span>|<span data-ttu-id="2388b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2388b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2388b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2388b-125">Accept</span></span>|<span data-ttu-id="2388b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2388b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2388b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2388b-127">Request body</span></span>
<span data-ttu-id="2388b-128">在请求正文中，提供 microsoftStoreForBusinessContainedApp 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2388b-128">In the request body, supply a JSON representation for the microsoftStoreForBusinessContainedApp object.</span></span>

<span data-ttu-id="2388b-129">下表显示时创建 microsoftStoreForBusinessContainedApp 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2388b-129">The following table shows the properties that are required when you create the microsoftStoreForBusinessContainedApp.</span></span>

|<span data-ttu-id="2388b-130">属性</span><span class="sxs-lookup"><span data-stu-id="2388b-130">Property</span></span>|<span data-ttu-id="2388b-131">类型</span><span class="sxs-lookup"><span data-stu-id="2388b-131">Type</span></span>|<span data-ttu-id="2388b-132">说明</span><span class="sxs-lookup"><span data-stu-id="2388b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2388b-133">id</span><span class="sxs-lookup"><span data-stu-id="2388b-133">id</span></span>|<span data-ttu-id="2388b-134">String</span><span class="sxs-lookup"><span data-stu-id="2388b-134">String</span></span>|<span data-ttu-id="2388b-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="2388b-135">Key of the entity.</span></span> <span data-ttu-id="2388b-136">继承自[mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span><span class="sxs-lookup"><span data-stu-id="2388b-136">Inherited from [mobileContainedApp](../resources/intune-apps-mobilecontainedapp.md)</span></span>|
|<span data-ttu-id="2388b-137">appUserModelId</span><span class="sxs-lookup"><span data-stu-id="2388b-137">appUserModelId</span></span>|<span data-ttu-id="2388b-138">字符串</span><span class="sxs-lookup"><span data-stu-id="2388b-138">String</span></span>|<span data-ttu-id="2388b-139">MicrosoftStoreForBusinessApp 包含应用程序的应用程序用户模型 ID。</span><span class="sxs-lookup"><span data-stu-id="2388b-139">The app user model ID of the contained app of a MicrosoftStoreForBusinessApp.</span></span>|



## <a name="response"></a><span data-ttu-id="2388b-140">响应</span><span class="sxs-lookup"><span data-stu-id="2388b-140">Response</span></span>
<span data-ttu-id="2388b-141">如果成功，此方法返回`201 Created`响应代码和响应正文中的[microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md)对象。</span><span class="sxs-lookup"><span data-stu-id="2388b-141">If successful, this method returns a `201 Created` response code and a [microsoftStoreForBusinessContainedApp](../resources/intune-apps-microsoftstoreforbusinesscontainedapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="2388b-142">示例</span><span class="sxs-lookup"><span data-stu-id="2388b-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="2388b-143">请求</span><span class="sxs-lookup"><span data-stu-id="2388b-143">Request</span></span>
<span data-ttu-id="2388b-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2388b-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
Content-type: application/json
Content-length: 127

{
  "@odata.type": "#microsoft.graph.microsoftStoreForBusinessContainedApp",
  "appUserModelId": "App User Model Id value"
}
```

### <a name="response"></a><span data-ttu-id="2388b-145">响应</span><span class="sxs-lookup"><span data-stu-id="2388b-145">Response</span></span>
<span data-ttu-id="2388b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2388b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





