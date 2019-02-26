---
title: 删除 sharedPCConfiguration
description: 删除 sharedPCConfiguration。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 545ac5d4963a1b5b739a26fc0f79ec1672964399
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259505"
---
# <a name="delete-sharedpcconfiguration"></a><span data-ttu-id="04afb-103">删除 sharedPCConfiguration</span><span class="sxs-lookup"><span data-stu-id="04afb-103">Delete sharedPCConfiguration</span></span>

> <span data-ttu-id="04afb-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="04afb-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="04afb-105">删除 [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="04afb-105">Deletes a [sharedPCConfiguration](../resources/intune-deviceconfig-sharedpcconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="04afb-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="04afb-106">Prerequisites</span></span>
<span data-ttu-id="04afb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="04afb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="04afb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="04afb-109">Permission type</span></span>|<span data-ttu-id="04afb-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="04afb-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="04afb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="04afb-111">Delegated (work or school account)</span></span>|<span data-ttu-id="04afb-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="04afb-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="04afb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="04afb-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="04afb-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="04afb-114">Not supported.</span></span>|
|<span data-ttu-id="04afb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="04afb-115">Application</span></span>|<span data-ttu-id="04afb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="04afb-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="04afb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="04afb-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="04afb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="04afb-118">Request headers</span></span>
|<span data-ttu-id="04afb-119">标头</span><span class="sxs-lookup"><span data-stu-id="04afb-119">Header</span></span>|<span data-ttu-id="04afb-120">值</span><span class="sxs-lookup"><span data-stu-id="04afb-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="04afb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="04afb-121">Authorization</span></span>|<span data-ttu-id="04afb-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="04afb-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="04afb-123">Accept</span><span class="sxs-lookup"><span data-stu-id="04afb-123">Accept</span></span>|<span data-ttu-id="04afb-124">application/json</span><span class="sxs-lookup"><span data-stu-id="04afb-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="04afb-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="04afb-125">Request body</span></span>
<span data-ttu-id="04afb-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="04afb-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="04afb-127">响应</span><span class="sxs-lookup"><span data-stu-id="04afb-127">Response</span></span>
<span data-ttu-id="04afb-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="04afb-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="04afb-129">示例</span><span class="sxs-lookup"><span data-stu-id="04afb-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="04afb-130">请求</span><span class="sxs-lookup"><span data-stu-id="04afb-130">Request</span></span>
<span data-ttu-id="04afb-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="04afb-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="04afb-132">响应</span><span class="sxs-lookup"><span data-stu-id="04afb-132">Response</span></span>
<span data-ttu-id="04afb-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="04afb-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



