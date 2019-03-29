---
title: 删除 windowsInformationProtectionPolicy
description: 删除 windowsInformationProtectionPolicy。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 5ca74dfde0c5b03c2d520df4ea30c42359828679
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30958205"
---
# <a name="delete-windowsinformationprotectionpolicy"></a><span data-ttu-id="18615-103">删除 windowsInformationProtectionPolicy</span><span class="sxs-lookup"><span data-stu-id="18615-103">Delete windowsInformationProtectionPolicy</span></span>

> <span data-ttu-id="18615-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="18615-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="18615-105">删除 [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="18615-105">Deletes a [windowsInformationProtectionPolicy](../resources/intune-mam-windowsinformationprotectionpolicy.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="18615-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="18615-106">Prerequisites</span></span>
<span data-ttu-id="18615-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="18615-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="18615-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="18615-109">Permission type</span></span>|<span data-ttu-id="18615-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="18615-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="18615-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="18615-111">Delegated (work or school account)</span></span>|<span data-ttu-id="18615-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="18615-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="18615-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="18615-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="18615-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="18615-114">Not supported.</span></span>|
|<span data-ttu-id="18615-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="18615-115">Application</span></span>|<span data-ttu-id="18615-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="18615-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="18615-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="18615-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

## <a name="request-headers"></a><span data-ttu-id="18615-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="18615-118">Request headers</span></span>
|<span data-ttu-id="18615-119">标头</span><span class="sxs-lookup"><span data-stu-id="18615-119">Header</span></span>|<span data-ttu-id="18615-120">值</span><span class="sxs-lookup"><span data-stu-id="18615-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="18615-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="18615-121">Authorization</span></span>|<span data-ttu-id="18615-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="18615-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="18615-123">接受</span><span class="sxs-lookup"><span data-stu-id="18615-123">Accept</span></span>|<span data-ttu-id="18615-124">application/json</span><span class="sxs-lookup"><span data-stu-id="18615-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="18615-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="18615-125">Request body</span></span>
<span data-ttu-id="18615-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="18615-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="18615-127">响应</span><span class="sxs-lookup"><span data-stu-id="18615-127">Response</span></span>
<span data-ttu-id="18615-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="18615-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="18615-129">示例</span><span class="sxs-lookup"><span data-stu-id="18615-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="18615-130">请求</span><span class="sxs-lookup"><span data-stu-id="18615-130">Request</span></span>
<span data-ttu-id="18615-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="18615-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}
```

### <a name="response"></a><span data-ttu-id="18615-132">响应</span><span class="sxs-lookup"><span data-stu-id="18615-132">Response</span></span>
<span data-ttu-id="18615-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="18615-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



