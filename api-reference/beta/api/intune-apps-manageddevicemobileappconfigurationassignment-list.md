---
title: 列出 managedDeviceMobileAppConfigurationAssignments
description: 列出 managedDeviceMobileAppConfigurationAssignment 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 11f7dc83e20a1eb316a9dfcdd66eb1de0ca9cea0
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27980487"
---
# <a name="list-manageddevicemobileappconfigurationassignments"></a><span data-ttu-id="45d75-103">列出 managedDeviceMobileAppConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="45d75-103">List managedDeviceMobileAppConfigurationAssignments</span></span>

> <span data-ttu-id="45d75-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="45d75-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45d75-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="45d75-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="45d75-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="45d75-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45d75-107">列出 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="45d75-107">List properties and relationships of the [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45d75-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="45d75-108">Prerequisites</span></span>
<span data-ttu-id="45d75-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="45d75-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45d75-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="45d75-111">Permission type</span></span>|<span data-ttu-id="45d75-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="45d75-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45d75-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45d75-113">Delegated (work or school account)</span></span>|<span data-ttu-id="45d75-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="45d75-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="45d75-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45d75-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45d75-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="45d75-116">Not supported.</span></span>|
|<span data-ttu-id="45d75-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="45d75-117">Application</span></span>|<span data-ttu-id="45d75-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="45d75-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45d75-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45d75-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="45d75-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="45d75-120">Request headers</span></span>
|<span data-ttu-id="45d75-121">标头</span><span class="sxs-lookup"><span data-stu-id="45d75-121">Header</span></span>|<span data-ttu-id="45d75-122">值</span><span class="sxs-lookup"><span data-stu-id="45d75-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45d75-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="45d75-123">Authorization</span></span>|<span data-ttu-id="45d75-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="45d75-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45d75-125">Accept</span><span class="sxs-lookup"><span data-stu-id="45d75-125">Accept</span></span>|<span data-ttu-id="45d75-126">application/json</span><span class="sxs-lookup"><span data-stu-id="45d75-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45d75-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="45d75-127">Request body</span></span>
<span data-ttu-id="45d75-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="45d75-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45d75-129">响应</span><span class="sxs-lookup"><span data-stu-id="45d75-129">Response</span></span>
<span data-ttu-id="45d75-130">如果成功，此方法会在响应正文中返回 `200 OK` 响应代码和 [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="45d75-130">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceMobileAppConfigurationAssignment](../resources/intune-apps-manageddevicemobileappconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45d75-131">示例</span><span class="sxs-lookup"><span data-stu-id="45d75-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="45d75-132">请求</span><span class="sxs-lookup"><span data-stu-id="45d75-132">Request</span></span>
<span data-ttu-id="45d75-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="45d75-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/mobileAppConfigurations/{managedDeviceMobileAppConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="45d75-134">响应</span><span class="sxs-lookup"><span data-stu-id="45d75-134">Response</span></span>
<span data-ttu-id="45d75-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="45d75-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





