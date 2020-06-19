---
title: enableUnlicensedAdminstrators 操作
description: 启用后，通过角色分配成员身份分配给管理员的用户将不再需要分配的 Intune 许可证。 对于角色分配中的每个 AAD 安全组，限制为350个无许可证的直接成员，但如果需要支持超过350个未获得授权的管理员，则可以将多个 AAD 安全组分配给一个角色。 许可管理员将继续按中的顺序工作，这是可传递的成员资格应用且不受350成员限制的限制。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 882a5d1cafa8e25d4a69a0c525c0bb8d3b971cd1
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792804"
---
# <a name="enableunlicensedadminstrators-action"></a><span data-ttu-id="08ec4-105">enableUnlicensedAdminstrators 操作</span><span class="sxs-lookup"><span data-stu-id="08ec4-105">enableUnlicensedAdminstrators action</span></span>

<span data-ttu-id="08ec4-106">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08ec4-106">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08ec4-107">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="08ec4-107">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08ec4-108">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08ec4-108">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08ec4-109">启用后，通过角色分配成员身份分配给管理员的用户将不再需要分配的 Intune 许可证。</span><span class="sxs-lookup"><span data-stu-id="08ec4-109">Upon enabling, users assigned as administrators via Role Assignment Memberships will no longer require an assigned Intune license.</span></span> <span data-ttu-id="08ec4-110">对于角色分配中的每个 AAD 安全组，限制为350个无许可证的直接成员，但如果需要支持超过350个未获得授权的管理员，则可以将多个 AAD 安全组分配给一个角色。</span><span class="sxs-lookup"><span data-stu-id="08ec4-110">You are limited to 350 unlicensed direct members for each AAD security group in a role assignment, but you can assign multiple AAD security groups to a role if you need to support more than 350 unlicensed administrators.</span></span> <span data-ttu-id="08ec4-111">许可管理员将继续按中的顺序工作，这是可传递的成员资格应用且不受350成员限制的限制。</span><span class="sxs-lookup"><span data-stu-id="08ec4-111">Licensed administrators will continue to function as-is in that transitive memberships apply and are not subject to the 350 member limit.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08ec4-112">先决条件</span><span class="sxs-lookup"><span data-stu-id="08ec4-112">Prerequisites</span></span>
<span data-ttu-id="08ec4-113">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="08ec4-113">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="08ec4-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="08ec4-114">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08ec4-115">权限类型</span><span class="sxs-lookup"><span data-stu-id="08ec4-115">Permission type</span></span>|<span data-ttu-id="08ec4-116">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="08ec4-116">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08ec4-117">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08ec4-117">Delegated (work or school account)</span></span>|<span data-ttu-id="08ec4-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08ec4-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="08ec4-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08ec4-119">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08ec4-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="08ec4-120">Not supported.</span></span>|
|<span data-ttu-id="08ec4-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="08ec4-121">Application</span></span>|<span data-ttu-id="08ec4-122">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08ec4-122">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08ec4-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08ec4-123">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/enableUnlicensedAdminstrators
```

## <a name="request-headers"></a><span data-ttu-id="08ec4-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="08ec4-124">Request headers</span></span>
|<span data-ttu-id="08ec4-125">标头</span><span class="sxs-lookup"><span data-stu-id="08ec4-125">Header</span></span>|<span data-ttu-id="08ec4-126">值</span><span class="sxs-lookup"><span data-stu-id="08ec4-126">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08ec4-127">Authorization</span><span class="sxs-lookup"><span data-stu-id="08ec4-127">Authorization</span></span>|<span data-ttu-id="08ec4-128">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="08ec4-128">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08ec4-129">接受</span><span class="sxs-lookup"><span data-stu-id="08ec4-129">Accept</span></span>|<span data-ttu-id="08ec4-130">application/json</span><span class="sxs-lookup"><span data-stu-id="08ec4-130">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08ec4-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="08ec4-131">Request body</span></span>
<span data-ttu-id="08ec4-132">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="08ec4-132">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="08ec4-133">响应</span><span class="sxs-lookup"><span data-stu-id="08ec4-133">Response</span></span>
<span data-ttu-id="08ec4-134">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="08ec4-134">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="08ec4-135">示例</span><span class="sxs-lookup"><span data-stu-id="08ec4-135">Example</span></span>

### <a name="request"></a><span data-ttu-id="08ec4-136">请求</span><span class="sxs-lookup"><span data-stu-id="08ec4-136">Request</span></span>
<span data-ttu-id="08ec4-137">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="08ec4-137">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/enableUnlicensedAdminstrators
```

### <a name="response"></a><span data-ttu-id="08ec4-138">响应</span><span class="sxs-lookup"><span data-stu-id="08ec4-138">Response</span></span>
<span data-ttu-id="08ec4-139">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="08ec4-139">Here is an example of the response.</span></span> <span data-ttu-id="08ec4-140">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="08ec4-140">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="08ec4-141">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="08ec4-141">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



