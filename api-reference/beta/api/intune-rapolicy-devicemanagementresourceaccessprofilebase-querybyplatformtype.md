---
title: queryByPlatformType 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: cfef02eac2586fc98f8a86f9e7740b654695e14f
ms.sourcegitcommit: 3b583d7baa9ae81b796fd30bc24c65d26b2cdf43
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/04/2021
ms.locfileid: "50446610"
---
# <a name="querybyplatformtype-action"></a><span data-ttu-id="84b56-103">queryByPlatformType 操作</span><span class="sxs-lookup"><span data-stu-id="84b56-103">queryByPlatformType action</span></span>

<span data-ttu-id="84b56-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84b56-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84b56-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84b56-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84b56-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84b56-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84b56-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="84b56-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84b56-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="84b56-108">Prerequisites</span></span>
<span data-ttu-id="84b56-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84b56-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84b56-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="84b56-111">Permission type</span></span>|<span data-ttu-id="84b56-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="84b56-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84b56-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84b56-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84b56-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84b56-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="84b56-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84b56-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84b56-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="84b56-116">Not supported.</span></span>|
|<span data-ttu-id="84b56-117">Application</span><span class="sxs-lookup"><span data-stu-id="84b56-117">Application</span></span>|<span data-ttu-id="84b56-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="84b56-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84b56-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84b56-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/resourceAccessProfiles/queryByPlatformType
```

## <a name="request-headers"></a><span data-ttu-id="84b56-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="84b56-120">Request headers</span></span>
|<span data-ttu-id="84b56-121">标头</span><span class="sxs-lookup"><span data-stu-id="84b56-121">Header</span></span>|<span data-ttu-id="84b56-122">值</span><span class="sxs-lookup"><span data-stu-id="84b56-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84b56-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="84b56-123">Authorization</span></span>|<span data-ttu-id="84b56-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="84b56-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84b56-125">接受</span><span class="sxs-lookup"><span data-stu-id="84b56-125">Accept</span></span>|<span data-ttu-id="84b56-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84b56-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84b56-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="84b56-127">Request body</span></span>
<span data-ttu-id="84b56-128">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="84b56-128">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="84b56-129">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="84b56-129">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="84b56-130">属性</span><span class="sxs-lookup"><span data-stu-id="84b56-130">Property</span></span>|<span data-ttu-id="84b56-131">类型</span><span class="sxs-lookup"><span data-stu-id="84b56-131">Type</span></span>|<span data-ttu-id="84b56-132">说明</span><span class="sxs-lookup"><span data-stu-id="84b56-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="84b56-133">platformType</span><span class="sxs-lookup"><span data-stu-id="84b56-133">platformType</span></span>|[<span data-ttu-id="84b56-134">policyPlatformType</span><span class="sxs-lookup"><span data-stu-id="84b56-134">policyPlatformType</span></span>](../resources/intune-shared-policyplatformtype.md)|<span data-ttu-id="84b56-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="84b56-135">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="84b56-136">响应</span><span class="sxs-lookup"><span data-stu-id="84b56-136">Response</span></span>
<span data-ttu-id="84b56-137">如果成功，此操作在响应 `200 OK` 正文中返回iQueryable_1OfDeviceManagementResourceAccessProfileBase代码[](../resources/intune-rapolicy-iqueryable_1ofdevicemanagementresourceaccessprofilebase.md)和响应代码。</span><span class="sxs-lookup"><span data-stu-id="84b56-137">If successful, this action returns a `200 OK` response code and a [iQueryable_1OfDeviceManagementResourceAccessProfileBase](../resources/intune-rapolicy-iqueryable_1ofdevicemanagementresourceaccessprofilebase.md) in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84b56-138">示例</span><span class="sxs-lookup"><span data-stu-id="84b56-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="84b56-139">请求</span><span class="sxs-lookup"><span data-stu-id="84b56-139">Request</span></span>
<span data-ttu-id="84b56-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="84b56-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles/queryByPlatformType

Content-type: application/json
Content-length: 40

{
  "platformType": "androidForWork"
}
```

### <a name="response"></a><span data-ttu-id="84b56-141">响应</span><span class="sxs-lookup"><span data-stu-id="84b56-141">Response</span></span>
<span data-ttu-id="84b56-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="84b56-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 117

{
  "value": {
    "@odata.type": "microsoft.graph.iQueryable_1OfDeviceManagementResourceAccessProfileBase"
  }
}
```




