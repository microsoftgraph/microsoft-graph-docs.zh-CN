---
title: 列出 managedDeviceMobileAppConfigurationAssignments
description: 列出 managedDeviceMobileAppConfigurationAssignment 对象的属性和关系。
ms.openlocfilehash: c189801537f0ae191e138edca95080c0cb6d55d6
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044154"
---
# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="cec14-103">列出 managedDeviceMobileAppConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="cec14-103">List managedDeviceMobileAppConfigurationAssignments</span></span>

> <span data-ttu-id="cec14-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cec14-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cec14-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cec14-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cec14-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cec14-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cec14-107">列出 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="cec14-107">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cec14-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cec14-108">Prerequisites</span></span>
<span data-ttu-id="cec14-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cec14-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cec14-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cec14-111">Permission type</span></span>|<span data-ttu-id="cec14-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cec14-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cec14-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cec14-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cec14-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="cec14-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="cec14-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cec14-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cec14-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cec14-116">Not supported.</span></span>|
|<span data-ttu-id="cec14-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cec14-117">Application</span></span>|<span data-ttu-id="cec14-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cec14-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cec14-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cec14-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="cec14-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cec14-120">Request headers</span></span>
|<span data-ttu-id="cec14-121">标头</span><span class="sxs-lookup"><span data-stu-id="cec14-121">Header</span></span>|<span data-ttu-id="cec14-122">值</span><span class="sxs-lookup"><span data-stu-id="cec14-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cec14-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="cec14-123">Authorization</span></span>|<span data-ttu-id="cec14-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cec14-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cec14-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cec14-125">Accept</span></span>|<span data-ttu-id="cec14-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cec14-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cec14-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cec14-127">Request body</span></span>
<span data-ttu-id="cec14-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cec14-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cec14-129">响应</span><span class="sxs-lookup"><span data-stu-id="cec14-129">Response</span></span>
<span data-ttu-id="cec14-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="cec14-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cec14-131">示例</span><span class="sxs-lookup"><span data-stu-id="cec14-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="cec14-132">请求</span><span class="sxs-lookup"><span data-stu-id="cec14-132">Request</span></span>
<span data-ttu-id="cec14-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cec14-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="cec14-134">响应</span><span class="sxs-lookup"><span data-stu-id="cec14-134">Response</span></span>
<span data-ttu-id="cec14-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cec14-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 287

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceMobileAppConfigurationAssignment",
      "id": "4df81c9c-1c9c-4df8-9c1c-f84d9c1cf84d",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





