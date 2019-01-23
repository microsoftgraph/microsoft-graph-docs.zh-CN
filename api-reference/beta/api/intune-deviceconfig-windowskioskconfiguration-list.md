---
title: 列表 windowsKioskConfigurations
description: 列出属性和 windowsKioskConfiguration 对象之间的关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: dbcb11193be435cdea62ec9237eca21517f1db8c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413099"
---
# <a name="list-windowskioskconfigurations"></a><span data-ttu-id="7c9b7-103">列表 windowsKioskConfigurations</span><span class="sxs-lookup"><span data-stu-id="7c9b7-103">List windowsKioskConfigurations</span></span>

> <span data-ttu-id="7c9b7-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="7c9b7-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="7c9b7-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7c9b7-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="7c9b7-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7c9b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7c9b7-107">列出属性和[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="7c9b7-107">List properties and relationships of the [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7c9b7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7c9b7-108">Prerequisites</span></span>
<span data-ttu-id="7c9b7-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="7c9b7-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="7c9b7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7c9b7-111">Permission type</span></span>|<span data-ttu-id="7c9b7-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7c9b7-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7c9b7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7c9b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="7c9b7-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="7c9b7-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="7c9b7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7c9b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7c9b7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c9b7-116">Not supported.</span></span>|
|<span data-ttu-id="7c9b7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7c9b7-117">Application</span></span>|<span data-ttu-id="7c9b7-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7c9b7-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7c9b7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7c9b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="7c9b7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7c9b7-120">Request headers</span></span>
|<span data-ttu-id="7c9b7-121">标头</span><span class="sxs-lookup"><span data-stu-id="7c9b7-121">Header</span></span>|<span data-ttu-id="7c9b7-122">值</span><span class="sxs-lookup"><span data-stu-id="7c9b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7c9b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7c9b7-123">Authorization</span></span>|<span data-ttu-id="7c9b7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7c9b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7c9b7-125">Accept</span><span class="sxs-lookup"><span data-stu-id="7c9b7-125">Accept</span></span>|<span data-ttu-id="7c9b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="7c9b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7c9b7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="7c9b7-127">Request body</span></span>
<span data-ttu-id="7c9b7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7c9b7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7c9b7-129">响应</span><span class="sxs-lookup"><span data-stu-id="7c9b7-129">Response</span></span>
<span data-ttu-id="7c9b7-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="7c9b7-130">If successful, this method returns a `200 OK` response code and a collection of [windowsKioskConfiguration](../resources/intune-deviceconfig-windowskioskconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7c9b7-131">示例</span><span class="sxs-lookup"><span data-stu-id="7c9b7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="7c9b7-132">请求</span><span class="sxs-lookup"><span data-stu-id="7c9b7-132">Request</span></span>
<span data-ttu-id="7c9b7-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7c9b7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="7c9b7-134">响应</span><span class="sxs-lookup"><span data-stu-id="7c9b7-134">Response</span></span>
<span data-ttu-id="7c9b7-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7c9b7-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 2136

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsKioskConfiguration",
      "id": "146a990b-990b-146a-0b99-6a140b996a14",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "kioskProfiles": [
        {
          "@odata.type": "microsoft.graph.windowsKioskProfile",
          "profileId": "Profile Id value",
          "profileName": "Profile Name value",
          "appConfiguration": {
            "@odata.type": "microsoft.graph.windowsKioskMultipleApps",
            "apps": [
              {
                "@odata.type": "microsoft.graph.windowsKioskUWPApp",
                "startLayoutTileSize": "small",
                "name": "Name value",
                "appType": "store",
                "appUserModelId": "App User Model Id value",
                "appId": "App Id value",
                "containedAppId": "Contained App Id value"
              }
            ],
            "showTaskBar": true,
            "disallowDesktopApps": true,
            "startMenuLayoutXml": "c3RhcnRNZW51TGF5b3V0WG1s"
          },
          "userAccountsConfiguration": [
            {
              "@odata.type": "microsoft.graph.windowsKioskVisitor"
            }
          ]
        }
      ],
      "kioskBrowserDefaultUrl": "https://example.com/kioskBrowserDefaultUrl/",
      "kioskBrowserEnableHomeButton": true,
      "kioskBrowserEnableNavigationButtons": true,
      "kioskBrowserEnableEndSessionButton": true,
      "kioskBrowserRestartOnIdleTimeInMinutes": 6,
      "kioskBrowserBlockedURLs": [
        "Kiosk Browser Blocked URLs value"
      ],
      "kioskBrowserBlockedUrlExceptions": [
        "Kiosk Browser Blocked Url Exceptions value"
      ],
      "edgeKioskEnablePublicBrowsing": true,
      "edgeKioskResetAfterIdleTimeInMinutes": 4
    }
  ]
}
```




