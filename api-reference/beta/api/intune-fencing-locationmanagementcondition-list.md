---
title: 列出 locationManagementConditions
description: 列出 locationManagementCondition 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bd3d07f7e75427d33fe01c46297852c990df996e
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43454138"
---
# <a name="list-locationmanagementconditions"></a><span data-ttu-id="84971-103">列出 locationManagementConditions</span><span class="sxs-lookup"><span data-stu-id="84971-103">List locationManagementConditions</span></span>

<span data-ttu-id="84971-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="84971-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="84971-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="84971-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="84971-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="84971-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="84971-107">列出[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="84971-107">List properties and relationships of the [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="84971-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="84971-108">Prerequisites</span></span>
<span data-ttu-id="84971-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="84971-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="84971-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="84971-111">Permission type</span></span>|<span data-ttu-id="84971-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="84971-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="84971-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="84971-113">Delegated (work or school account)</span></span>|<span data-ttu-id="84971-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="84971-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="84971-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="84971-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="84971-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="84971-116">Not supported.</span></span>|
|<span data-ttu-id="84971-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="84971-117">Application</span></span>|<span data-ttu-id="84971-118">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="84971-118">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="84971-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="84971-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="84971-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="84971-120">Request headers</span></span>
|<span data-ttu-id="84971-121">标头</span><span class="sxs-lookup"><span data-stu-id="84971-121">Header</span></span>|<span data-ttu-id="84971-122">值</span><span class="sxs-lookup"><span data-stu-id="84971-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="84971-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="84971-123">Authorization</span></span>|<span data-ttu-id="84971-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="84971-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="84971-125">接受</span><span class="sxs-lookup"><span data-stu-id="84971-125">Accept</span></span>|<span data-ttu-id="84971-126">application/json</span><span class="sxs-lookup"><span data-stu-id="84971-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="84971-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="84971-127">Request body</span></span>
<span data-ttu-id="84971-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="84971-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="84971-129">响应</span><span class="sxs-lookup"><span data-stu-id="84971-129">Response</span></span>
<span data-ttu-id="84971-130">如果成功，此方法在响应`200 OK`正文中返回响应代码和[locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="84971-130">If successful, this method returns a `200 OK` response code and a collection of [locationManagementCondition](../resources/intune-fencing-locationmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="84971-131">示例</span><span class="sxs-lookup"><span data-stu-id="84971-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="84971-132">请求</span><span class="sxs-lookup"><span data-stu-id="84971-132">Request</span></span>
<span data-ttu-id="84971-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="84971-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="84971-134">响应</span><span class="sxs-lookup"><span data-stu-id="84971-134">Response</span></span>
<span data-ttu-id="84971-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="84971-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 512

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.locationManagementCondition",
      "id": "23b1ca32-ca32-23b1-32ca-b12332cab123",
      "uniqueName": "Unique Name value",
      "displayName": "Display Name value",
      "description": "Description value",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
      "eTag": "ETag value",
      "applicablePlatforms": [
        "androidForWork"
      ]
    }
  ]
}
```



