---
title: 删除 deviceManagementDerivedCredentialSettings
description: 删除 deviceManagementDerivedCredentialSettings。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 063957b79c72bf0fea685e0f4f00997179a79a62
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51867502"
---
# <a name="delete-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="7823a-103">删除 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="7823a-103">Delete deviceManagementDerivedCredentialSettings</span></span>

<span data-ttu-id="7823a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7823a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7823a-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7823a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7823a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7823a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7823a-107">删除 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="7823a-107">Deletes a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7823a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7823a-108">Prerequisites</span></span>
<span data-ttu-id="7823a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7823a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7823a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7823a-111">Permission type</span></span>|<span data-ttu-id="7823a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7823a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7823a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7823a-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="7823a-114">&nbsp;&nbsp;**资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="7823a-114">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="7823a-115">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7823a-115">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="7823a-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7823a-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7823a-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7823a-117">Not supported.</span></span>|
|<span data-ttu-id="7823a-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="7823a-118">Application</span></span>||
|<span data-ttu-id="7823a-119">&nbsp;&nbsp;**资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="7823a-119">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="7823a-120">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7823a-120">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7823a-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7823a-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

## <a name="request-headers"></a><span data-ttu-id="7823a-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7823a-122">Request headers</span></span>
|<span data-ttu-id="7823a-123">标头</span><span class="sxs-lookup"><span data-stu-id="7823a-123">Header</span></span>|<span data-ttu-id="7823a-124">值</span><span class="sxs-lookup"><span data-stu-id="7823a-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7823a-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7823a-125">Authorization</span></span>|<span data-ttu-id="7823a-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7823a-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7823a-127">接受</span><span class="sxs-lookup"><span data-stu-id="7823a-127">Accept</span></span>|<span data-ttu-id="7823a-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7823a-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7823a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7823a-129">Request body</span></span>
<span data-ttu-id="7823a-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7823a-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7823a-131">响应</span><span class="sxs-lookup"><span data-stu-id="7823a-131">Response</span></span>
<span data-ttu-id="7823a-132">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7823a-132">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7823a-133">示例</span><span class="sxs-lookup"><span data-stu-id="7823a-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="7823a-134">请求</span><span class="sxs-lookup"><span data-stu-id="7823a-134">Request</span></span>
<span data-ttu-id="7823a-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7823a-135">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

### <a name="response"></a><span data-ttu-id="7823a-136">响应</span><span class="sxs-lookup"><span data-stu-id="7823a-136">Response</span></span>
<span data-ttu-id="7823a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7823a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```








