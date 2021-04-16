---
title: targetApps 操作
description: 尚未记录
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 5dba5d7e6127ae59b01c35e9a80cce13e51a66cd
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51865388"
---
# <a name="targetapps-action"></a><span data-ttu-id="7d00f-103">targetApps 操作</span><span class="sxs-lookup"><span data-stu-id="7d00f-103">targetApps action</span></span>

<span data-ttu-id="7d00f-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7d00f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="7d00f-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="7d00f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="7d00f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7d00f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7d00f-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7d00f-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7d00f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="7d00f-108">Prerequisites</span></span>
<span data-ttu-id="7d00f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7d00f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7d00f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7d00f-111">Permission type</span></span>|<span data-ttu-id="7d00f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7d00f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7d00f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7d00f-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="7d00f-114">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="7d00f-114">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="7d00f-115">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d00f-115">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7d00f-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7d00f-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7d00f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="7d00f-117">Not supported.</span></span>|
|<span data-ttu-id="7d00f-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="7d00f-118">Application</span></span>||
| <span data-ttu-id="7d00f-119">&nbsp; &nbsp; **移动应用管理 (MAM)**</span><span class="sxs-lookup"><span data-stu-id="7d00f-119">&nbsp; &nbsp; **Mobile app management (MAM)**</span></span> | <span data-ttu-id="7d00f-120">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7d00f-120">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="7d00f-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7d00f-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps
```

## <a name="request-headers"></a><span data-ttu-id="7d00f-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="7d00f-122">Request headers</span></span>
|<span data-ttu-id="7d00f-123">标头</span><span class="sxs-lookup"><span data-stu-id="7d00f-123">Header</span></span>|<span data-ttu-id="7d00f-124">值</span><span class="sxs-lookup"><span data-stu-id="7d00f-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7d00f-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="7d00f-125">Authorization</span></span>|<span data-ttu-id="7d00f-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7d00f-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7d00f-127">接受</span><span class="sxs-lookup"><span data-stu-id="7d00f-127">Accept</span></span>|<span data-ttu-id="7d00f-128">application/json</span><span class="sxs-lookup"><span data-stu-id="7d00f-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7d00f-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7d00f-129">Request body</span></span>
<span data-ttu-id="7d00f-130">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7d00f-130">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="7d00f-131">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="7d00f-131">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="7d00f-132">属性</span><span class="sxs-lookup"><span data-stu-id="7d00f-132">Property</span></span>|<span data-ttu-id="7d00f-133">类型</span><span class="sxs-lookup"><span data-stu-id="7d00f-133">Type</span></span>|<span data-ttu-id="7d00f-134">说明</span><span class="sxs-lookup"><span data-stu-id="7d00f-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7d00f-135">apps</span><span class="sxs-lookup"><span data-stu-id="7d00f-135">apps</span></span>|<span data-ttu-id="7d00f-136">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) 集合</span><span class="sxs-lookup"><span data-stu-id="7d00f-136">[managedMobileApp](../resources/intune-mam-managedmobileapp.md) collection</span></span>|<span data-ttu-id="7d00f-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="7d00f-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="7d00f-138">响应</span><span class="sxs-lookup"><span data-stu-id="7d00f-138">Response</span></span>
<span data-ttu-id="7d00f-139">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7d00f-139">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7d00f-140">示例</span><span class="sxs-lookup"><span data-stu-id="7d00f-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="7d00f-141">请求</span><span class="sxs-lookup"><span data-stu-id="7d00f-141">Request</span></span>
<span data-ttu-id="7d00f-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7d00f-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/targetApps

Content-type: application/json
Content-length: 286

{
  "apps": [
    {
      "@odata.type": "#microsoft.graph.managedMobileApp",
      "mobileAppIdentifier": {
        "@odata.type": "microsoft.graph.mobileAppIdentifier"
      },
      "id": "0a129715-9715-0a12-1597-120a1597120a",
      "version": "Version value"
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="7d00f-143">响应</span><span class="sxs-lookup"><span data-stu-id="7d00f-143">Response</span></span>
<span data-ttu-id="7d00f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7d00f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```







