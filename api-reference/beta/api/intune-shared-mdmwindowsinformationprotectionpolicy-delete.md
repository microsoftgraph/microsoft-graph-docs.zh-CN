---
title: 删除 mdmWindowsInformationProtectionPolicy
description: 删除 mdmWindowsInformationProtectionPolicy。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 7268b7754629fb87a6f32acac84c005dfb513c98
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863042"
---
# <a name="delete-mdmwindowsinformationprotectionpolicy"></a><span data-ttu-id="11320-103">删除 mdmWindowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="11320-103">Delete mdmWindowsInformationProtectionPolicy</span></span>

<span data-ttu-id="11320-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="11320-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="11320-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="11320-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="11320-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="11320-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="11320-107">删除 [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="11320-107">Deletes a [mdmWindowsInformationProtectionPolicy](../resources/intune-shared-mdmwindowsinformationprotectionpolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="11320-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="11320-108">Prerequisites</span></span>
<span data-ttu-id="11320-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="11320-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="11320-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="11320-111">Permission type</span></span>|<span data-ttu-id="11320-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="11320-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="11320-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="11320-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="11320-114">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="11320-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="11320-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11320-115">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="11320-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="11320-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="11320-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11320-117">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="11320-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="11320-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="11320-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="11320-119">Not supported.</span></span>|
|<span data-ttu-id="11320-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="11320-120">Application</span></span>||
| <span data-ttu-id="11320-121">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="11320-121">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="11320-122">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11320-122">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="11320-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="11320-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="11320-124">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="11320-124">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="11320-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="11320-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="11320-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="11320-126">Request headers</span></span>
|<span data-ttu-id="11320-127">标头</span><span class="sxs-lookup"><span data-stu-id="11320-127">Header</span></span>|<span data-ttu-id="11320-128">值</span><span class="sxs-lookup"><span data-stu-id="11320-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="11320-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="11320-129">Authorization</span></span>|<span data-ttu-id="11320-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="11320-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="11320-131">接受</span><span class="sxs-lookup"><span data-stu-id="11320-131">Accept</span></span>|<span data-ttu-id="11320-132">application/json</span><span class="sxs-lookup"><span data-stu-id="11320-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="11320-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="11320-133">Request body</span></span>
<span data-ttu-id="11320-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="11320-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="11320-135">响应</span><span class="sxs-lookup"><span data-stu-id="11320-135">Response</span></span>
<span data-ttu-id="11320-136">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="11320-136">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="11320-137">示例</span><span class="sxs-lookup"><span data-stu-id="11320-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="11320-138">请求</span><span class="sxs-lookup"><span data-stu-id="11320-138">Request</span></span>
<span data-ttu-id="11320-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="11320-139">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="11320-140">响应</span><span class="sxs-lookup"><span data-stu-id="11320-140">Response</span></span>
<span data-ttu-id="11320-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="11320-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







