---
title: 列出 mobileAppIntentAndStates
description: 列出 mobileAppIntentAndState 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 220eb7728c80973a68855da6fdc5222e9c059af2
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43473960"
---
# <a name="list-mobileappintentandstates"></a><span data-ttu-id="b4b37-103">列出 mobileAppIntentAndStates</span><span class="sxs-lookup"><span data-stu-id="b4b37-103">List mobileAppIntentAndStates</span></span>

<span data-ttu-id="b4b37-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b4b37-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b4b37-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b4b37-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b4b37-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b4b37-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b4b37-107">列出[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b4b37-107">List properties and relationships of the [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b4b37-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b4b37-108">Prerequisites</span></span>
<span data-ttu-id="b4b37-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b4b37-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b4b37-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b4b37-111">Permission type</span></span>|<span data-ttu-id="b4b37-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b4b37-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b4b37-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b4b37-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b4b37-114">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4b37-114">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|
|<span data-ttu-id="b4b37-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b4b37-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b4b37-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b4b37-116">Not supported.</span></span>|
|<span data-ttu-id="b4b37-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b4b37-117">Application</span></span>|<span data-ttu-id="b4b37-118">DeviceManagementManagedDevices.ReadWrite.All、DeviceManagementManagedDevices.Read.All</span><span class="sxs-lookup"><span data-stu-id="b4b37-118">DeviceManagementManagedDevices.ReadWrite.All, DeviceManagementManagedDevices.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b4b37-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b4b37-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /users/{usersId}/mobileAppIntentAndStates
```

## <a name="request-headers"></a><span data-ttu-id="b4b37-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b4b37-120">Request headers</span></span>
|<span data-ttu-id="b4b37-121">标头</span><span class="sxs-lookup"><span data-stu-id="b4b37-121">Header</span></span>|<span data-ttu-id="b4b37-122">值</span><span class="sxs-lookup"><span data-stu-id="b4b37-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b4b37-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b4b37-123">Authorization</span></span>|<span data-ttu-id="b4b37-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b4b37-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b4b37-125">接受</span><span class="sxs-lookup"><span data-stu-id="b4b37-125">Accept</span></span>|<span data-ttu-id="b4b37-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b4b37-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b4b37-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b4b37-127">Request body</span></span>
<span data-ttu-id="b4b37-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b4b37-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b4b37-129">响应</span><span class="sxs-lookup"><span data-stu-id="b4b37-129">Response</span></span>
<span data-ttu-id="b4b37-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="b4b37-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppIntentAndState](../resources/intune-troubleshooting-mobileappintentandstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b4b37-131">示例</span><span class="sxs-lookup"><span data-stu-id="b4b37-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b4b37-132">请求</span><span class="sxs-lookup"><span data-stu-id="b4b37-132">Request</span></span>
<span data-ttu-id="b4b37-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b4b37-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/users/{usersId}/mobileAppIntentAndStates
```

### <a name="response"></a><span data-ttu-id="b4b37-134">响应</span><span class="sxs-lookup"><span data-stu-id="b4b37-134">Response</span></span>
<span data-ttu-id="b4b37-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b4b37-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 1001

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppIntentAndState",
      "id": "45a775d6-75d6-45a7-d675-a745d675a745",
      "managedDeviceIdentifier": "Managed Device Identifier value",
      "userId": "User Id value",
      "mobileAppList": [
        {
          "@odata.type": "microsoft.graph.mobileAppIntentAndStateDetail",
          "applicationId": "Application Id value",
          "displayName": "Display Name value",
          "mobileAppIntent": "notAvailable",
          "displayVersion": "Display Version value",
          "installState": "failed",
          "supportedDeviceTypes": [
            {
              "@odata.type": "microsoft.graph.mobileAppSupportedDeviceType",
              "type": "windowsRT",
              "minimumOperatingSystemVersion": "Minimum Operating System Version value",
              "maximumOperatingSystemVersion": "Maximum Operating System Version value"
            }
          ]
        }
      ]
    }
  ]
}
```



