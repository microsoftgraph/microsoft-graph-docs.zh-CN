---
title: 列表 iosVppAppAssignedLicenses
description: 列出属性和 iosVppAppAssignedLicense 对象之间的关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: b02e35b7f0d2a6f64c2e1e891db6a6ae066be90b
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27883209"
---
# <a name="list-iosvppappassignedlicenses"></a><span data-ttu-id="1de91-103">列表 iosVppAppAssignedLicenses</span><span class="sxs-lookup"><span data-stu-id="1de91-103">List iosVppAppAssignedLicenses</span></span>

> <span data-ttu-id="1de91-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1de91-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1de91-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1de91-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1de91-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1de91-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1de91-107">列出属性和[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象之间的关系。</span><span class="sxs-lookup"><span data-stu-id="1de91-107">List properties and relationships of the [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1de91-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1de91-108">Prerequisites</span></span>
<span data-ttu-id="1de91-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1de91-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1de91-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1de91-111">Permission type</span></span>|<span data-ttu-id="1de91-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1de91-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1de91-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1de91-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1de91-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="1de91-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="1de91-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1de91-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1de91-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1de91-116">Not supported.</span></span>|
|<span data-ttu-id="1de91-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1de91-117">Application</span></span>|<span data-ttu-id="1de91-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1de91-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1de91-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1de91-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="1de91-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1de91-120">Request headers</span></span>
|<span data-ttu-id="1de91-121">标头</span><span class="sxs-lookup"><span data-stu-id="1de91-121">Header</span></span>|<span data-ttu-id="1de91-122">值</span><span class="sxs-lookup"><span data-stu-id="1de91-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1de91-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1de91-123">Authorization</span></span>|<span data-ttu-id="1de91-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1de91-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1de91-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1de91-125">Accept</span></span>|<span data-ttu-id="1de91-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1de91-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1de91-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1de91-127">Request body</span></span>
<span data-ttu-id="1de91-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1de91-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1de91-129">响应</span><span class="sxs-lookup"><span data-stu-id="1de91-129">Response</span></span>
<span data-ttu-id="1de91-130">如果成功，此方法返回`200 OK`响应代码和响应正文中的[iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)对象的集合。</span><span class="sxs-lookup"><span data-stu-id="1de91-130">If successful, this method returns a `200 OK` response code and a collection of [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1de91-131">示例</span><span class="sxs-lookup"><span data-stu-id="1de91-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="1de91-132">请求</span><span class="sxs-lookup"><span data-stu-id="1de91-132">Request</span></span>
<span data-ttu-id="1de91-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1de91-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

### <a name="response"></a><span data-ttu-id="1de91-134">响应</span><span class="sxs-lookup"><span data-stu-id="1de91-134">Response</span></span>
<span data-ttu-id="1de91-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1de91-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 340

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.iosVppAppAssignedLicense",
      "id": "090a8d2e-8d2e-090a-2e8d-0a092e8d0a09",
      "userEmailAddress": "User Email Address value",
      "userId": "User Id value",
      "userName": "User Name value",
      "userPrincipalName": "User Principal Name value"
    }
  ]
}
```





