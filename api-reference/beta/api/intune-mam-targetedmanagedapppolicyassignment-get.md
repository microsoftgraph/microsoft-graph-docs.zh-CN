---
title: 获取 targetedManagedAppPolicyAssignment
description: 读取 targetedManagedAppPolicyAssignment 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: fd5451539eeb97e1611a68fa467a41ca1dfdaa7d
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44791915"
---
# <a name="get-targetedmanagedapppolicyassignment"></a><span data-ttu-id="151fd-103">获取 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="151fd-103">Get targetedManagedAppPolicyAssignment</span></span>

<span data-ttu-id="151fd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="151fd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="151fd-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="151fd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="151fd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="151fd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="151fd-107">读取 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="151fd-107">Read properties and relationships of the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="151fd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="151fd-108">Prerequisites</span></span>
<span data-ttu-id="151fd-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="151fd-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="151fd-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="151fd-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="151fd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="151fd-111">Permission type</span></span>|<span data-ttu-id="151fd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="151fd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="151fd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="151fd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="151fd-114">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="151fd-114">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="151fd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="151fd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="151fd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="151fd-116">Not supported.</span></span>|
|<span data-ttu-id="151fd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="151fd-117">Application</span></span>|<span data-ttu-id="151fd-118">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="151fd-118">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="151fd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="151fd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="151fd-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="151fd-120">Optional query parameters</span></span>
<span data-ttu-id="151fd-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="151fd-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="151fd-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="151fd-122">Request headers</span></span>
|<span data-ttu-id="151fd-123">标头</span><span class="sxs-lookup"><span data-stu-id="151fd-123">Header</span></span>|<span data-ttu-id="151fd-124">值</span><span class="sxs-lookup"><span data-stu-id="151fd-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="151fd-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="151fd-125">Authorization</span></span>|<span data-ttu-id="151fd-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="151fd-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="151fd-127">接受</span><span class="sxs-lookup"><span data-stu-id="151fd-127">Accept</span></span>|<span data-ttu-id="151fd-128">application/json</span><span class="sxs-lookup"><span data-stu-id="151fd-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="151fd-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="151fd-129">Request body</span></span>
<span data-ttu-id="151fd-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="151fd-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="151fd-131">响应</span><span class="sxs-lookup"><span data-stu-id="151fd-131">Response</span></span>
<span data-ttu-id="151fd-132">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="151fd-132">If successful, this method returns a `200 OK` response code and [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="151fd-133">示例</span><span class="sxs-lookup"><span data-stu-id="151fd-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="151fd-134">请求</span><span class="sxs-lookup"><span data-stu-id="151fd-134">Request</span></span>
<span data-ttu-id="151fd-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="151fd-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

### <a name="response"></a><span data-ttu-id="151fd-136">响应</span><span class="sxs-lookup"><span data-stu-id="151fd-136">Response</span></span>
<span data-ttu-id="151fd-137">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="151fd-137">Here is an example of the response.</span></span> <span data-ttu-id="151fd-138">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="151fd-138">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="151fd-139">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="151fd-139">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 476

{
  "value": {
    "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
    "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
    "target": {
      "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
      "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
      "deviceAndAppManagementAssignmentFilterType": "include"
    },
    "source": "policySets",
    "sourceId": "Source Id value"
  }
}
```



