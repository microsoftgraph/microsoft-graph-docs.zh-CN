---
title: 获取 userExperienceAnalyticsDeviceStartupProcess
description: 读取 userExperienceAnalyticsDeviceStartupProcess 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: dc0cd0e174add6eac798dfa1ca2705771aca85e8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51154089"
---
# <a name="get-userexperienceanalyticsdevicestartupprocess"></a><span data-ttu-id="fda85-103">获取 userExperienceAnalyticsDeviceStartupProcess</span><span class="sxs-lookup"><span data-stu-id="fda85-103">Get userExperienceAnalyticsDeviceStartupProcess</span></span>

<span data-ttu-id="fda85-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fda85-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fda85-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="fda85-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="fda85-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fda85-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fda85-107">读取 [userExperienceAnalyticsDeviceStartupProcess 对象的属性和](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="fda85-107">Read properties and relationships of the [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fda85-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fda85-108">Prerequisites</span></span>
<span data-ttu-id="fda85-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fda85-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fda85-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fda85-111">Permission type</span></span>|<span data-ttu-id="fda85-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fda85-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fda85-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fda85-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fda85-114">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fda85-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="fda85-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fda85-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fda85-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fda85-116">Not supported.</span></span>|
|<span data-ttu-id="fda85-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fda85-117">Application</span></span>|<span data-ttu-id="fda85-118">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fda85-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="fda85-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fda85-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="fda85-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="fda85-120">Optional query parameters</span></span>
<span data-ttu-id="fda85-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="fda85-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="fda85-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="fda85-122">Request headers</span></span>
|<span data-ttu-id="fda85-123">标头</span><span class="sxs-lookup"><span data-stu-id="fda85-123">Header</span></span>|<span data-ttu-id="fda85-124">值</span><span class="sxs-lookup"><span data-stu-id="fda85-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fda85-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="fda85-125">Authorization</span></span>|<span data-ttu-id="fda85-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fda85-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fda85-127">接受</span><span class="sxs-lookup"><span data-stu-id="fda85-127">Accept</span></span>|<span data-ttu-id="fda85-128">application/json</span><span class="sxs-lookup"><span data-stu-id="fda85-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fda85-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="fda85-129">Request body</span></span>
<span data-ttu-id="fda85-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fda85-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fda85-131">响应</span><span class="sxs-lookup"><span data-stu-id="fda85-131">Response</span></span>
<span data-ttu-id="fda85-132">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fda85-132">If successful, this method returns a `200 OK` response code and [userExperienceAnalyticsDeviceStartupProcess](../resources/intune-devices-userexperienceanalyticsdevicestartupprocess.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fda85-133">示例</span><span class="sxs-lookup"><span data-stu-id="fda85-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="fda85-134">请求</span><span class="sxs-lookup"><span data-stu-id="fda85-134">Request</span></span>
<span data-ttu-id="fda85-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fda85-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsDeviceStartupProcesses/{userExperienceAnalyticsDeviceStartupProcessId}
```

### <a name="response"></a><span data-ttu-id="fda85-136">响应</span><span class="sxs-lookup"><span data-stu-id="fda85-136">Response</span></span>
<span data-ttu-id="fda85-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fda85-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 358

{
  "value": {
    "@odata.type": "#microsoft.graph.userExperienceAnalyticsDeviceStartupProcess",
    "id": "03b451e6-51e6-03b4-e651-b403e651b403",
    "managedDeviceId": "Managed Device Id value",
    "processName": "Process Name value",
    "productName": "Product Name value",
    "publisher": "Publisher value",
    "startupImpactInMs": 1
  }
}
```




