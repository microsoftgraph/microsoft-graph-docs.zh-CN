---
title: 删除 enrollmentProfile
description: 删除 enrollmentProfile。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ad20a6a282fa44f6d721f2175ca09f9d8f1273d3
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30959731"
---
# <a name="delete-enrollmentprofile"></a><span data-ttu-id="f3885-103">删除 enrollmentProfile</span><span class="sxs-lookup"><span data-stu-id="f3885-103">Delete enrollmentProfile</span></span>

> <span data-ttu-id="f3885-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f3885-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f3885-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f3885-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f3885-106">删除[enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md)。</span><span class="sxs-lookup"><span data-stu-id="f3885-106">Deletes a [enrollmentProfile](../resources/intune-enrollment-enrollmentprofile.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f3885-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="f3885-107">Prerequisites</span></span>
<span data-ttu-id="f3885-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f3885-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f3885-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="f3885-110">Permission type</span></span>|<span data-ttu-id="f3885-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f3885-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f3885-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f3885-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f3885-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f3885-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="f3885-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f3885-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f3885-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3885-115">Not supported.</span></span>|
|<span data-ttu-id="f3885-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="f3885-116">Application</span></span>|<span data-ttu-id="f3885-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f3885-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f3885-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f3885-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

## <a name="request-headers"></a><span data-ttu-id="f3885-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="f3885-119">Request headers</span></span>
|<span data-ttu-id="f3885-120">标头</span><span class="sxs-lookup"><span data-stu-id="f3885-120">Header</span></span>|<span data-ttu-id="f3885-121">值</span><span class="sxs-lookup"><span data-stu-id="f3885-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f3885-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f3885-122">Authorization</span></span>|<span data-ttu-id="f3885-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f3885-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f3885-124">接受</span><span class="sxs-lookup"><span data-stu-id="f3885-124">Accept</span></span>|<span data-ttu-id="f3885-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f3885-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f3885-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="f3885-126">Request body</span></span>
<span data-ttu-id="f3885-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f3885-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f3885-128">响应</span><span class="sxs-lookup"><span data-stu-id="f3885-128">Response</span></span>
<span data-ttu-id="f3885-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="f3885-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="f3885-130">示例</span><span class="sxs-lookup"><span data-stu-id="f3885-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="f3885-131">请求</span><span class="sxs-lookup"><span data-stu-id="f3885-131">Request</span></span>
<span data-ttu-id="f3885-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f3885-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}
```

### <a name="response"></a><span data-ttu-id="f3885-133">响应</span><span class="sxs-lookup"><span data-stu-id="f3885-133">Response</span></span>
<span data-ttu-id="f3885-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f3885-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




