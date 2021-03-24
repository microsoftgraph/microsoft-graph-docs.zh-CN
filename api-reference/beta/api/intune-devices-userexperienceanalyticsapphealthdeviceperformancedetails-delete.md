---
title: 删除 userExperienceAnalyticsAppHealthDevicePerformanceDetails
description: 删除 userExperienceAnalyticsAppHealthDevicePerformanceDetails。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 54d453a145e2d9a2370dee1d2e07638368757141
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51136053"
---
# <a name="delete-userexperienceanalyticsapphealthdeviceperformancedetails"></a><span data-ttu-id="6c3aa-103">删除 userExperienceAnalyticsAppHealthDevicePerformanceDetails</span><span class="sxs-lookup"><span data-stu-id="6c3aa-103">Delete userExperienceAnalyticsAppHealthDevicePerformanceDetails</span></span>

<span data-ttu-id="6c3aa-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6c3aa-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6c3aa-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6c3aa-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6c3aa-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6c3aa-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6c3aa-107">删除 [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md)。</span><span class="sxs-lookup"><span data-stu-id="6c3aa-107">Deletes a [userExperienceAnalyticsAppHealthDevicePerformanceDetails](../resources/intune-devices-userexperienceanalyticsapphealthdeviceperformancedetails.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6c3aa-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6c3aa-108">Prerequisites</span></span>
<span data-ttu-id="6c3aa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6c3aa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6c3aa-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6c3aa-111">Permission type</span></span>|<span data-ttu-id="6c3aa-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6c3aa-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6c3aa-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6c3aa-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6c3aa-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c3aa-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="6c3aa-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6c3aa-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6c3aa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6c3aa-116">Not supported.</span></span>|
|<span data-ttu-id="6c3aa-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6c3aa-117">Application</span></span>|<span data-ttu-id="6c3aa-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6c3aa-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6c3aa-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6c3aa-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails/{userExperienceAnalyticsAppHealthDevicePerformanceDetailsId}
```

## <a name="request-headers"></a><span data-ttu-id="6c3aa-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6c3aa-120">Request headers</span></span>
|<span data-ttu-id="6c3aa-121">标头</span><span class="sxs-lookup"><span data-stu-id="6c3aa-121">Header</span></span>|<span data-ttu-id="6c3aa-122">值</span><span class="sxs-lookup"><span data-stu-id="6c3aa-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6c3aa-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6c3aa-123">Authorization</span></span>|<span data-ttu-id="6c3aa-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6c3aa-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6c3aa-125">接受</span><span class="sxs-lookup"><span data-stu-id="6c3aa-125">Accept</span></span>|<span data-ttu-id="6c3aa-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6c3aa-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6c3aa-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6c3aa-127">Request body</span></span>
<span data-ttu-id="6c3aa-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6c3aa-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6c3aa-129">响应</span><span class="sxs-lookup"><span data-stu-id="6c3aa-129">Response</span></span>
<span data-ttu-id="6c3aa-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6c3aa-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6c3aa-131">示例</span><span class="sxs-lookup"><span data-stu-id="6c3aa-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="6c3aa-132">请求</span><span class="sxs-lookup"><span data-stu-id="6c3aa-132">Request</span></span>
<span data-ttu-id="6c3aa-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6c3aa-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsAppHealthDevicePerformanceDetails/{userExperienceAnalyticsAppHealthDevicePerformanceDetailsId}
```

### <a name="response"></a><span data-ttu-id="6c3aa-134">响应</span><span class="sxs-lookup"><span data-stu-id="6c3aa-134">Response</span></span>
<span data-ttu-id="6c3aa-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6c3aa-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




