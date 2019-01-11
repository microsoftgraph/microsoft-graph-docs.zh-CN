---
title: 更新 mobileAppContent
description: 更新 mobileAppContent 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 5d793c25763de7a33cbb18bebc8888d0c5cfd512
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27838358"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="5ea77-103">更新 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="5ea77-103">Update mobileAppContent</span></span>

> <span data-ttu-id="5ea77-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="5ea77-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5ea77-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="5ea77-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5ea77-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5ea77-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5ea77-107">更新 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="5ea77-107">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5ea77-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5ea77-108">Prerequisites</span></span>
<span data-ttu-id="5ea77-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="5ea77-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5ea77-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5ea77-111">Permission type</span></span>|<span data-ttu-id="5ea77-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5ea77-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5ea77-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5ea77-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5ea77-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5ea77-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5ea77-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5ea77-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5ea77-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ea77-116">Not supported.</span></span>|
|<span data-ttu-id="5ea77-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5ea77-117">Application</span></span>|<span data-ttu-id="5ea77-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="5ea77-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5ea77-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5ea77-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="5ea77-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5ea77-120">Request headers</span></span>
|<span data-ttu-id="5ea77-121">标头</span><span class="sxs-lookup"><span data-stu-id="5ea77-121">Header</span></span>|<span data-ttu-id="5ea77-122">值</span><span class="sxs-lookup"><span data-stu-id="5ea77-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5ea77-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5ea77-123">Authorization</span></span>|<span data-ttu-id="5ea77-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5ea77-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5ea77-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5ea77-125">Accept</span></span>|<span data-ttu-id="5ea77-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5ea77-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5ea77-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5ea77-127">Request body</span></span>
<span data-ttu-id="5ea77-128">在请求正文中，提供 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5ea77-128">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="5ea77-129">下表显示创建 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5ea77-129">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="5ea77-130">属性</span><span class="sxs-lookup"><span data-stu-id="5ea77-130">Property</span></span>|<span data-ttu-id="5ea77-131">类型</span><span class="sxs-lookup"><span data-stu-id="5ea77-131">Type</span></span>|<span data-ttu-id="5ea77-132">说明</span><span class="sxs-lookup"><span data-stu-id="5ea77-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5ea77-133">id</span><span class="sxs-lookup"><span data-stu-id="5ea77-133">id</span></span>|<span data-ttu-id="5ea77-134">String</span><span class="sxs-lookup"><span data-stu-id="5ea77-134">String</span></span>|<span data-ttu-id="5ea77-135">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="5ea77-135">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="5ea77-136">响应</span><span class="sxs-lookup"><span data-stu-id="5ea77-136">Response</span></span>
<span data-ttu-id="5ea77-137">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5ea77-137">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5ea77-138">示例</span><span class="sxs-lookup"><span data-stu-id="5ea77-138">Example</span></span>
### <a name="request"></a><span data-ttu-id="5ea77-139">请求</span><span class="sxs-lookup"><span data-stu-id="5ea77-139">Request</span></span>
<span data-ttu-id="5ea77-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5ea77-140">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 2

{}
```

### <a name="response"></a><span data-ttu-id="5ea77-141">响应</span><span class="sxs-lookup"><span data-stu-id="5ea77-141">Response</span></span>
<span data-ttu-id="5ea77-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5ea77-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```





