---
title: 获取 iosDeviceFeaturesConfiguration
description: 读取 iosDeviceFeaturesConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4d61486a55731e74da88553e3d73ec53c8a90685
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52747961"
---
# <a name="get-iosdevicefeaturesconfiguration"></a><span data-ttu-id="c690c-103">获取 iosDeviceFeaturesConfiguration</span><span class="sxs-lookup"><span data-stu-id="c690c-103">Get iosDeviceFeaturesConfiguration</span></span>

<span data-ttu-id="c690c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c690c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c690c-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c690c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c690c-106">读取 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="c690c-106">Read properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c690c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c690c-107">Prerequisites</span></span>
<span data-ttu-id="c690c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c690c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c690c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c690c-110">Permission type</span></span>|<span data-ttu-id="c690c-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c690c-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c690c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c690c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c690c-113">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c690c-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c690c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c690c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c690c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c690c-115">Not supported.</span></span>|
|<span data-ttu-id="c690c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c690c-116">Application</span></span>|<span data-ttu-id="c690c-117">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c690c-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c690c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c690c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="c690c-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="c690c-119">Optional query parameters</span></span>
<span data-ttu-id="c690c-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="c690c-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="c690c-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="c690c-121">Request headers</span></span>
|<span data-ttu-id="c690c-122">标头</span><span class="sxs-lookup"><span data-stu-id="c690c-122">Header</span></span>|<span data-ttu-id="c690c-123">值</span><span class="sxs-lookup"><span data-stu-id="c690c-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c690c-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="c690c-124">Authorization</span></span>|<span data-ttu-id="c690c-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c690c-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c690c-126">接受</span><span class="sxs-lookup"><span data-stu-id="c690c-126">Accept</span></span>|<span data-ttu-id="c690c-127">application/json</span><span class="sxs-lookup"><span data-stu-id="c690c-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c690c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="c690c-128">Request body</span></span>
<span data-ttu-id="c690c-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c690c-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c690c-130">响应</span><span class="sxs-lookup"><span data-stu-id="c690c-130">Response</span></span>
<span data-ttu-id="c690c-131">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c690c-131">If successful, this method returns a `200 OK` response code and [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c690c-132">示例</span><span class="sxs-lookup"><span data-stu-id="c690c-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="c690c-133">请求</span><span class="sxs-lookup"><span data-stu-id="c690c-133">Request</span></span>
<span data-ttu-id="c690c-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c690c-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="c690c-135">响应</span><span class="sxs-lookup"><span data-stu-id="c690c-135">Response</span></span>
<span data-ttu-id="c690c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c690c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




