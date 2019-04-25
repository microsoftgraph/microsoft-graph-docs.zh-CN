---
title: 创建 mobileAppContent
description: 创建新的 mobileAppContent 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ce39017036717efa679384d0efa15423ffb7e97c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32541645"
---
# <a name="create-mobileappcontent"></a><span data-ttu-id="09b08-103">创建 mobileAppContent</span><span class="sxs-lookup"><span data-stu-id="09b08-103">Create mobileAppContent</span></span>

> <span data-ttu-id="09b08-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="09b08-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="09b08-105">创建新的 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="09b08-105">Create a new [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="09b08-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="09b08-106">Prerequisites</span></span>
<span data-ttu-id="09b08-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="09b08-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="09b08-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="09b08-109">Permission type</span></span>|<span data-ttu-id="09b08-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="09b08-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="09b08-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="09b08-111">Delegated (work or school account)</span></span>|<span data-ttu-id="09b08-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="09b08-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="09b08-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="09b08-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="09b08-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="09b08-114">Not supported.</span></span>|
|<span data-ttu-id="09b08-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="09b08-115">Application</span></span>|<span data-ttu-id="09b08-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="09b08-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="09b08-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="09b08-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.mobileLobApp/contentVersions
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.managedMobileLobApp/contentVersions
```

## <a name="request-headers"></a><span data-ttu-id="09b08-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="09b08-118">Request headers</span></span>
|<span data-ttu-id="09b08-119">标头</span><span class="sxs-lookup"><span data-stu-id="09b08-119">Header</span></span>|<span data-ttu-id="09b08-120">值</span><span class="sxs-lookup"><span data-stu-id="09b08-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="09b08-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="09b08-121">Authorization</span></span>|<span data-ttu-id="09b08-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="09b08-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="09b08-123">接受</span><span class="sxs-lookup"><span data-stu-id="09b08-123">Accept</span></span>|<span data-ttu-id="09b08-124">application/json</span><span class="sxs-lookup"><span data-stu-id="09b08-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="09b08-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="09b08-125">Request body</span></span>
<span data-ttu-id="09b08-126">在请求正文中，提供 mobileAppContent 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="09b08-126">In the request body, supply a JSON representation for the mobileAppContent object.</span></span>

<span data-ttu-id="09b08-127">下表显示创建 mobileAppContent 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="09b08-127">The following table shows the properties that are required when you create the mobileAppContent.</span></span>

|<span data-ttu-id="09b08-128">属性</span><span class="sxs-lookup"><span data-stu-id="09b08-128">Property</span></span>|<span data-ttu-id="09b08-129">类型</span><span class="sxs-lookup"><span data-stu-id="09b08-129">Type</span></span>|<span data-ttu-id="09b08-130">说明</span><span class="sxs-lookup"><span data-stu-id="09b08-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="09b08-131">id</span><span class="sxs-lookup"><span data-stu-id="09b08-131">id</span></span>|<span data-ttu-id="09b08-132">String</span><span class="sxs-lookup"><span data-stu-id="09b08-132">String</span></span>|<span data-ttu-id="09b08-133">应用内容版本。</span><span class="sxs-lookup"><span data-stu-id="09b08-133">The app content version.</span></span>|



## <a name="response"></a><span data-ttu-id="09b08-134">响应</span><span class="sxs-lookup"><span data-stu-id="09b08-134">Response</span></span>
<span data-ttu-id="09b08-135">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [mobileAppContent](../resources/intune-apps-mobileappcontent.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="09b08-135">If successful, this method returns a `201 Created` response code and a [mobileAppContent](../resources/intune-apps-mobileappcontent.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="09b08-136">示例</span><span class="sxs-lookup"><span data-stu-id="09b08-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="09b08-137">请求</span><span class="sxs-lookup"><span data-stu-id="09b08-137">Request</span></span>
<span data-ttu-id="09b08-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="09b08-138">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions
Content-type: application/json
Content-length: 58

{
  "@odata.type": "#microsoft.graph.mobileAppContent"
}
```

### <a name="response"></a><span data-ttu-id="09b08-139">响应</span><span class="sxs-lookup"><span data-stu-id="09b08-139">Response</span></span>
<span data-ttu-id="09b08-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="09b08-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 107

{
  "@odata.type": "#microsoft.graph.mobileAppContent",
  "id": "fe0bb9a9-b9a9-fe0b-a9b9-0bfea9b90bfe"
}
```



