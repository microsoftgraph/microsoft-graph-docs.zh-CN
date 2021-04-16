---
title: 列出 deviceCompliancePolicies
description: 列出 deviceCompliancePolicy 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 41a38f453d524e73dc1d0a3b79718ca559deee02
ms.sourcegitcommit: ed45b5ce0583dfa4d12f7cb0b3ac0c5aeb2318d4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/16/2021
ms.locfileid: "51863371"
---
# <a name="list-devicecompliancepolicies"></a><span data-ttu-id="6f6e1-103">列出 deviceCompliancePolicies</span><span class="sxs-lookup"><span data-stu-id="6f6e1-103">List deviceCompliancePolicies</span></span>

<span data-ttu-id="6f6e1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6f6e1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6f6e1-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6f6e1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6f6e1-107">列出 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-107">List properties and relationships of the [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6f6e1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6f6e1-108">Prerequisites</span></span>
<span data-ttu-id="6f6e1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6f6e1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6f6e1-111">Permission type</span></span>|<span data-ttu-id="6f6e1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6f6e1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6f6e1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6f6e1-113">Delegated (work or school account)</span></span>||
| <span data-ttu-id="6f6e1-114">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="6f6e1-114">&nbsp; &nbsp; **Device configuration**</span></span>  | <span data-ttu-id="6f6e1-115">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f6e1-115">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="6f6e1-116">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="6f6e1-116">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="6f6e1-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f6e1-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="6f6e1-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6f6e1-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6f6e1-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-119">Not supported.</span></span>|
|<span data-ttu-id="6f6e1-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="6f6e1-120">Application</span></span>||
| <span data-ttu-id="6f6e1-121">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="6f6e1-121">&nbsp; &nbsp; **Device configuration**</span></span>  | <span data-ttu-id="6f6e1-122">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f6e1-122">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
| <span data-ttu-id="6f6e1-123">&nbsp;&nbsp;**策略集**</span><span class="sxs-lookup"><span data-stu-id="6f6e1-123">&nbsp; &nbsp; **Policy Set**</span></span> | <span data-ttu-id="6f6e1-124">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="6f6e1-124">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6f6e1-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6f6e1-125">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceCompliancePolicies
```

## <a name="request-headers"></a><span data-ttu-id="6f6e1-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="6f6e1-126">Request headers</span></span>
|<span data-ttu-id="6f6e1-127">标头</span><span class="sxs-lookup"><span data-stu-id="6f6e1-127">Header</span></span>|<span data-ttu-id="6f6e1-128">值</span><span class="sxs-lookup"><span data-stu-id="6f6e1-128">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6f6e1-129">Authorization</span><span class="sxs-lookup"><span data-stu-id="6f6e1-129">Authorization</span></span>|<span data-ttu-id="6f6e1-130">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-130">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6f6e1-131">接受</span><span class="sxs-lookup"><span data-stu-id="6f6e1-131">Accept</span></span>|<span data-ttu-id="6f6e1-132">application/json</span><span class="sxs-lookup"><span data-stu-id="6f6e1-132">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6f6e1-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="6f6e1-133">Request body</span></span>
<span data-ttu-id="6f6e1-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="6f6e1-135">响应</span><span class="sxs-lookup"><span data-stu-id="6f6e1-135">Response</span></span>
<span data-ttu-id="6f6e1-136">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-136">If successful, this method returns a `200 OK` response code and a collection of [deviceCompliancePolicy](../resources/intune-shared-devicecompliancepolicy.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6f6e1-137">示例</span><span class="sxs-lookup"><span data-stu-id="6f6e1-137">Example</span></span>

### <a name="request"></a><span data-ttu-id="6f6e1-138">请求</span><span class="sxs-lookup"><span data-stu-id="6f6e1-138">Request</span></span>
<span data-ttu-id="6f6e1-139">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-139">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceCompliancePolicies
```

### <a name="response"></a><span data-ttu-id="6f6e1-140">响应</span><span class="sxs-lookup"><span data-stu-id="6f6e1-140">Response</span></span>
<span data-ttu-id="6f6e1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6f6e1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 467

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceCompliancePolicy",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "id": "4214b716-b716-4214-16b7-144216b71442",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "displayName": "Display Name value",
      "version": 7
    }
  ]
}
```







