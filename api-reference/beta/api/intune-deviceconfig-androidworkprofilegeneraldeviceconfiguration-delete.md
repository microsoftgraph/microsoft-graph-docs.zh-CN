---
title: 删除 androidWorkProfileGeneralDeviceConfiguration
description: 删除 androidWorkProfileGeneralDeviceConfiguration。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c78412d2a675385e895653269c20369ca71d6bf0
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48697005"
---
# <a name="delete-androidworkprofilegeneraldeviceconfiguration"></a><span data-ttu-id="84938-103">删除 androidWorkProfileGeneralDeviceConfiguration</span><span class="sxs-lookup"><span data-stu-id="84938-103">Delete androidWorkProfileGeneralDeviceConfiguration</span></span>

<span data-ttu-id="84938-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84938-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84938-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84938-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84938-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84938-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84938-107">删除 [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="84938-107">Deletes a [androidWorkProfileGeneralDeviceConfiguration](../resources/intune-deviceconfig-androidworkprofilegeneraldeviceconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84938-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="84938-108">Prerequisites</span></span>
<span data-ttu-id="84938-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84938-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84938-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="84938-111">Permission type</span></span>|<span data-ttu-id="84938-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="84938-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84938-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84938-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84938-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84938-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="84938-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84938-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84938-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="84938-116">Not supported.</span></span>|
|<span data-ttu-id="84938-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="84938-117">Application</span></span>|<span data-ttu-id="84938-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84938-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84938-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84938-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="84938-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="84938-120">Request headers</span></span>
|<span data-ttu-id="84938-121">标头</span><span class="sxs-lookup"><span data-stu-id="84938-121">Header</span></span>|<span data-ttu-id="84938-122">值</span><span class="sxs-lookup"><span data-stu-id="84938-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84938-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="84938-123">Authorization</span></span>|<span data-ttu-id="84938-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="84938-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84938-125">接受</span><span class="sxs-lookup"><span data-stu-id="84938-125">Accept</span></span>|<span data-ttu-id="84938-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84938-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84938-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="84938-127">Request body</span></span>
<span data-ttu-id="84938-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="84938-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84938-129">响应</span><span class="sxs-lookup"><span data-stu-id="84938-129">Response</span></span>
<span data-ttu-id="84938-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="84938-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="84938-131">示例</span><span class="sxs-lookup"><span data-stu-id="84938-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="84938-132">请求</span><span class="sxs-lookup"><span data-stu-id="84938-132">Request</span></span>
<span data-ttu-id="84938-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="84938-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="84938-134">响应</span><span class="sxs-lookup"><span data-stu-id="84938-134">Response</span></span>
<span data-ttu-id="84938-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="84938-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





