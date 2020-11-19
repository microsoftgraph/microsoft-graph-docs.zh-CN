---
title: 删除 iosLobAppProvisioningConfiguration
description: 删除 iosLobAppProvisioningConfiguration。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d78b79483a871085da03293805bad196594ee4eb
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49232429"
---
# <a name="delete-ioslobappprovisioningconfiguration"></a><span data-ttu-id="6e80b-103">删除 iosLobAppProvisioningConfiguration</span><span class="sxs-lookup"><span data-stu-id="6e80b-103">Delete iosLobAppProvisioningConfiguration</span></span>

<span data-ttu-id="6e80b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6e80b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6e80b-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6e80b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6e80b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6e80b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6e80b-107">删除 [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="6e80b-107">Deletes a [iosLobAppProvisioningConfiguration](../resources/intune-shared-ioslobappprovisioningconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6e80b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6e80b-108">Prerequisites</span></span>
<span data-ttu-id="6e80b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6e80b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6e80b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6e80b-111">Permission type</span></span>|<span data-ttu-id="6e80b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6e80b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6e80b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6e80b-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6e80b-114">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="6e80b-114">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="6e80b-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e80b-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="6e80b-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="6e80b-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="6e80b-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e80b-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="6e80b-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6e80b-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6e80b-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="6e80b-119">Not supported.</span></span>|
|<span data-ttu-id="6e80b-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="6e80b-120">Application</span></span>||
| <span data-ttu-id="6e80b-121">&nbsp; &nbsp; **应用**</span><span class="sxs-lookup"><span data-stu-id="6e80b-121">&nbsp; &nbsp; **Apps**</span></span> | <span data-ttu-id="6e80b-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e80b-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="6e80b-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="6e80b-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="6e80b-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6e80b-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6e80b-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6e80b-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="6e80b-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="6e80b-126">Request headers</span></span>
|<span data-ttu-id="6e80b-127">标头</span><span class="sxs-lookup"><span data-stu-id="6e80b-127">Header</span></span>|<span data-ttu-id="6e80b-128">值</span><span class="sxs-lookup"><span data-stu-id="6e80b-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6e80b-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="6e80b-129">Authorization</span></span>|<span data-ttu-id="6e80b-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6e80b-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6e80b-131">接受</span><span class="sxs-lookup"><span data-stu-id="6e80b-131">Accept</span></span>|<span data-ttu-id="6e80b-132">application/json</span><span class="sxs-lookup"><span data-stu-id="6e80b-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6e80b-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="6e80b-133">Request body</span></span>
<span data-ttu-id="6e80b-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6e80b-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6e80b-135">响应</span><span class="sxs-lookup"><span data-stu-id="6e80b-135">Response</span></span>
<span data-ttu-id="6e80b-136">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="6e80b-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="6e80b-137">示例</span><span class="sxs-lookup"><span data-stu-id="6e80b-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="6e80b-138">请求</span><span class="sxs-lookup"><span data-stu-id="6e80b-138">Request</span></span>
<span data-ttu-id="6e80b-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6e80b-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/iosLobAppProvisioningConfigurations/{iosLobAppProvisioningConfigurationId}
```

### <a name="response"></a><span data-ttu-id="6e80b-140">响应</span><span class="sxs-lookup"><span data-stu-id="6e80b-140">Response</span></span>
<span data-ttu-id="6e80b-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6e80b-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







