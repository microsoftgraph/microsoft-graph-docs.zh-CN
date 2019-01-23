---
title: 删除 deviceEnrollmentWindowsHelloForBusinessConfiguration
description: 删除 deviceEnrollmentWindowsHelloForBusinessConfiguration。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: df6879a9bc2548b05a50c8b79c8b01eb0879b8b1
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29420484"
---
# <a name="delete-deviceenrollmentwindowshelloforbusinessconfiguration"></a><span data-ttu-id="2ed18-103">删除 deviceEnrollmentWindowsHelloForBusinessConfiguration</span><span class="sxs-lookup"><span data-stu-id="2ed18-103">Delete deviceEnrollmentWindowsHelloForBusinessConfiguration</span></span>

> <span data-ttu-id="2ed18-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="2ed18-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="2ed18-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="2ed18-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="2ed18-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2ed18-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2ed18-107">删除 [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="2ed18-107">Deletes a [deviceEnrollmentWindowsHelloForBusinessConfiguration](../resources/intune-onboarding-deviceenrollmentwindowshelloforbusinessconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2ed18-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2ed18-108">Prerequisites</span></span>
<span data-ttu-id="2ed18-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="2ed18-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="2ed18-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ed18-111">Permission type</span></span>|<span data-ttu-id="2ed18-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2ed18-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ed18-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ed18-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2ed18-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2ed18-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="2ed18-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ed18-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ed18-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ed18-116">Not supported.</span></span>|
|<span data-ttu-id="2ed18-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ed18-117">Application</span></span>|<span data-ttu-id="2ed18-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ed18-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ed18-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ed18-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2ed18-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ed18-120">Request headers</span></span>
|<span data-ttu-id="2ed18-121">标头</span><span class="sxs-lookup"><span data-stu-id="2ed18-121">Header</span></span>|<span data-ttu-id="2ed18-122">值</span><span class="sxs-lookup"><span data-stu-id="2ed18-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2ed18-123">授权</span><span class="sxs-lookup"><span data-stu-id="2ed18-123">Authorization</span></span>|<span data-ttu-id="2ed18-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2ed18-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2ed18-125">Accept</span><span class="sxs-lookup"><span data-stu-id="2ed18-125">Accept</span></span>|<span data-ttu-id="2ed18-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2ed18-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ed18-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ed18-127">Request body</span></span>
<span data-ttu-id="2ed18-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2ed18-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2ed18-129">响应</span><span class="sxs-lookup"><span data-stu-id="2ed18-129">Response</span></span>
<span data-ttu-id="2ed18-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2ed18-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2ed18-131">示例</span><span class="sxs-lookup"><span data-stu-id="2ed18-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2ed18-132">请求</span><span class="sxs-lookup"><span data-stu-id="2ed18-132">Request</span></span>
<span data-ttu-id="2ed18-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2ed18-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}
```

### <a name="response"></a><span data-ttu-id="2ed18-134">响应</span><span class="sxs-lookup"><span data-stu-id="2ed18-134">Response</span></span>
<span data-ttu-id="2ed18-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2ed18-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




