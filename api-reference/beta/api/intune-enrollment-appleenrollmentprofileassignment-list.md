---
title: 列出 appleEnrollmentProfileAssignments
description: 列出 appleEnrollmentProfileAssignment 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 406de661b5f485c31e958e5f96e688518ec810b4
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42467506"
---
# <a name="list-appleenrollmentprofileassignments"></a><span data-ttu-id="ff95f-103">列出 appleEnrollmentProfileAssignments</span><span class="sxs-lookup"><span data-stu-id="ff95f-103">List appleEnrollmentProfileAssignments</span></span>

<span data-ttu-id="ff95f-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ff95f-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="ff95f-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="ff95f-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ff95f-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="ff95f-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ff95f-107">列出[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="ff95f-107">List properties and relationships of the [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ff95f-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ff95f-108">Prerequisites</span></span>
<span data-ttu-id="ff95f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ff95f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ff95f-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ff95f-111">Permission type</span></span>|<span data-ttu-id="ff95f-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ff95f-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ff95f-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ff95f-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ff95f-114">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff95f-114">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="ff95f-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ff95f-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ff95f-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ff95f-116">Not supported.</span></span>|
|<span data-ttu-id="ff95f-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ff95f-117">Application</span></span>|<span data-ttu-id="ff95f-118">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="ff95f-118">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="ff95f-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ff95f-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ff95f-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ff95f-120">Request headers</span></span>
|<span data-ttu-id="ff95f-121">标头</span><span class="sxs-lookup"><span data-stu-id="ff95f-121">Header</span></span>|<span data-ttu-id="ff95f-122">值</span><span class="sxs-lookup"><span data-stu-id="ff95f-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ff95f-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ff95f-123">Authorization</span></span>|<span data-ttu-id="ff95f-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ff95f-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ff95f-125">接受</span><span class="sxs-lookup"><span data-stu-id="ff95f-125">Accept</span></span>|<span data-ttu-id="ff95f-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ff95f-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ff95f-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ff95f-127">Request body</span></span>
<span data-ttu-id="ff95f-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ff95f-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ff95f-129">响应</span><span class="sxs-lookup"><span data-stu-id="ff95f-129">Response</span></span>
<span data-ttu-id="ff95f-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="ff95f-130">If successful, this method returns a `200 OK` response code and a collection of [appleEnrollmentProfileAssignment](../resources/intune-enrollment-appleenrollmentprofileassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ff95f-131">示例</span><span class="sxs-lookup"><span data-stu-id="ff95f-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="ff95f-132">请求</span><span class="sxs-lookup"><span data-stu-id="ff95f-132">Request</span></span>
<span data-ttu-id="ff95f-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ff95f-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/appleUserInitiatedEnrollmentProfiles/{appleUserInitiatedEnrollmentProfileId}/assignments
```

### <a name="response"></a><span data-ttu-id="ff95f-134">响应</span><span class="sxs-lookup"><span data-stu-id="ff95f-134">Response</span></span>
<span data-ttu-id="ff95f-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ff95f-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 274

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.appleEnrollmentProfileAssignment",
      "id": "5b603771-3771-5b60-7137-605b7137605b",
      "target": {
        "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
      }
    }
  ]
}
```





