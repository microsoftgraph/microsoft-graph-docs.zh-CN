---
title: extendQualityUpdatesPause 操作
description: 扩展适用于企业 Windows 更新圈的质量更新暂停。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc3d4208d76b1cd4c0c48e649126d2c6e1994491
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51150869"
---
# <a name="extendqualityupdatespause-action"></a><span data-ttu-id="24d20-103">extendQualityUpdatesPause 操作</span><span class="sxs-lookup"><span data-stu-id="24d20-103">extendQualityUpdatesPause action</span></span>

<span data-ttu-id="24d20-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="24d20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="24d20-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="24d20-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="24d20-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="24d20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="24d20-107">扩展适用于企业 Windows 更新圈的质量更新暂停。</span><span class="sxs-lookup"><span data-stu-id="24d20-107">Extend Quality Updates Pause for a Windows Update for Business ring.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="24d20-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="24d20-108">Prerequisites</span></span>
<span data-ttu-id="24d20-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="24d20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="24d20-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="24d20-111">Permission type</span></span>|<span data-ttu-id="24d20-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="24d20-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="24d20-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="24d20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="24d20-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24d20-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="24d20-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="24d20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="24d20-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="24d20-116">Not supported.</span></span>|
|<span data-ttu-id="24d20-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="24d20-117">Application</span></span>|<span data-ttu-id="24d20-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="24d20-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="24d20-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="24d20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/extendQualityUpdatesPause
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration/extendQualityUpdatesPause
POST /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}/extendQualityUpdatesPause
```

## <a name="request-headers"></a><span data-ttu-id="24d20-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="24d20-120">Request headers</span></span>
|<span data-ttu-id="24d20-121">标头</span><span class="sxs-lookup"><span data-stu-id="24d20-121">Header</span></span>|<span data-ttu-id="24d20-122">值</span><span class="sxs-lookup"><span data-stu-id="24d20-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="24d20-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="24d20-123">Authorization</span></span>|<span data-ttu-id="24d20-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="24d20-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="24d20-125">接受</span><span class="sxs-lookup"><span data-stu-id="24d20-125">Accept</span></span>|<span data-ttu-id="24d20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="24d20-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="24d20-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="24d20-127">Request body</span></span>
<span data-ttu-id="24d20-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="24d20-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="24d20-129">响应</span><span class="sxs-lookup"><span data-stu-id="24d20-129">Response</span></span>
<span data-ttu-id="24d20-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="24d20-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="24d20-131">示例</span><span class="sxs-lookup"><span data-stu-id="24d20-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="24d20-132">请求</span><span class="sxs-lookup"><span data-stu-id="24d20-132">Request</span></span>
<span data-ttu-id="24d20-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="24d20-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}/extendQualityUpdatesPause
```

### <a name="response"></a><span data-ttu-id="24d20-134">响应</span><span class="sxs-lookup"><span data-stu-id="24d20-134">Response</span></span>
<span data-ttu-id="24d20-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="24d20-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




