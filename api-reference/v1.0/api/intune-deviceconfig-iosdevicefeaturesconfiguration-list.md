---
title: 列出 iosDeviceFeaturesConfigurations
description: 列出 iosDeviceFeaturesConfiguration 对象的属性和关系。
ms.openlocfilehash: 2a284ffa457e5ef2289d731a034e0f02fa5c1515
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008517"
---
# <a name="list-iosdevicefeaturesconfigurations"></a><span data-ttu-id="fd07e-103">列出 iosDeviceFeaturesConfigurations</span><span class="sxs-lookup"><span data-stu-id="fd07e-103">List iosDeviceFeaturesConfigurations</span></span>

> <span data-ttu-id="fd07e-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fd07e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fd07e-105">列出 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="fd07e-105">List properties and relationships of the [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fd07e-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="fd07e-106">Prerequisites</span></span>
<span data-ttu-id="fd07e-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="fd07e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fd07e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="fd07e-109">Permission type</span></span>|<span data-ttu-id="fd07e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fd07e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fd07e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fd07e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="fd07e-112">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="fd07e-112">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="fd07e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fd07e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fd07e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd07e-114">Not supported.</span></span>|
|<span data-ttu-id="fd07e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="fd07e-115">Application</span></span>|<span data-ttu-id="fd07e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fd07e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fd07e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fd07e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="fd07e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="fd07e-118">Request headers</span></span>
|<span data-ttu-id="fd07e-119">标头</span><span class="sxs-lookup"><span data-stu-id="fd07e-119">Header</span></span>|<span data-ttu-id="fd07e-120">值</span><span class="sxs-lookup"><span data-stu-id="fd07e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fd07e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="fd07e-121">Authorization</span></span>|<span data-ttu-id="fd07e-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fd07e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fd07e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="fd07e-123">Accept</span></span>|<span data-ttu-id="fd07e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="fd07e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fd07e-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="fd07e-125">Request body</span></span>
<span data-ttu-id="fd07e-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fd07e-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fd07e-127">响应</span><span class="sxs-lookup"><span data-stu-id="fd07e-127">Response</span></span>
<span data-ttu-id="fd07e-128">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="fd07e-128">If successful, this method returns a `200 OK` response code and a collection of [iosDeviceFeaturesConfiguration](../resources/intune-deviceconfig-iosdevicefeaturesconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fd07e-129">示例</span><span class="sxs-lookup"><span data-stu-id="fd07e-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="fd07e-130">请求</span><span class="sxs-lookup"><span data-stu-id="fd07e-130">Request</span></span>
<span data-ttu-id="fd07e-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fd07e-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="fd07e-132">响应</span><span class="sxs-lookup"><span data-stu-id="fd07e-132">Response</span></span>
<span data-ttu-id="fd07e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fd07e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2461

{
  "value": [
    {
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
  ]
}
```



