---
title: setDefaultProfile 操作
description: 尚未记录
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 4087cfdf9e84fd62f6f1ba039506b1901d6989f9
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413624"
---
# <a name="setdefaultprofile-action"></a><span data-ttu-id="df4ca-103">setDefaultProfile 操作</span><span class="sxs-lookup"><span data-stu-id="df4ca-103">setDefaultProfile action</span></span>

> <span data-ttu-id="df4ca-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="df4ca-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="df4ca-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="df4ca-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="df4ca-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="df4ca-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="df4ca-107">尚未记录</span><span class="sxs-lookup"><span data-stu-id="df4ca-107">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="df4ca-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="df4ca-108">Prerequisites</span></span>
<span data-ttu-id="df4ca-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="df4ca-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="df4ca-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="df4ca-111">Permission type</span></span>|<span data-ttu-id="df4ca-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="df4ca-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="df4ca-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df4ca-113">Delegated (work or school account)</span></span>|<span data-ttu-id="df4ca-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df4ca-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="df4ca-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df4ca-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df4ca-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="df4ca-116">Not supported.</span></span>|
|<span data-ttu-id="df4ca-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="df4ca-117">Application</span></span>|<span data-ttu-id="df4ca-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="df4ca-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="df4ca-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df4ca-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/setDefaultProfile
```

## <a name="request-headers"></a><span data-ttu-id="df4ca-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="df4ca-120">Request headers</span></span>
|<span data-ttu-id="df4ca-121">标头</span><span class="sxs-lookup"><span data-stu-id="df4ca-121">Header</span></span>|<span data-ttu-id="df4ca-122">值</span><span class="sxs-lookup"><span data-stu-id="df4ca-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="df4ca-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="df4ca-123">Authorization</span></span>|<span data-ttu-id="df4ca-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="df4ca-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="df4ca-125">Accept</span><span class="sxs-lookup"><span data-stu-id="df4ca-125">Accept</span></span>|<span data-ttu-id="df4ca-126">application/json</span><span class="sxs-lookup"><span data-stu-id="df4ca-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="df4ca-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="df4ca-127">Request body</span></span>
<span data-ttu-id="df4ca-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="df4ca-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="df4ca-129">响应</span><span class="sxs-lookup"><span data-stu-id="df4ca-129">Response</span></span>
<span data-ttu-id="df4ca-130">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="df4ca-130">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="df4ca-131">示例</span><span class="sxs-lookup"><span data-stu-id="df4ca-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="df4ca-132">请求</span><span class="sxs-lookup"><span data-stu-id="df4ca-132">Request</span></span>
<span data-ttu-id="df4ca-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="df4ca-133">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/depOnboardingSettings/{depOnboardingSettingId}/enrollmentProfiles/{enrollmentProfileId}/setDefaultProfile
```

### <a name="response"></a><span data-ttu-id="df4ca-134">响应</span><span class="sxs-lookup"><span data-stu-id="df4ca-134">Response</span></span>
<span data-ttu-id="df4ca-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="df4ca-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




