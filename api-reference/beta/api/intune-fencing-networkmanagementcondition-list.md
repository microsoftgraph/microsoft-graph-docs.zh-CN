---
title: 列出 networkManagementConditions
description: 列出 networkManagementCondition 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ed7fe993497e164ba983feae748e572e6e5d0039
ms.sourcegitcommit: 20fef447f7e658a454a3887ea49746142c22e45c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/11/2019
ms.locfileid: "31805759"
---
# <a name="list-networkmanagementconditions"></a><span data-ttu-id="eea4c-103">列出 networkManagementConditions</span><span class="sxs-lookup"><span data-stu-id="eea4c-103">List networkManagementConditions</span></span>

> <span data-ttu-id="eea4c-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="eea4c-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="eea4c-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eea4c-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eea4c-106">列出[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eea4c-106">List properties and relationships of the [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eea4c-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="eea4c-107">Prerequisites</span></span>
<span data-ttu-id="eea4c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eea4c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eea4c-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="eea4c-110">Permission type</span></span>|<span data-ttu-id="eea4c-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eea4c-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eea4c-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eea4c-112">Delegated (work or school account)</span></span>|<span data-ttu-id="eea4c-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eea4c-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="eea4c-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eea4c-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eea4c-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="eea4c-115">Not supported.</span></span>|
|<span data-ttu-id="eea4c-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="eea4c-116">Application</span></span>|<span data-ttu-id="eea4c-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="eea4c-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eea4c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eea4c-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managementConditions
GET /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="eea4c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="eea4c-119">Request headers</span></span>
|<span data-ttu-id="eea4c-120">标头</span><span class="sxs-lookup"><span data-stu-id="eea4c-120">Header</span></span>|<span data-ttu-id="eea4c-121">值</span><span class="sxs-lookup"><span data-stu-id="eea4c-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eea4c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="eea4c-122">Authorization</span></span>|<span data-ttu-id="eea4c-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eea4c-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eea4c-124">接受</span><span class="sxs-lookup"><span data-stu-id="eea4c-124">Accept</span></span>|<span data-ttu-id="eea4c-125">application/json</span><span class="sxs-lookup"><span data-stu-id="eea4c-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eea4c-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="eea4c-126">Request body</span></span>
<span data-ttu-id="eea4c-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eea4c-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eea4c-128">响应</span><span class="sxs-lookup"><span data-stu-id="eea4c-128">Response</span></span>
<span data-ttu-id="eea4c-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="eea4c-129">If successful, this method returns a `200 OK` response code and a collection of [networkManagementCondition](../resources/intune-fencing-networkmanagementcondition.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eea4c-130">示例</span><span class="sxs-lookup"><span data-stu-id="eea4c-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="eea4c-131">请求</span><span class="sxs-lookup"><span data-stu-id="eea4c-131">Request</span></span>
<span data-ttu-id="eea4c-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eea4c-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managementConditions
```

### <a name="response"></a><span data-ttu-id="eea4c-133">响应</span><span class="sxs-lookup"><span data-stu-id="eea4c-133">Response</span></span>
<span data-ttu-id="eea4c-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eea4c-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 511

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.networkManagementCondition",
      "id": "c2919b8f-9b8f-c291-8f9b-91c28f9b91c2",
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





