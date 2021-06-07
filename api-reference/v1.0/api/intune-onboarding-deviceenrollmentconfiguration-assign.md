---
title: assign 操作
description: 尚未记录
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 00d0413149350224d9fcf75bebe25ca5857b545f
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52745315"
---
# <a name="assign-action"></a><span data-ttu-id="c455a-103">分配操作</span><span class="sxs-lookup"><span data-stu-id="c455a-103">assign action</span></span>

<span data-ttu-id="c455a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c455a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c455a-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c455a-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c455a-106">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c455a-106">Not yet documented</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c455a-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c455a-107">Prerequisites</span></span>
<span data-ttu-id="c455a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c455a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c455a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c455a-110">Permission type</span></span>|<span data-ttu-id="c455a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c455a-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c455a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c455a-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c455a-113">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c455a-113">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="c455a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c455a-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c455a-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c455a-115">Not supported.</span></span>|
|<span data-ttu-id="c455a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c455a-116">Application</span></span>|<span data-ttu-id="c455a-117">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c455a-117">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c455a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c455a-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign
```

## <a name="request-headers"></a><span data-ttu-id="c455a-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c455a-119">Request headers</span></span>
|<span data-ttu-id="c455a-120">标头</span><span class="sxs-lookup"><span data-stu-id="c455a-120">Header</span></span>|<span data-ttu-id="c455a-121">值</span><span class="sxs-lookup"><span data-stu-id="c455a-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c455a-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c455a-122">Authorization</span></span>|<span data-ttu-id="c455a-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c455a-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c455a-124">接受</span><span class="sxs-lookup"><span data-stu-id="c455a-124">Accept</span></span>|<span data-ttu-id="c455a-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c455a-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c455a-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c455a-126">Request body</span></span>
<span data-ttu-id="c455a-127">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c455a-127">In the request body, supply JSON representation of the parameters.</span></span>

<span data-ttu-id="c455a-128">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="c455a-128">The following table shows the parameters that can be used with this action.</span></span>

|<span data-ttu-id="c455a-129">属性</span><span class="sxs-lookup"><span data-stu-id="c455a-129">Property</span></span>|<span data-ttu-id="c455a-130">类型</span><span class="sxs-lookup"><span data-stu-id="c455a-130">Type</span></span>|<span data-ttu-id="c455a-131">Description</span><span class="sxs-lookup"><span data-stu-id="c455a-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c455a-132">enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="c455a-132">enrollmentConfigurationAssignments</span></span>|<span data-ttu-id="c455a-133">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 集合</span><span class="sxs-lookup"><span data-stu-id="c455a-133">[enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) collection</span></span>|<span data-ttu-id="c455a-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="c455a-134">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="c455a-135">响应</span><span class="sxs-lookup"><span data-stu-id="c455a-135">Response</span></span>
<span data-ttu-id="c455a-136">如果成功，此操作返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="c455a-136">If successful, this action returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="c455a-137">示例</span><span class="sxs-lookup"><span data-stu-id="c455a-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="c455a-138">请求</span><span class="sxs-lookup"><span data-stu-id="c455a-138">Request</span></span>
<span data-ttu-id="c455a-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c455a-139">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assign

Content-type: application/json
Content-length: 360

{
  "enrollmentConfigurationAssignments": [
    {
      "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
      "id": "705b021c-021c-705b-1c02-5b701c025b70",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "collectionId": "Collection Id value"
      }
    }
  ]
}
```

### <a name="response"></a><span data-ttu-id="c455a-140">响应</span><span class="sxs-lookup"><span data-stu-id="c455a-140">Response</span></span>
<span data-ttu-id="c455a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c455a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```




