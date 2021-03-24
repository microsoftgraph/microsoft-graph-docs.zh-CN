---
title: 删除 androidForWorkPkcsCertificateProfile
description: 删除 androidForWorkPkcsCertificateProfile。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: df74cdee12a0a94153b12c48a3316bf799f245b8
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51142581"
---
# <a name="delete-androidforworkpkcscertificateprofile"></a><span data-ttu-id="2cebd-103">删除 androidForWorkPkcsCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="2cebd-103">Delete androidForWorkPkcsCertificateProfile</span></span>

<span data-ttu-id="2cebd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2cebd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="2cebd-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2cebd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cebd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2cebd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cebd-107">删除 [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="2cebd-107">Deletes a [androidForWorkPkcsCertificateProfile](../resources/intune-deviceconfig-androidforworkpkcscertificateprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2cebd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="2cebd-108">Prerequisites</span></span>
<span data-ttu-id="2cebd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2cebd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cebd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2cebd-111">Permission type</span></span>|<span data-ttu-id="2cebd-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2cebd-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cebd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2cebd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="2cebd-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cebd-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="2cebd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2cebd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cebd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2cebd-116">Not supported.</span></span>|
|<span data-ttu-id="2cebd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2cebd-117">Application</span></span>|<span data-ttu-id="2cebd-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cebd-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cebd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2cebd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2cebd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2cebd-120">Request headers</span></span>
|<span data-ttu-id="2cebd-121">标头</span><span class="sxs-lookup"><span data-stu-id="2cebd-121">Header</span></span>|<span data-ttu-id="2cebd-122">值</span><span class="sxs-lookup"><span data-stu-id="2cebd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cebd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cebd-123">Authorization</span></span>|<span data-ttu-id="2cebd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2cebd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cebd-125">接受</span><span class="sxs-lookup"><span data-stu-id="2cebd-125">Accept</span></span>|<span data-ttu-id="2cebd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="2cebd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cebd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2cebd-127">Request body</span></span>
<span data-ttu-id="2cebd-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2cebd-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2cebd-129">响应</span><span class="sxs-lookup"><span data-stu-id="2cebd-129">Response</span></span>
<span data-ttu-id="2cebd-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2cebd-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2cebd-131">示例</span><span class="sxs-lookup"><span data-stu-id="2cebd-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="2cebd-132">请求</span><span class="sxs-lookup"><span data-stu-id="2cebd-132">Request</span></span>
<span data-ttu-id="2cebd-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2cebd-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="2cebd-134">响应</span><span class="sxs-lookup"><span data-stu-id="2cebd-134">Response</span></span>
<span data-ttu-id="2cebd-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2cebd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




