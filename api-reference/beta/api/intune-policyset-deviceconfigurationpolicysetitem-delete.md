---
title: 删除 deviceConfigurationPolicySetItem
description: 删除 deviceConfigurationPolicySetItem。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bca0364242137faf679ae0bb939cae6cc28287a2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48093712"
---
# <a name="delete-deviceconfigurationpolicysetitem"></a><span data-ttu-id="b5903-103">删除 deviceConfigurationPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="b5903-103">Delete deviceConfigurationPolicySetItem</span></span>

<span data-ttu-id="b5903-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5903-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5903-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b5903-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5903-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5903-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5903-107">删除 [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="b5903-107">Deletes a [deviceConfigurationPolicySetItem](../resources/intune-policyset-deviceconfigurationpolicysetitem.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5903-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b5903-108">Prerequisites</span></span>
<span data-ttu-id="b5903-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5903-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5903-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5903-111">Permission type</span></span>|<span data-ttu-id="b5903-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b5903-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5903-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5903-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5903-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5903-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b5903-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5903-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5903-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5903-116">Not supported.</span></span>|
|<span data-ttu-id="b5903-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5903-117">Application</span></span>|<span data-ttu-id="b5903-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5903-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5903-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5903-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="b5903-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5903-120">Request headers</span></span>
|<span data-ttu-id="b5903-121">标头</span><span class="sxs-lookup"><span data-stu-id="b5903-121">Header</span></span>|<span data-ttu-id="b5903-122">值</span><span class="sxs-lookup"><span data-stu-id="b5903-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5903-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5903-123">Authorization</span></span>|<span data-ttu-id="b5903-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b5903-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5903-125">接受</span><span class="sxs-lookup"><span data-stu-id="b5903-125">Accept</span></span>|<span data-ttu-id="b5903-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5903-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5903-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5903-127">Request body</span></span>
<span data-ttu-id="b5903-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b5903-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5903-129">响应</span><span class="sxs-lookup"><span data-stu-id="b5903-129">Response</span></span>
<span data-ttu-id="b5903-130">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="b5903-130">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="b5903-131">示例</span><span class="sxs-lookup"><span data-stu-id="b5903-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5903-132">请求</span><span class="sxs-lookup"><span data-stu-id="b5903-132">Request</span></span>
<span data-ttu-id="b5903-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5903-133">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="b5903-134">响应</span><span class="sxs-lookup"><span data-stu-id="b5903-134">Response</span></span>
<span data-ttu-id="b5903-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b5903-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```






