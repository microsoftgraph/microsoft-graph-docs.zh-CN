---
title: 创建 mobileAppContent
description: 创建新的 mobileAppContent 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fede826dfdca0a823ec08a11fda096498e4babd7
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37177155"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="f23ff-103">创建 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="f23ff-103">Create mobileAppContent</span></span>

> <span data-ttu-id="f23ff-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f23ff-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f23ff-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f23ff-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f23ff-106">创建新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f23ff-106">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f23ff-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f23ff-107">Prerequisites</span></span>
<span data-ttu-id="f23ff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f23ff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f23ff-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f23ff-110">Permission type</span></span>|<span data-ttu-id="f23ff-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f23ff-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f23ff-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f23ff-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f23ff-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f23ff-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f23ff-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f23ff-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f23ff-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f23ff-115">Not supported.</span></span>|
|<span data-ttu-id="f23ff-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f23ff-116">Application</span></span>|<span data-ttu-id="f23ff-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f23ff-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f23ff-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f23ff-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="f23ff-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f23ff-119">Request headers</span></span>
|<span data-ttu-id="f23ff-120">标头</span><span class="sxs-lookup"><span data-stu-id="f23ff-120">Header</span></span>|<span data-ttu-id="f23ff-121">值</span><span class="sxs-lookup"><span data-stu-id="f23ff-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f23ff-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f23ff-122">Authorization</span></span>|<span data-ttu-id="f23ff-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f23ff-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f23ff-124">接受</span><span class="sxs-lookup"><span data-stu-id="f23ff-124">Accept</span></span>|<span data-ttu-id="f23ff-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f23ff-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f23ff-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f23ff-126">Request body</span></span>
<span data-ttu-id="f23ff-127">在请求正文中，提供 mobileAppContent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f23ff-127">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="f23ff-128">下表显示创建 mobileAppContent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f23ff-128">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="f23ff-129">属性</span><span class="sxs-lookup"><span data-stu-id="f23ff-129">Property</span></span>|<span data-ttu-id="f23ff-130">类型</span><span class="sxs-lookup"><span data-stu-id="f23ff-130">Type</span></span>|<span data-ttu-id="f23ff-131">说明</span><span class="sxs-lookup"><span data-stu-id="f23ff-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f23ff-132">id</span><span class="sxs-lookup"><span data-stu-id="f23ff-132">id</span></span>|<span data-ttu-id="f23ff-133">String</span><span class="sxs-lookup"><span data-stu-id="f23ff-133">String</span></span>|<span data-ttu-id="f23ff-134">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="f23ff-134">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="f23ff-135">响应</span><span class="sxs-lookup"><span data-stu-id="f23ff-135">Response</span></span>
<span data-ttu-id="f23ff-136">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f23ff-136">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f23ff-137">示例</span><span class="sxs-lookup"><span data-stu-id="f23ff-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="f23ff-138">请求</span><span class="sxs-lookup"><span data-stu-id="f23ff-138">Request</span></span>
<span data-ttu-id="f23ff-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f23ff-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="f23ff-140">响应</span><span class="sxs-lookup"><span data-stu-id="f23ff-140">Response</span></span>
<span data-ttu-id="f23ff-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f23ff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```




