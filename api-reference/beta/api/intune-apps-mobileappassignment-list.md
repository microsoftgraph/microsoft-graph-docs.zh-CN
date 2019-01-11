---
title: 列出 mobileAppAssignments
description: 列出 mobileAppAssignment 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 0c412c05a0a9e0755aba7b933379b7eda3e26a50
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27870173"
---
# <a name="list-mobileappassignments"></a><span data-ttu-id="10ecd-103">列出 mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="10ecd-103">List mobileAppAssignments</span></span>

> <span data-ttu-id="10ecd-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="10ecd-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="10ecd-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="10ecd-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="10ecd-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="10ecd-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="10ecd-107">列出 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="10ecd-107">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="10ecd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="10ecd-108">Prerequisites</span></span>
<span data-ttu-id="10ecd-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="10ecd-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="10ecd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="10ecd-111">Permission type</span></span>|<span data-ttu-id="10ecd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="10ecd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="10ecd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="10ecd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="10ecd-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="10ecd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="10ecd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="10ecd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="10ecd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="10ecd-116">Not supported.</span></span>|
|<span data-ttu-id="10ecd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="10ecd-117">Application</span></span>|<span data-ttu-id="10ecd-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="10ecd-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="10ecd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="10ecd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="10ecd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="10ecd-120">Request headers</span></span>
|<span data-ttu-id="10ecd-121">标头</span><span class="sxs-lookup"><span data-stu-id="10ecd-121">Header</span></span>|<span data-ttu-id="10ecd-122">值</span><span class="sxs-lookup"><span data-stu-id="10ecd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="10ecd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="10ecd-123">Authorization</span></span>|<span data-ttu-id="10ecd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="10ecd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="10ecd-125">Accept</span><span class="sxs-lookup"><span data-stu-id="10ecd-125">Accept</span></span>|<span data-ttu-id="10ecd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="10ecd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="10ecd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="10ecd-127">Request body</span></span>
<span data-ttu-id="10ecd-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="10ecd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="10ecd-129">响应</span><span class="sxs-lookup"><span data-stu-id="10ecd-129">Response</span></span>
<span data-ttu-id="10ecd-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="10ecd-130">If successful, this method returns a `200 OK` response code and a collection of [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="10ecd-131">示例</span><span class="sxs-lookup"><span data-stu-id="10ecd-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="10ecd-132">请求</span><span class="sxs-lookup"><span data-stu-id="10ecd-132">Request</span></span>
<span data-ttu-id="10ecd-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="10ecd-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

### <a name="response"></a><span data-ttu-id="10ecd-134">响应</span><span class="sxs-lookup"><span data-stu-id="10ecd-134">Response</span></span>
<span data-ttu-id="10ecd-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="10ecd-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 391

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.mobileAppAssignment",
      "id": "591620b7-20b7-5916-b720-1659b7201659",
      "intent": "required",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      },
      "settings": {
        "@odata.type": "microsoft.graph.mobileAppAssignmentSettings"
      }
    }
  ]
}
```





