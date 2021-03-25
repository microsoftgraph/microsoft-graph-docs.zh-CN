---
title: 列出 userExperienceAnalyticsImpactingProcesses
description: 列出 userExperienceAnalyticsImpactingProcess 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ce9c93790582d2e91e2dac899bb8ccf6ae71fd27
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153949"
---
# <a name="list-userexperienceanalyticsimpactingprocesses"></a><span data-ttu-id="1a4b7-103">列出 userExperienceAnalyticsImpactingProcesses</span><span class="sxs-lookup"><span data-stu-id="1a4b7-103">List userExperienceAnalyticsImpactingProcesses</span></span>

<span data-ttu-id="1a4b7-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1a4b7-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="1a4b7-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="1a4b7-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="1a4b7-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="1a4b7-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1a4b7-107">列出 [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="1a4b7-107">List properties and relationships of the [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1a4b7-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1a4b7-108">Prerequisites</span></span>
<span data-ttu-id="1a4b7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a4b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a4b7-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a4b7-111">Permission type</span></span>|<span data-ttu-id="1a4b7-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a4b7-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1a4b7-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a4b7-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1a4b7-114">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a4b7-114">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="1a4b7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a4b7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1a4b7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a4b7-116">Not supported.</span></span>|
|<span data-ttu-id="1a4b7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a4b7-117">Application</span></span>|<span data-ttu-id="1a4b7-118">DeviceManagementManagedDevices.Read.All、DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1a4b7-118">DeviceManagementManagedDevices.Read.All, DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="1a4b7-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a4b7-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/userExperienceAnalyticsImpactingProcess
```

## <a name="request-headers"></a><span data-ttu-id="1a4b7-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a4b7-120">Request headers</span></span>
|<span data-ttu-id="1a4b7-121">标头</span><span class="sxs-lookup"><span data-stu-id="1a4b7-121">Header</span></span>|<span data-ttu-id="1a4b7-122">值</span><span class="sxs-lookup"><span data-stu-id="1a4b7-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1a4b7-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a4b7-123">Authorization</span></span>|<span data-ttu-id="1a4b7-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1a4b7-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1a4b7-125">接受</span><span class="sxs-lookup"><span data-stu-id="1a4b7-125">Accept</span></span>|<span data-ttu-id="1a4b7-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1a4b7-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1a4b7-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a4b7-127">Request body</span></span>
<span data-ttu-id="1a4b7-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1a4b7-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a4b7-129">响应</span><span class="sxs-lookup"><span data-stu-id="1a4b7-129">Response</span></span>
<span data-ttu-id="1a4b7-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="1a4b7-130">If successful, this method returns a `200 OK` response code and a collection of [userExperienceAnalyticsImpactingProcess](../resources/intune-devices-userexperienceanalyticsimpactingprocess.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1a4b7-131">示例</span><span class="sxs-lookup"><span data-stu-id="1a4b7-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="1a4b7-132">请求</span><span class="sxs-lookup"><span data-stu-id="1a4b7-132">Request</span></span>
<span data-ttu-id="1a4b7-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a4b7-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsImpactingProcess
```

### <a name="response"></a><span data-ttu-id="1a4b7-134">响应</span><span class="sxs-lookup"><span data-stu-id="1a4b7-134">Response</span></span>
<span data-ttu-id="1a4b7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1a4b7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 414

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.userExperienceAnalyticsImpactingProcess",
      "id": "faefd665-d665-faef-65d6-effa65d6effa",
      "deviceId": "Device Id value",
      "category": "Category value",
      "processName": "Process Name value",
      "description": "Description value",
      "publisher": "Publisher value",
      "impactValue": 3.6666666666666665
    }
  ]
}
```




