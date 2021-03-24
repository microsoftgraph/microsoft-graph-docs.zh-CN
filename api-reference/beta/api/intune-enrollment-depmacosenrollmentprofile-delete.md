---
title: 删除 depMacOSEnrollmentProfile
description: 删除 depMacOSEnrollmentProfile。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0509c9d16c6fc746c477f6ba6a9e3f58659ad223
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51135773"
---
# <a name="delete-depmacosenrollmentprofile"></a><span data-ttu-id="bd46e-103">删除 depMacOSEnrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="bd46e-103">Delete depMacOSEnrollmentProfile</span></span>

<span data-ttu-id="bd46e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd46e-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd46e-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bd46e-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd46e-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bd46e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd46e-107">删除 [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="bd46e-107">Deletes a [depMacOSEnrollmentProfile](../resources/intune-enrollment-depmacosenrollmentprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd46e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bd46e-108">Prerequisites</span></span>
<span data-ttu-id="bd46e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd46e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd46e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd46e-111">Permission type</span></span>|<span data-ttu-id="bd46e-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="bd46e-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd46e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd46e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd46e-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd46e-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="bd46e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd46e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd46e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd46e-116">Not supported.</span></span>|
|<span data-ttu-id="bd46e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd46e-117">Application</span></span>|<span data-ttu-id="bd46e-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd46e-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd46e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd46e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

## <a name="request-headers"></a><span data-ttu-id="bd46e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd46e-120">Request headers</span></span>
|<span data-ttu-id="bd46e-121">标头</span><span class="sxs-lookup"><span data-stu-id="bd46e-121">Header</span></span>|<span data-ttu-id="bd46e-122">值</span><span class="sxs-lookup"><span data-stu-id="bd46e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd46e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd46e-123">Authorization</span></span>|<span data-ttu-id="bd46e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bd46e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd46e-125">接受</span><span class="sxs-lookup"><span data-stu-id="bd46e-125">Accept</span></span>|<span data-ttu-id="bd46e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd46e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd46e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd46e-127">Request body</span></span>
<span data-ttu-id="bd46e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="bd46e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="bd46e-129">响应</span><span class="sxs-lookup"><span data-stu-id="bd46e-129">Response</span></span>
<span data-ttu-id="bd46e-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="bd46e-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="bd46e-131">示例</span><span class="sxs-lookup"><span data-stu-id="bd46e-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd46e-132">请求</span><span class="sxs-lookup"><span data-stu-id="bd46e-132">Request</span></span>
<span data-ttu-id="bd46e-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bd46e-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/defaultMacOsEnrollmentProfile
```

### <a name="response"></a><span data-ttu-id="bd46e-134">响应</span><span class="sxs-lookup"><span data-stu-id="bd46e-134">Response</span></span>
<span data-ttu-id="bd46e-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bd46e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




