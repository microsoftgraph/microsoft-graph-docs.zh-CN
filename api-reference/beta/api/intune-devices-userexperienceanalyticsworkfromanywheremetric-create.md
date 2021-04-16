---
title: 创建 userExperienceAnalyticsWorkFromAnywhereMetric
description: 创建新的 userExperienceAnalyticsWorkFromAnywhereMetric 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: f33a06a7c9f9f256476319464a79fadcf680e709
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51868457"
---
# <a name="create-userexperienceanalyticsworkfromanywheremetric"></a><span data-ttu-id="40868-103">创建 userExperienceAnalyticsWorkFromAnywhereMetric</span><span class="sxs-lookup"><span data-stu-id="40868-103">Create userExperienceAnalyticsWorkFromAnywhereMetric</span></span>

<span data-ttu-id="40868-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="40868-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="40868-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="40868-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="40868-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="40868-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="40868-107">创建新的 [userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="40868-107">Create a new [userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="40868-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="40868-108">Prerequisites</span></span>
<span data-ttu-id="40868-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="40868-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="40868-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="40868-111">Permission type</span></span>|<span data-ttu-id="40868-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="40868-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="40868-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="40868-113">Delegated (work or school account)</span></span>|<span data-ttu-id="40868-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40868-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="40868-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="40868-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="40868-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="40868-116">Not supported.</span></span>|
|<span data-ttu-id="40868-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="40868-117">Application</span></span>|<span data-ttu-id="40868-118">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="40868-118">DeviceManagementManagedDevices.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="40868-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="40868-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics
```

## <a name="request-headers"></a><span data-ttu-id="40868-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="40868-120">Request headers</span></span>
|<span data-ttu-id="40868-121">标头</span><span class="sxs-lookup"><span data-stu-id="40868-121">Header</span></span>|<span data-ttu-id="40868-122">值</span><span class="sxs-lookup"><span data-stu-id="40868-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="40868-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="40868-123">Authorization</span></span>|<span data-ttu-id="40868-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="40868-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="40868-125">接受</span><span class="sxs-lookup"><span data-stu-id="40868-125">Accept</span></span>|<span data-ttu-id="40868-126">application/json</span><span class="sxs-lookup"><span data-stu-id="40868-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="40868-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="40868-127">Request body</span></span>
<span data-ttu-id="40868-128">在请求正文中，提供 userExperienceAnalyticsWorkFromAnywhereMetric 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="40868-128">In the request body, supply a JSON representation for the userExperienceAnalyticsWorkFromAnywhereMetric object.</span></span>

<span data-ttu-id="40868-129">下表显示创建 userExperienceAnalyticsWorkFromAnywhereMetric 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="40868-129">The following table shows the properties that are required when you create the userExperienceAnalyticsWorkFromAnywhereMetric.</span></span>

|<span data-ttu-id="40868-130">属性</span><span class="sxs-lookup"><span data-stu-id="40868-130">Property</span></span>|<span data-ttu-id="40868-131">类型</span><span class="sxs-lookup"><span data-stu-id="40868-131">Type</span></span>|<span data-ttu-id="40868-132">说明</span><span class="sxs-lookup"><span data-stu-id="40868-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="40868-133">id</span><span class="sxs-lookup"><span data-stu-id="40868-133">id</span></span>|<span data-ttu-id="40868-134">String</span><span class="sxs-lookup"><span data-stu-id="40868-134">String</span></span>|<span data-ttu-id="40868-135">用户体验分析的唯一标识符在任何指标中都工作。</span><span class="sxs-lookup"><span data-stu-id="40868-135">The unique identifier of the user experience analytics work from anywhere metric.</span></span>|



## <a name="response"></a><span data-ttu-id="40868-136">响应</span><span class="sxs-lookup"><span data-stu-id="40868-136">Response</span></span>
<span data-ttu-id="40868-137">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="40868-137">If successful, this method returns a `201 Created` response code and a [userExperienceAnalyticsWorkFromAnywhereMetric](../resources/intune-devices-userexperienceanalyticsworkfromanywheremetric.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="40868-138">示例</span><span class="sxs-lookup"><span data-stu-id="40868-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="40868-139">请求</span><span class="sxs-lookup"><span data-stu-id="40868-139">Request</span></span>
<span data-ttu-id="40868-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="40868-140">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/userExperienceAnalyticsWorkFromAnywhereMetrics
Content-type: application/json
Content-length: 87

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereMetric"
}
```

### <a name="response"></a><span data-ttu-id="40868-141">响应</span><span class="sxs-lookup"><span data-stu-id="40868-141">Response</span></span>
<span data-ttu-id="40868-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="40868-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 136

{
  "@odata.type": "#microsoft.graph.userExperienceAnalyticsWorkFromAnywhereMetric",
  "id": "7e6fda96-da96-7e6f-96da-6f7e96da6f7e"
}
```




