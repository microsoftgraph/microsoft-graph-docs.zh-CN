---
title: 获取 iosDeviceFeaturesConfiguration
description: 读取 iosDeviceFeaturesConfiguration 对象的属性和关系。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 28a408a6143f0b8499ccc20f63a2e73a0ac69b6c
ms.sourcegitcommit: bd5bb20856d4bffe93b2f77f131664849b602dbb
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/02/2019
ms.locfileid: "37366389"
---
# <a name="get-iosdevicefeaturesconfiguration"></a><span data-ttu-id="5f905-103">获取 iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="5f905-103">Get iosDeviceFeaturesConfiguration</span></span>

> <span data-ttu-id="5f905-104">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5f905-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5f905-105">读取 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="5f905-105">Read properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5f905-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="5f905-106">Prerequisites</span></span>
<span data-ttu-id="5f905-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5f905-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5f905-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5f905-109">Permission type</span></span>|<span data-ttu-id="5f905-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5f905-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5f905-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5f905-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5f905-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="5f905-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="5f905-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5f905-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5f905-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f905-114">Not supported.</span></span>|
|<span data-ttu-id="5f905-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5f905-115">Application</span></span>|<span data-ttu-id="5f905-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5f905-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5f905-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5f905-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="5f905-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="5f905-118">Optional query parameters</span></span>
<span data-ttu-id="5f905-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="5f905-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="5f905-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5f905-120">Request headers</span></span>
|<span data-ttu-id="5f905-121">标头</span><span class="sxs-lookup"><span data-stu-id="5f905-121">Header</span></span>|<span data-ttu-id="5f905-122">值</span><span class="sxs-lookup"><span data-stu-id="5f905-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5f905-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5f905-123">Authorization</span></span>|<span data-ttu-id="5f905-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5f905-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5f905-125">接受</span><span class="sxs-lookup"><span data-stu-id="5f905-125">Accept</span></span>|<span data-ttu-id="5f905-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5f905-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5f905-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5f905-127">Request body</span></span>
<span data-ttu-id="5f905-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="5f905-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="5f905-129">响应</span><span class="sxs-lookup"><span data-stu-id="5f905-129">Response</span></span>
<span data-ttu-id="5f905-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5f905-130">If successful, this method returns a `200 OK` response code and [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5f905-131">示例</span><span class="sxs-lookup"><span data-stu-id="5f905-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="5f905-132">请求</span><span class="sxs-lookup"><span data-stu-id="5f905-132">Request</span></span>
<span data-ttu-id="5f905-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5f905-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="5f905-134">响应</span><span class="sxs-lookup"><span data-stu-id="5f905-134">Response</span></span>
<span data-ttu-id="5f905-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5f905-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2313

{
  "value": {
    "@odata.type": "#microsoft.graph.iosDeviceFeaturesConfiguration",
    "id": "651e0ab3-0ab3-651e-b30a-1e65b30a1e65",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "description": "Description value",
    "displayName": "Display Name value",
    "version": 7,
    "assetTagTemplate": "Asset Tag Template value",
    "lockScreenFootnote": "Lock Screen Footnote value",
    "homeScreenDockIcons": [
      {
        "@odata.type": "microsoft.graph.iosHomeScreenFolder",
        "displayName": "Display Name value",
        "pages": [
          {
            "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
            "displayName": "Display Name value",
            "apps": [
              {
                "@odata.type": "microsoft.graph.iosHomeScreenApp",
                "displayName": "Display Name value",
                "bundleID": "Bundle ID value"
              }
            ]
          }
        ]
      }
    ],
    "homeScreenPages": [
      {
        "@odata.type": "microsoft.graph.iosHomeScreenPage",
        "displayName": "Display Name value",
        "icons": [
          {
            "@odata.type": "microsoft.graph.iosHomeScreenFolder",
            "displayName": "Display Name value",
            "pages": [
              {
                "@odata.type": "microsoft.graph.iosHomeScreenFolderPage",
                "displayName": "Display Name value",
                "apps": [
                  {
                    "@odata.type": "microsoft.graph.iosHomeScreenApp",
                    "displayName": "Display Name value",
                    "bundleID": "Bundle ID value"
                  }
                ]
              }
            ]
          }
        ]
      }
    ],
    "notificationSettings": [
      {
        "@odata.type": "microsoft.graph.iosNotificationSettings",
        "bundleID": "Bundle ID value",
        "appName": "App Name value",
        "publisher": "Publisher value",
        "enabled": true,
        "showInNotificationCenter": true,
        "showOnLockScreen": true,
        "alertType": "banner",
        "badgesEnabled": true,
        "soundsEnabled": true
      }
    ]
  }
}
```




