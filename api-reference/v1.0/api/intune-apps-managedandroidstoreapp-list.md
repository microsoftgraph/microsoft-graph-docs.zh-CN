---
title: 列出 managedAndroidStoreApps
description: 列出 managedAndroidStoreApp 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e2800c42b23b4491d3b5a2e7cc8335c2c998182c
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52754285"
---
# <a name="list-managedandroidstoreapps"></a><span data-ttu-id="0916f-103">列出 managedAndroidStoreApps</span><span class="sxs-lookup"><span data-stu-id="0916f-103">List managedAndroidStoreApps</span></span>

<span data-ttu-id="0916f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0916f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0916f-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0916f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0916f-106">列出 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0916f-106">List properties and relationships of the [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0916f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0916f-107">Prerequisites</span></span>
<span data-ttu-id="0916f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0916f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0916f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0916f-110">Permission type</span></span>|<span data-ttu-id="0916f-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0916f-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0916f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0916f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0916f-113">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0916f-113">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="0916f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0916f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0916f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0916f-115">Not supported.</span></span>|
|<span data-ttu-id="0916f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0916f-116">Application</span></span>|<span data-ttu-id="0916f-117">DeviceManagementApps.Read.All、DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0916f-117">DeviceManagementApps.Read.All, DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0916f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0916f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps
```

## <a name="request-headers"></a><span data-ttu-id="0916f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0916f-119">Request headers</span></span>
|<span data-ttu-id="0916f-120">标头</span><span class="sxs-lookup"><span data-stu-id="0916f-120">Header</span></span>|<span data-ttu-id="0916f-121">值</span><span class="sxs-lookup"><span data-stu-id="0916f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0916f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0916f-122">Authorization</span></span>|<span data-ttu-id="0916f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0916f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0916f-124">接受</span><span class="sxs-lookup"><span data-stu-id="0916f-124">Accept</span></span>|<span data-ttu-id="0916f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0916f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0916f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0916f-126">Request body</span></span>
<span data-ttu-id="0916f-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0916f-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0916f-128">响应</span><span class="sxs-lookup"><span data-stu-id="0916f-128">Response</span></span>
<span data-ttu-id="0916f-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0916f-129">If successful, this method returns a `200 OK` response code and a collection of [managedAndroidStoreApp](../resources/intune-apps-managedandroidstoreapp.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0916f-130">示例</span><span class="sxs-lookup"><span data-stu-id="0916f-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0916f-131">请求</span><span class="sxs-lookup"><span data-stu-id="0916f-131">Request</span></span>
<span data-ttu-id="0916f-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0916f-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps
```

### <a name="response"></a><span data-ttu-id="0916f-133">响应</span><span class="sxs-lookup"><span data-stu-id="0916f-133">Response</span></span>
<span data-ttu-id="0916f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0916f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1405

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedAndroidStoreApp",
      "id": "89e7e991-e991-89e7-91e9-e78991e9e789",
      "displayName": "Display Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "largeIcon": {
        "@odata.type": "microsoft.graph.mimeContent",
        "type": "Type value",
        "value": "dmFsdWU="
      },
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "isFeatured": true,
      "privacyInformationUrl": "https://example.com/privacyInformationUrl/",
      "informationUrl": "https://example.com/informationUrl/",
      "owner": "Owner value",
      "developer": "Developer value",
      "notes": "Notes value",
      "publishingState": "processing",
      "appAvailability": "lineOfBusiness",
      "version": "Version value",
      "packageId": "Package Id value",
      "appStoreUrl": "https://example.com/appStoreUrl/",
      "minimumSupportedOperatingSystem": {
        "@odata.type": "microsoft.graph.androidMinimumOperatingSystem",
        "v4_0": true,
        "v4_0_3": true,
        "v4_1": true,
        "v4_2": true,
        "v4_3": true,
        "v4_4": true,
        "v5_0": true,
        "v5_1": true,
        "v10_0": true,
        "v11_0": true
      }
    }
  ]
}
```




