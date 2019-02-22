---
title: 删除 windows10EasEmailProfileConfiguration
description: 删除 windows10EasEmailProfileConfiguration。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ec9f569c197416b0141979554bed2ac43cc3e6f8
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30141816"
---
# <a name="delete-windows10easemailprofileconfiguration"></a><span data-ttu-id="cd022-103">删除 windows10EasEmailProfileConfiguration</span><span class="sxs-lookup"><span data-stu-id="cd022-103">Delete windows10EasEmailProfileConfiguration</span></span>

> <span data-ttu-id="cd022-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="cd022-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="cd022-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="cd022-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="cd022-106">删除[windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="cd022-106">Deletes a [windows10EasEmailProfileConfiguration](../resources/intune-deviceconfig-windows10easemailprofileconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="cd022-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="cd022-107">Prerequisites</span></span>
<span data-ttu-id="cd022-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="cd022-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="cd022-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cd022-110">Permission type</span></span>|<span data-ttu-id="cd022-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cd022-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cd022-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cd022-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cd022-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cd022-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="cd022-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cd022-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cd022-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd022-115">Not supported.</span></span>|
|<span data-ttu-id="cd022-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cd022-116">Application</span></span>|<span data-ttu-id="cd022-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cd022-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cd022-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cd022-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="cd022-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cd022-119">Request headers</span></span>
|<span data-ttu-id="cd022-120">标头</span><span class="sxs-lookup"><span data-stu-id="cd022-120">Header</span></span>|<span data-ttu-id="cd022-121">值</span><span class="sxs-lookup"><span data-stu-id="cd022-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cd022-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cd022-122">Authorization</span></span>|<span data-ttu-id="cd022-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cd022-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cd022-124">Accept</span><span class="sxs-lookup"><span data-stu-id="cd022-124">Accept</span></span>|<span data-ttu-id="cd022-125">application/json</span><span class="sxs-lookup"><span data-stu-id="cd022-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cd022-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="cd022-126">Request body</span></span>
<span data-ttu-id="cd022-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cd022-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cd022-128">响应</span><span class="sxs-lookup"><span data-stu-id="cd022-128">Response</span></span>
<span data-ttu-id="cd022-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cd022-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cd022-130">示例</span><span class="sxs-lookup"><span data-stu-id="cd022-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="cd022-131">请求</span><span class="sxs-lookup"><span data-stu-id="cd022-131">Request</span></span>
<span data-ttu-id="cd022-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cd022-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="cd022-133">响应</span><span class="sxs-lookup"><span data-stu-id="cd022-133">Response</span></span>
<span data-ttu-id="cd022-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cd022-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




