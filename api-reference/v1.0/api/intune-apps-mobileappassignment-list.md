---
title: 列出 mobileAppAssignments
description: 列出 mobileAppAssignment 对象的属性和关系。
author: tfitzmac
ms.openlocfilehash: f4cac347aec66a6b41e260941b72cd71514e4a95
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318016"
---
# <a name="list-mobileappassignments"></a><span data-ttu-id="9cf7a-103">列出 mobileAppAssignments</span><span class="sxs-lookup"><span data-stu-id="9cf7a-103">List mobileAppAssignments</span></span>

> <span data-ttu-id="9cf7a-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="9cf7a-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="9cf7a-105">列出 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9cf7a-105">List properties and relationships of the [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="9cf7a-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="9cf7a-106">Prerequisites</span></span>
<span data-ttu-id="9cf7a-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="9cf7a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cf7a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cf7a-109">Permission type</span></span>|<span data-ttu-id="9cf7a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="9cf7a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cf7a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cf7a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="9cf7a-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="9cf7a-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="9cf7a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cf7a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cf7a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cf7a-114">Not supported.</span></span>|
|<span data-ttu-id="9cf7a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="9cf7a-115">Application</span></span>|<span data-ttu-id="9cf7a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cf7a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cf7a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cf7a-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9cf7a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cf7a-118">Request headers</span></span>
|<span data-ttu-id="9cf7a-119">标头</span><span class="sxs-lookup"><span data-stu-id="9cf7a-119">Header</span></span>|<span data-ttu-id="9cf7a-120">值</span><span class="sxs-lookup"><span data-stu-id="9cf7a-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cf7a-121">授权</span><span class="sxs-lookup"><span data-stu-id="9cf7a-121">Authorization</span></span>|<span data-ttu-id="9cf7a-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9cf7a-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cf7a-123">Accept</span><span class="sxs-lookup"><span data-stu-id="9cf7a-123">Accept</span></span>|<span data-ttu-id="9cf7a-124">application/json</span><span class="sxs-lookup"><span data-stu-id="9cf7a-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cf7a-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cf7a-125">Request body</span></span>
<span data-ttu-id="9cf7a-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9cf7a-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cf7a-127">响应</span><span class="sxs-lookup"><span data-stu-id="9cf7a-127">Response</span></span>
<span data-ttu-id="9cf7a-128">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9cf7a-128">If successful, this method returns a `200 OK` response code and a collection of [mobileAppAssignment](../resources/intune-apps-mobileappassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cf7a-129">示例</span><span class="sxs-lookup"><span data-stu-id="9cf7a-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="9cf7a-130">请求</span><span class="sxs-lookup"><span data-stu-id="9cf7a-130">Request</span></span>
<span data-ttu-id="9cf7a-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9cf7a-131">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/mobileApps/{mobileAppId}/assignments
```

### <a name="response"></a><span data-ttu-id="9cf7a-132">响应</span><span class="sxs-lookup"><span data-stu-id="9cf7a-132">Response</span></span>
<span data-ttu-id="9cf7a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9cf7a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



