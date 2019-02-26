---
title: 删除 androidCustomConfiguration
description: 删除 androidCustomConfiguration。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ebb060f72a006168bef0fd9dc67e390c1e1725be
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30255281"
---
# <a name="delete-androidcustomconfiguration"></a><span data-ttu-id="aad91-103">删除 androidCustomConfiguration</span><span class="sxs-lookup"><span data-stu-id="aad91-103">Delete androidCustomConfiguration</span></span>

> <span data-ttu-id="aad91-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="aad91-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="aad91-105">删除 [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="aad91-105">Deletes a [androidCustomConfiguration](../resources/intune-deviceconfig-androidcustomconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="aad91-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="aad91-106">Prerequisites</span></span>
<span data-ttu-id="aad91-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="aad91-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="aad91-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="aad91-109">Permission type</span></span>|<span data-ttu-id="aad91-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="aad91-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="aad91-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aad91-111">Delegated (work or school account)</span></span>|<span data-ttu-id="aad91-112">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="aad91-112">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="aad91-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aad91-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="aad91-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="aad91-114">Not supported.</span></span>|
|<span data-ttu-id="aad91-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="aad91-115">Application</span></span>|<span data-ttu-id="aad91-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="aad91-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="aad91-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aad91-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="aad91-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="aad91-118">Request headers</span></span>
|<span data-ttu-id="aad91-119">标头</span><span class="sxs-lookup"><span data-stu-id="aad91-119">Header</span></span>|<span data-ttu-id="aad91-120">值</span><span class="sxs-lookup"><span data-stu-id="aad91-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="aad91-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="aad91-121">Authorization</span></span>|<span data-ttu-id="aad91-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="aad91-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="aad91-123">Accept</span><span class="sxs-lookup"><span data-stu-id="aad91-123">Accept</span></span>|<span data-ttu-id="aad91-124">application/json</span><span class="sxs-lookup"><span data-stu-id="aad91-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="aad91-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="aad91-125">Request body</span></span>
<span data-ttu-id="aad91-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="aad91-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="aad91-127">响应</span><span class="sxs-lookup"><span data-stu-id="aad91-127">Response</span></span>
<span data-ttu-id="aad91-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="aad91-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="aad91-129">示例</span><span class="sxs-lookup"><span data-stu-id="aad91-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="aad91-130">请求</span><span class="sxs-lookup"><span data-stu-id="aad91-130">Request</span></span>
<span data-ttu-id="aad91-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aad91-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="aad91-132">响应</span><span class="sxs-lookup"><span data-stu-id="aad91-132">Response</span></span>
<span data-ttu-id="aad91-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aad91-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



