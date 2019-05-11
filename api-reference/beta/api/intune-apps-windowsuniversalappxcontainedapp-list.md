---
title: 列出 windowsUniversalAppXContainedApps
description: 列出 windowsUniversalAppXContainedApp 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7c32f9e3457707e82747d72675f42867f15527e1
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934430"
---
# <a name="list-windowsuniversalappxcontainedapps"></a><span data-ttu-id="cbaab-103">列出 windowsUniversalAppXContainedApps</span><span class="sxs-lookup"><span data-stu-id="cbaab-103">List windowsUniversalAppXContainedApps</span></span>

> <span data-ttu-id="cbaab-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cbaab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cbaab-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cbaab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cbaab-106">列出[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cbaab-106">List properties and relationships of the [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cbaab-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cbaab-107">Prerequisites</span></span>
<span data-ttu-id="cbaab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cbaab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cbaab-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cbaab-110">Permission type</span></span>|<span data-ttu-id="cbaab-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cbaab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cbaab-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cbaab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cbaab-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cbaab-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cbaab-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cbaab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cbaab-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbaab-115">Not supported.</span></span>|
|<span data-ttu-id="cbaab-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cbaab-116">Application</span></span>|<span data-ttu-id="cbaab-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cbaab-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cbaab-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cbaab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.microsoftStoreForBusinessApp/containedApps
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.windowsUniversalAppX/committedContainedApps
```

## <a name="request-headers"></a><span data-ttu-id="cbaab-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cbaab-119">Request headers</span></span>
|<span data-ttu-id="cbaab-120">标头</span><span class="sxs-lookup"><span data-stu-id="cbaab-120">Header</span></span>|<span data-ttu-id="cbaab-121">值</span><span class="sxs-lookup"><span data-stu-id="cbaab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cbaab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cbaab-122">Authorization</span></span>|<span data-ttu-id="cbaab-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cbaab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cbaab-124">接受</span><span class="sxs-lookup"><span data-stu-id="cbaab-124">Accept</span></span>|<span data-ttu-id="cbaab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cbaab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cbaab-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cbaab-126">Request body</span></span>
<span data-ttu-id="cbaab-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cbaab-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cbaab-128">响应</span><span class="sxs-lookup"><span data-stu-id="cbaab-128">Response</span></span>
<span data-ttu-id="cbaab-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="cbaab-129">If successful, this method returns a `200 OK` response code and a collection of [windowsUniversalAppXContainedApp](../resources/intune-apps-windowsuniversalappxcontainedapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cbaab-130">示例</span><span class="sxs-lookup"><span data-stu-id="cbaab-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cbaab-131">请求</span><span class="sxs-lookup"><span data-stu-id="cbaab-131">Request</span></span>
<span data-ttu-id="cbaab-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cbaab-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/contentVersions/{mobileAppContentId}/containedApps
```

### <a name="response"></a><span data-ttu-id="cbaab-133">响应</span><span class="sxs-lookup"><span data-stu-id="cbaab-133">Response</span></span>
<span data-ttu-id="cbaab-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cbaab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 216

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsUniversalAppXContainedApp",
      "id": "2d03284a-284a-2d03-4a28-032d4a28032d",
      "appUserModelId": "App User Model Id value"
    }
  ]
}
```




