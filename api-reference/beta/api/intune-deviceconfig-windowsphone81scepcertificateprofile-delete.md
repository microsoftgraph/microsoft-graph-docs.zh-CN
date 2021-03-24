---
title: 删除 windowsPhone81SCEPCertificateProfile
description: 删除 windowsPhone81SCEPCertificateProfile。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 88a89c4d61cf902e4e01ff7109af3989e0b128d2
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51129354"
---
# <a name="delete-windowsphone81scepcertificateprofile"></a><span data-ttu-id="83903-103">删除 windowsPhone81SCEPCertificateProfile</span><span class="sxs-lookup"><span data-stu-id="83903-103">Delete windowsPhone81SCEPCertificateProfile</span></span>

<span data-ttu-id="83903-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="83903-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="83903-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="83903-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="83903-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="83903-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="83903-107">删除 [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="83903-107">Deletes a [windowsPhone81SCEPCertificateProfile](../resources/intune-deviceconfig-windowsphone81scepcertificateprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="83903-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="83903-108">Prerequisites</span></span>
<span data-ttu-id="83903-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="83903-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83903-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="83903-111">Permission type</span></span>|<span data-ttu-id="83903-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="83903-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83903-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83903-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83903-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83903-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="83903-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83903-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83903-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="83903-116">Not supported.</span></span>|
|<span data-ttu-id="83903-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="83903-117">Application</span></span>|<span data-ttu-id="83903-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83903-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="83903-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83903-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/groupAssignments/{deviceConfigurationGroupAssignmentId}/deviceConfiguration
DELETE /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations/{deviceConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="83903-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="83903-120">Request headers</span></span>
|<span data-ttu-id="83903-121">标头</span><span class="sxs-lookup"><span data-stu-id="83903-121">Header</span></span>|<span data-ttu-id="83903-122">值</span><span class="sxs-lookup"><span data-stu-id="83903-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83903-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83903-123">Authorization</span></span>|<span data-ttu-id="83903-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="83903-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83903-125">接受</span><span class="sxs-lookup"><span data-stu-id="83903-125">Accept</span></span>|<span data-ttu-id="83903-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83903-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83903-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="83903-127">Request body</span></span>
<span data-ttu-id="83903-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="83903-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="83903-129">响应</span><span class="sxs-lookup"><span data-stu-id="83903-129">Response</span></span>
<span data-ttu-id="83903-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="83903-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="83903-131">示例</span><span class="sxs-lookup"><span data-stu-id="83903-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="83903-132">请求</span><span class="sxs-lookup"><span data-stu-id="83903-132">Request</span></span>
<span data-ttu-id="83903-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="83903-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations/{deviceConfigurationId}
```

### <a name="response"></a><span data-ttu-id="83903-134">响应</span><span class="sxs-lookup"><span data-stu-id="83903-134">Response</span></span>
<span data-ttu-id="83903-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="83903-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




