---
title: 列出 appleEnrollmentProfileAssignments
description: 列出 appleEnrollmentProfileAssignment 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 0b4c649b78c4fa798a9051795105f1699877a483
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44792069"
---
# <a name="list-appleenrollmentprofileassignments"></a><span data-ttu-id="799e0-103">列出 appleEnrollmentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="799e0-103">List appleEnrollmentProfileAssignments</span></span>

<span data-ttu-id="799e0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="799e0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="799e0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="799e0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="799e0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="799e0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="799e0-107">列出[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="799e0-107">List properties and relationships of the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="799e0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="799e0-108">Prerequisites</span></span>
<span data-ttu-id="799e0-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="799e0-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="799e0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="799e0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="799e0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="799e0-111">Permission type</span></span>|<span data-ttu-id="799e0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="799e0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="799e0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="799e0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="799e0-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="799e0-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="799e0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="799e0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="799e0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="799e0-116">Not supported.</span></span>|
|<span data-ttu-id="799e0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="799e0-117">Application</span></span>|<span data-ttu-id="799e0-118">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="799e0-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="799e0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="799e0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="799e0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="799e0-120">Request headers</span></span>
|<span data-ttu-id="799e0-121">标头</span><span class="sxs-lookup"><span data-stu-id="799e0-121">Header</span></span>|<span data-ttu-id="799e0-122">值</span><span class="sxs-lookup"><span data-stu-id="799e0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="799e0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="799e0-123">Authorization</span></span>|<span data-ttu-id="799e0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="799e0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="799e0-125">接受</span><span class="sxs-lookup"><span data-stu-id="799e0-125">Accept</span></span>|<span data-ttu-id="799e0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="799e0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="799e0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="799e0-127">Request body</span></span>
<span data-ttu-id="799e0-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="799e0-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="799e0-129">响应</span><span class="sxs-lookup"><span data-stu-id="799e0-129">Response</span></span>
<span data-ttu-id="799e0-130">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="799e0-130">If successful, this method returns a `200 OK` response code and a collection of [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="799e0-131">示例</span><span class="sxs-lookup"><span data-stu-id="799e0-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="799e0-132">请求</span><span class="sxs-lookup"><span data-stu-id="799e0-132">Request</span></span>
<span data-ttu-id="799e0-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="799e0-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
```

### <a name="response"></a><span data-ttu-id="799e0-134">响应</span><span class="sxs-lookup"><span data-stu-id="799e0-134">Response</span></span>
<span data-ttu-id="799e0-135">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="799e0-135">Here is an example of the response.</span></span> <span data-ttu-id="799e0-136">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="799e0-136">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="799e0-137">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="799e0-137">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 437

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
      "id": "5b603771-3771-5b60-7137-605b7137605b",
      "target": {
        "@odata.type": "microsoft.graph.allDevicesAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include"
      }
    }
  ]
}
```



