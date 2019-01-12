---
title: 列表 userAppInstallStatuses
description: 列出属性和 userAppInstallStatus 对象之间的关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 7638ce7755c655c454022bcf2df5556abac109f4
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985191"
---
# <a name="list-userappinstallstatuses"></a><span data-ttu-id="05869-103">列表 userAppInstallStatuses</span><span class="sxs-lookup"><span data-stu-id="05869-103">List userAppInstallStatuses</span></span>

> <span data-ttu-id="05869-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="05869-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="05869-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="05869-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="05869-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="05869-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="05869-107">列出属性和[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="05869-107">List properties and relationships of the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="05869-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="05869-108">Prerequisites</span></span>
<span data-ttu-id="05869-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="05869-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="05869-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="05869-111">Permission type</span></span>|<span data-ttu-id="05869-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="05869-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="05869-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="05869-113">Delegated (work or school account)</span></span>|<span data-ttu-id="05869-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="05869-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="05869-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="05869-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="05869-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="05869-116">Not supported.</span></span>|
|<span data-ttu-id="05869-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="05869-117">Application</span></span>|<span data-ttu-id="05869-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="05869-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="05869-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="05869-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="05869-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="05869-120">Request headers</span></span>
|<span data-ttu-id="05869-121">标头</span><span class="sxs-lookup"><span data-stu-id="05869-121">Header</span></span>|<span data-ttu-id="05869-122">值</span><span class="sxs-lookup"><span data-stu-id="05869-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="05869-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="05869-123">Authorization</span></span>|<span data-ttu-id="05869-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="05869-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="05869-125">Accept</span><span class="sxs-lookup"><span data-stu-id="05869-125">Accept</span></span>|<span data-ttu-id="05869-126">application/json</span><span class="sxs-lookup"><span data-stu-id="05869-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="05869-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="05869-127">Request body</span></span>
<span data-ttu-id="05869-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="05869-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="05869-129">响应</span><span class="sxs-lookup"><span data-stu-id="05869-129">Response</span></span>
<span data-ttu-id="05869-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="05869-130">If successful, this method returns a `200 OK` response code and a collection of [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="05869-131">示例</span><span class="sxs-lookup"><span data-stu-id="05869-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="05869-132">请求</span><span class="sxs-lookup"><span data-stu-id="05869-132">Request</span></span>
<span data-ttu-id="05869-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="05869-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

### <a name="response"></a><span data-ttu-id="05869-134">响应</span><span class="sxs-lookup"><span data-stu-id="05869-134">Response</span></span>
<span data-ttu-id="05869-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="05869-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 349

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userAppInstallStatus",
      "id": "14959a2a-9a2a-1495-2a9a-95142a9a9514",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value",
      "installedDeviceCount": 4,
      "failedDeviceCount": 1,
      "notInstalledDeviceCount": 7
    }
  ]
}
```





