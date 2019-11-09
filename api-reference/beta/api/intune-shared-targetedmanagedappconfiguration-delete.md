---
title: 删除 targetedManagedAppConfiguration
description: 删除 targetedManagedAppConfiguration。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: e00df89fe420aa7dbeb6ce1f1ce4722d074eed5b
ms.sourcegitcommit: 5b1fad41067629d0e9f87746328664bb248f754f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/09/2019
ms.locfileid: "38085638"
---
# <a name="delete-targetedmanagedappconfiguration"></a><span data-ttu-id="2cf98-103">删除 targetedManagedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2cf98-103">Delete targetedManagedAppConfiguration</span></span>

> <span data-ttu-id="2cf98-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="2cf98-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="2cf98-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="2cf98-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2cf98-106">删除 [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md)。</span><span class="sxs-lookup"><span data-stu-id="2cf98-106">Deletes a [targetedManagedAppConfiguration](../resources/intune-shared-targetedmanagedappconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="2cf98-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="2cf98-107">Prerequisites</span></span>
<span data-ttu-id="2cf98-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2cf98-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2cf98-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="2cf98-110">Permission type</span></span>|<span data-ttu-id="2cf98-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2cf98-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2cf98-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2cf98-112">Delegated (work or school account)</span></span>||
| <span data-ttu-id="2cf98-113">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="2cf98-113">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="2cf98-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cf98-114">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="2cf98-115">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="2cf98-115">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="2cf98-116">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cf98-116">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="2cf98-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2cf98-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2cf98-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2cf98-118">Not supported.</span></span>|
|<span data-ttu-id="2cf98-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="2cf98-119">Application</span></span>||
| <span data-ttu-id="2cf98-120">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="2cf98-120">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="2cf98-121">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cf98-121">DeviceManagementApps.ReadWrite.All</span></span>|
| <span data-ttu-id="2cf98-122">&nbsp;&nbsp; **策略集**</span><span class="sxs-lookup"><span data-stu-id="2cf98-122">&nbsp; &nbsp; **Policy Set**</span></span>  | <span data-ttu-id="2cf98-123">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2cf98-123">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="2cf98-124">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2cf98-124">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

## <a name="request-headers"></a><span data-ttu-id="2cf98-125">请求标头</span><span class="sxs-lookup"><span data-stu-id="2cf98-125">Request headers</span></span>
|<span data-ttu-id="2cf98-126">标头</span><span class="sxs-lookup"><span data-stu-id="2cf98-126">Header</span></span>|<span data-ttu-id="2cf98-127">值</span><span class="sxs-lookup"><span data-stu-id="2cf98-127">Value</span></span>|
|:---|:---|
|<span data-ttu-id="2cf98-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="2cf98-128">Authorization</span></span>|<span data-ttu-id="2cf98-129">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="2cf98-129">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="2cf98-130">接受</span><span class="sxs-lookup"><span data-stu-id="2cf98-130">Accept</span></span>|<span data-ttu-id="2cf98-131">application/json</span><span class="sxs-lookup"><span data-stu-id="2cf98-131">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="2cf98-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="2cf98-132">Request body</span></span>
<span data-ttu-id="2cf98-133">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2cf98-133">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2cf98-134">响应</span><span class="sxs-lookup"><span data-stu-id="2cf98-134">Response</span></span>
<span data-ttu-id="2cf98-135">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="2cf98-135">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="2cf98-136">示例</span><span class="sxs-lookup"><span data-stu-id="2cf98-136">Example</span></span>

### <a name="request"></a><span data-ttu-id="2cf98-137">请求</span><span class="sxs-lookup"><span data-stu-id="2cf98-137">Request</span></span>
<span data-ttu-id="2cf98-138">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="2cf98-138">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}
```

### <a name="response"></a><span data-ttu-id="2cf98-139">响应</span><span class="sxs-lookup"><span data-stu-id="2cf98-139">Response</span></span>
<span data-ttu-id="2cf98-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="2cf98-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```









