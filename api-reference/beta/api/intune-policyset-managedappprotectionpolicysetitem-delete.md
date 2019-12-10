---
title: 删除 managedAppProtectionPolicySetItem
description: 删除 managedAppProtectionPolicySetItem。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 64f5a25e5f2bfc84aced5efecaa52af032b8d345
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39941111"
---
# <a name="delete-managedappprotectionpolicysetitem"></a><span data-ttu-id="e39e8-103">删除 managedAppProtectionPolicySetItem</span><span class="sxs-lookup"><span data-stu-id="e39e8-103">Delete managedAppProtectionPolicySetItem</span></span>

> <span data-ttu-id="e39e8-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e39e8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e39e8-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e39e8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e39e8-106">删除[managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md)。</span><span class="sxs-lookup"><span data-stu-id="e39e8-106">Deletes a [managedAppProtectionPolicySetItem](../resources/intune-policyset-managedappprotectionpolicysetitem.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e39e8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="e39e8-107">Prerequisites</span></span>
<span data-ttu-id="e39e8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e39e8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e39e8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="e39e8-110">Permission type</span></span>|<span data-ttu-id="e39e8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e39e8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e39e8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e39e8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e39e8-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e39e8-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e39e8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e39e8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e39e8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="e39e8-115">Not supported.</span></span>|
|<span data-ttu-id="e39e8-116">Application</span><span class="sxs-lookup"><span data-stu-id="e39e8-116">Application</span></span>|<span data-ttu-id="e39e8-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e39e8-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e39e8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e39e8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

## <a name="request-headers"></a><span data-ttu-id="e39e8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="e39e8-119">Request headers</span></span>
|<span data-ttu-id="e39e8-120">标头</span><span class="sxs-lookup"><span data-stu-id="e39e8-120">Header</span></span>|<span data-ttu-id="e39e8-121">值</span><span class="sxs-lookup"><span data-stu-id="e39e8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e39e8-122">授权</span><span class="sxs-lookup"><span data-stu-id="e39e8-122">Authorization</span></span>|<span data-ttu-id="e39e8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e39e8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e39e8-124">接受</span><span class="sxs-lookup"><span data-stu-id="e39e8-124">Accept</span></span>|<span data-ttu-id="e39e8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e39e8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e39e8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e39e8-126">Request body</span></span>
<span data-ttu-id="e39e8-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e39e8-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e39e8-128">响应</span><span class="sxs-lookup"><span data-stu-id="e39e8-128">Response</span></span>
<span data-ttu-id="e39e8-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="e39e8-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="e39e8-130">示例</span><span class="sxs-lookup"><span data-stu-id="e39e8-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="e39e8-131">请求</span><span class="sxs-lookup"><span data-stu-id="e39e8-131">Request</span></span>
<span data-ttu-id="e39e8-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e39e8-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceAppManagement/policySets/{policySetId}/items/{policySetItemId}
```

### <a name="response"></a><span data-ttu-id="e39e8-133">响应</span><span class="sxs-lookup"><span data-stu-id="e39e8-133">Response</span></span>
<span data-ttu-id="e39e8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e39e8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```





