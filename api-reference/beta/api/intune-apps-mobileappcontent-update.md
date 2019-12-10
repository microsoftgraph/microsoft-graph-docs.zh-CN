---
title: 更新 mobileAppContent
description: 更新 mobileAppContent 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: aeaf2a3c3ae5dc49a746697fc15cf40706cddcbb
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39935601"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="928c0-103">更新 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="928c0-103">Update mobileAppContent</span></span>

> <span data-ttu-id="928c0-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="928c0-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="928c0-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="928c0-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="928c0-106">更新 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="928c0-106">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="928c0-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="928c0-107">Prerequisites</span></span>
<span data-ttu-id="928c0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="928c0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="928c0-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="928c0-110">Permission type</span></span>|<span data-ttu-id="928c0-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="928c0-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="928c0-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="928c0-112">Delegated (work or school account)</span></span>|<span data-ttu-id="928c0-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="928c0-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="928c0-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="928c0-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="928c0-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="928c0-115">Not supported.</span></span>|
|<span data-ttu-id="928c0-116">Application</span><span class="sxs-lookup"><span data-stu-id="928c0-116">Application</span></span>|<span data-ttu-id="928c0-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="928c0-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="928c0-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="928c0-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="928c0-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="928c0-119">Request headers</span></span>
|<span data-ttu-id="928c0-120">标头</span><span class="sxs-lookup"><span data-stu-id="928c0-120">Header</span></span>|<span data-ttu-id="928c0-121">值</span><span class="sxs-lookup"><span data-stu-id="928c0-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="928c0-122">授权</span><span class="sxs-lookup"><span data-stu-id="928c0-122">Authorization</span></span>|<span data-ttu-id="928c0-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="928c0-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="928c0-124">接受</span><span class="sxs-lookup"><span data-stu-id="928c0-124">Accept</span></span>|<span data-ttu-id="928c0-125">application/json</span><span class="sxs-lookup"><span data-stu-id="928c0-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="928c0-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="928c0-126">Request body</span></span>
<span data-ttu-id="928c0-127">在请求正文中，提供 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="928c0-127">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="928c0-128">下表显示创建 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="928c0-128">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="928c0-129">属性</span><span class="sxs-lookup"><span data-stu-id="928c0-129">Property</span></span>|<span data-ttu-id="928c0-130">类型</span><span class="sxs-lookup"><span data-stu-id="928c0-130">Type</span></span>|<span data-ttu-id="928c0-131">说明</span><span class="sxs-lookup"><span data-stu-id="928c0-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="928c0-132">id</span><span class="sxs-lookup"><span data-stu-id="928c0-132">id</span></span>|<span data-ttu-id="928c0-133">字符串</span><span class="sxs-lookup"><span data-stu-id="928c0-133">String</span></span>|<span data-ttu-id="928c0-134">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="928c0-134">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="928c0-135">响应</span><span class="sxs-lookup"><span data-stu-id="928c0-135">Response</span></span>
<span data-ttu-id="928c0-136">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="928c0-136">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="928c0-137">示例</span><span class="sxs-lookup"><span data-stu-id="928c0-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="928c0-138">请求</span><span class="sxs-lookup"><span data-stu-id="928c0-138">Request</span></span>
<span data-ttu-id="928c0-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="928c0-139">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="928c0-140">响应</span><span class="sxs-lookup"><span data-stu-id="928c0-140">Response</span></span>
<span data-ttu-id="928c0-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="928c0-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```





