---
title: 删除 deviceManagementDerivedCredentialSettings
description: 删除 deviceManagementDerivedCredentialSettings。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 62574dec6669d2d366cd396bcc0dd0cfd45e1154
ms.sourcegitcommit: 0dcabe677927c259c2ddcefd0d5e2a2aef065e8b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/16/2019
ms.locfileid: "37538180"
---
# <a name="delete-devicemanagementderivedcredentialsettings"></a><span data-ttu-id="e74e7-103">删除 deviceManagementDerivedCredentialSettings</span><span class="sxs-lookup"><span data-stu-id="e74e7-103">Delete deviceManagementDerivedCredentialSettings</span></span>

> <span data-ttu-id="e74e7-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e74e7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e74e7-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e74e7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e74e7-106">删除[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)。</span><span class="sxs-lookup"><span data-stu-id="e74e7-106">Deletes a [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e74e7-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e74e7-107">Prerequisites</span></span>
<span data-ttu-id="e74e7-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e74e7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e74e7-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e74e7-110">Permission type</span></span>|<span data-ttu-id="e74e7-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e74e7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e74e7-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e74e7-112">Delegated (work or school account)</span></span>||
|<span data-ttu-id="e74e7-113">&nbsp;&nbsp; **资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="e74e7-113">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="e74e7-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e74e7-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e74e7-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e74e7-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e74e7-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e74e7-116">Not supported.</span></span>|
|<span data-ttu-id="e74e7-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e74e7-117">Application</span></span>||
|<span data-ttu-id="e74e7-118">&nbsp;&nbsp; **资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="e74e7-118">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="e74e7-119">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e74e7-119">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e74e7-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e74e7-120">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

## <a name="request-headers"></a><span data-ttu-id="e74e7-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="e74e7-121">Request headers</span></span>
|<span data-ttu-id="e74e7-122">标头</span><span class="sxs-lookup"><span data-stu-id="e74e7-122">Header</span></span>|<span data-ttu-id="e74e7-123">值</span><span class="sxs-lookup"><span data-stu-id="e74e7-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e74e7-124">授权</span><span class="sxs-lookup"><span data-stu-id="e74e7-124">Authorization</span></span>|<span data-ttu-id="e74e7-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e74e7-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e74e7-126">接受</span><span class="sxs-lookup"><span data-stu-id="e74e7-126">Accept</span></span>|<span data-ttu-id="e74e7-127">application/json</span><span class="sxs-lookup"><span data-stu-id="e74e7-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e74e7-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="e74e7-128">Request body</span></span>
<span data-ttu-id="e74e7-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e74e7-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e74e7-130">响应</span><span class="sxs-lookup"><span data-stu-id="e74e7-130">Response</span></span>
<span data-ttu-id="e74e7-131">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e74e7-131">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e74e7-132">示例</span><span class="sxs-lookup"><span data-stu-id="e74e7-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="e74e7-133">请求</span><span class="sxs-lookup"><span data-stu-id="e74e7-133">Request</span></span>
<span data-ttu-id="e74e7-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e74e7-134">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/derivedCredentials/{deviceManagementDerivedCredentialSettingsId}
```

### <a name="response"></a><span data-ttu-id="e74e7-135">响应</span><span class="sxs-lookup"><span data-stu-id="e74e7-135">Response</span></span>
<span data-ttu-id="e74e7-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e74e7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







