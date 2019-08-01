---
title: 更新 mobileAppContent
description: 更新 mobileAppContent 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2718dd551a1d9bf1d5210d3d668e0bd26951c6fb
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36002025"
---
# <a name="update-mobileappcontent"></a><span data-ttu-id="6a816-103">更新 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="6a816-103">Update mobileAppContent</span></span>

> <span data-ttu-id="6a816-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6a816-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a816-105">更新 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="6a816-105">Update the properties of a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a816-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="6a816-106">Prerequisites</span></span>
<span data-ttu-id="6a816-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a816-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a816-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a816-109">Permission type</span></span>|<span data-ttu-id="6a816-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6a816-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a816-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a816-111">Delegated (work or school account)</span></span>|<span data-ttu-id="6a816-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a816-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6a816-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a816-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a816-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a816-114">Not supported.</span></span>|
|<span data-ttu-id="6a816-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a816-115">Application</span></span>|<span data-ttu-id="6a816-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a816-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a816-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a816-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions/{mobileAppContentId}
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions/{mobileAppContentId}
```

## <a name="request-headers"></a><span data-ttu-id="6a816-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a816-118">Request headers</span></span>
|<span data-ttu-id="6a816-119">标头</span><span class="sxs-lookup"><span data-stu-id="6a816-119">Header</span></span>|<span data-ttu-id="6a816-120">值</span><span class="sxs-lookup"><span data-stu-id="6a816-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a816-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a816-121">Authorization</span></span>|<span data-ttu-id="6a816-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6a816-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a816-123">接受</span><span class="sxs-lookup"><span data-stu-id="6a816-123">Accept</span></span>|<span data-ttu-id="6a816-124">application/json</span><span class="sxs-lookup"><span data-stu-id="6a816-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a816-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a816-125">Request body</span></span>
<span data-ttu-id="6a816-126">在请求正文中，提供 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a816-126">In the request body, supply a JSON representation for the [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

<span data-ttu-id="6a816-127">下表显示创建 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6a816-127">The following table shows the properties that are required when you create the [mobileAppContent](../resources/intune-apps-mobileappcontent.md).</span></span>

|<span data-ttu-id="6a816-128">属性</span><span class="sxs-lookup"><span data-stu-id="6a816-128">Property</span></span>|<span data-ttu-id="6a816-129">类型</span><span class="sxs-lookup"><span data-stu-id="6a816-129">Type</span></span>|<span data-ttu-id="6a816-130">说明</span><span class="sxs-lookup"><span data-stu-id="6a816-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a816-131">id</span><span class="sxs-lookup"><span data-stu-id="6a816-131">id</span></span>|<span data-ttu-id="6a816-132">String</span><span class="sxs-lookup"><span data-stu-id="6a816-132">String</span></span>|<span data-ttu-id="6a816-133">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="6a816-133">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="6a816-134">响应</span><span class="sxs-lookup"><span data-stu-id="6a816-134">Response</span></span>
<span data-ttu-id="6a816-135">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6a816-135">If successful, this method returns a `200 OK` response code and an updated [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a816-136">示例</span><span class="sxs-lookup"><span data-stu-id="6a816-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a816-137">请求</span><span class="sxs-lookup"><span data-stu-id="6a816-137">Request</span></span>
<span data-ttu-id="6a816-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a816-138">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="6a816-139">响应</span><span class="sxs-lookup"><span data-stu-id="6a816-139">Response</span></span>
<span data-ttu-id="6a816-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6a816-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



