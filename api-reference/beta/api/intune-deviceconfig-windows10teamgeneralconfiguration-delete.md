---
title: 删除 windows10TeamGeneralConfiguration
description: 删除 windows10TeamGeneralConfiguration。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d954a7c8832c451e09961844dd8d514ea68e086a
ms.sourcegitcommit: 86903a4730bbd825eabb7f0a1b2429723cc8b1e6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/26/2019
ms.locfileid: "37182167"
---
# <a name="delete-windows10teamgeneralconfiguration"></a><span data-ttu-id="d3931-103">删除 windows10TeamGeneralConfiguration</span><span class="sxs-lookup"><span data-stu-id="d3931-103">Delete windows10TeamGeneralConfiguration</span></span>

> <span data-ttu-id="d3931-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d3931-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d3931-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d3931-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d3931-106">删除 [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="d3931-106">Deletes a [windows10TeamGeneralConfiguration](../resources/intune-deviceconfig-windows10teamgeneralconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d3931-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d3931-107">Prerequisites</span></span>
<span data-ttu-id="d3931-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d3931-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d3931-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d3931-110">Permission type</span></span>|<span data-ttu-id="d3931-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d3931-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d3931-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d3931-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d3931-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3931-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d3931-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d3931-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d3931-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d3931-115">Not supported.</span></span>|
|<span data-ttu-id="d3931-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d3931-116">Application</span></span>|<span data-ttu-id="d3931-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d3931-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d3931-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d3931-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="d3931-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d3931-119">Request headers</span></span>
|<span data-ttu-id="d3931-120">标头</span><span class="sxs-lookup"><span data-stu-id="d3931-120">Header</span></span>|<span data-ttu-id="d3931-121">值</span><span class="sxs-lookup"><span data-stu-id="d3931-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d3931-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d3931-122">Authorization</span></span>|<span data-ttu-id="d3931-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d3931-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d3931-124">接受</span><span class="sxs-lookup"><span data-stu-id="d3931-124">Accept</span></span>|<span data-ttu-id="d3931-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d3931-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d3931-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d3931-126">Request body</span></span>
<span data-ttu-id="d3931-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d3931-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d3931-128">响应</span><span class="sxs-lookup"><span data-stu-id="d3931-128">Response</span></span>
<span data-ttu-id="d3931-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="d3931-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="d3931-130">示例</span><span class="sxs-lookup"><span data-stu-id="d3931-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d3931-131">请求</span><span class="sxs-lookup"><span data-stu-id="d3931-131">Request</span></span>
<span data-ttu-id="d3931-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d3931-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="d3931-133">响应</span><span class="sxs-lookup"><span data-stu-id="d3931-133">Response</span></span>
<span data-ttu-id="d3931-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d3931-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




