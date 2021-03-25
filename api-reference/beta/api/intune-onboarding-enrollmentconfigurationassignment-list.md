---
title: 列出 enrollmentConfigurationAssignments
description: 列出 enrollmentConfigurationAssignment 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 678af5356670e6699b4c42ed9ead1ed4b6e1fd85
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156882"
---
# <a name="list-enrollmentconfigurationassignments"></a><span data-ttu-id="9cf20-103">列出 enrollmentConfigurationAssignments</span><span class="sxs-lookup"><span data-stu-id="9cf20-103">List enrollmentConfigurationAssignments</span></span>

<span data-ttu-id="9cf20-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="9cf20-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="9cf20-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="9cf20-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="9cf20-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="9cf20-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="9cf20-107">列出 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="9cf20-107">List properties and relationships of the [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="9cf20-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="9cf20-108">Prerequisites</span></span>
<span data-ttu-id="9cf20-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="9cf20-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="9cf20-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="9cf20-111">Permission type</span></span>|<span data-ttu-id="9cf20-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="9cf20-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="9cf20-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="9cf20-113">Delegated (work or school account)</span></span>|<span data-ttu-id="9cf20-114">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cf20-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="9cf20-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="9cf20-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="9cf20-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="9cf20-116">Not supported.</span></span>|
|<span data-ttu-id="9cf20-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="9cf20-117">Application</span></span>|<span data-ttu-id="9cf20-118">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="9cf20-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="9cf20-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="9cf20-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="9cf20-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="9cf20-120">Request headers</span></span>
|<span data-ttu-id="9cf20-121">标头</span><span class="sxs-lookup"><span data-stu-id="9cf20-121">Header</span></span>|<span data-ttu-id="9cf20-122">值</span><span class="sxs-lookup"><span data-stu-id="9cf20-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="9cf20-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="9cf20-123">Authorization</span></span>|<span data-ttu-id="9cf20-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="9cf20-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="9cf20-125">接受</span><span class="sxs-lookup"><span data-stu-id="9cf20-125">Accept</span></span>|<span data-ttu-id="9cf20-126">application/json</span><span class="sxs-lookup"><span data-stu-id="9cf20-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="9cf20-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="9cf20-127">Request body</span></span>
<span data-ttu-id="9cf20-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="9cf20-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="9cf20-129">响应</span><span class="sxs-lookup"><span data-stu-id="9cf20-129">Response</span></span>
<span data-ttu-id="9cf20-130">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和 [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="9cf20-130">If successful, this method returns a `200 OK` response code and a collection of [enrollmentConfigurationAssignment](../resources/intune-onboarding-enrollmentconfigurationassignment.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="9cf20-131">示例</span><span class="sxs-lookup"><span data-stu-id="9cf20-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="9cf20-132">请求</span><span class="sxs-lookup"><span data-stu-id="9cf20-132">Request</span></span>
<span data-ttu-id="9cf20-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="9cf20-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceEnrollmentConfigurations/{deviceEnrollmentConfigurationId}/assignments
```

### <a name="response"></a><span data-ttu-id="9cf20-134">响应</span><span class="sxs-lookup"><span data-stu-id="9cf20-134">Response</span></span>
<span data-ttu-id="9cf20-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="9cf20-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 575

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.enrollmentConfigurationAssignment",
      "id": "705b021c-021c-705b-1c02-5b701c025b70",
      "target": {
        "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
        "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
        "deviceAndAppManagementAssignmentFilterType": "include",
        "collectionId": "Collection Id value"
      },
      "source": "policySets",
      "sourceId": "Source Id value"
    }
  ]
}
```




