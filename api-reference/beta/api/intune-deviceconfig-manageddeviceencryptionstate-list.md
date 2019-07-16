---
title: 列出 managedDeviceEncryptionStates
description: 列出 managedDeviceEncryptionState 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 12d95ec8159e6cd04f119b8c3033882ebb3bd6d9
ms.sourcegitcommit: 3f7bac952864cfa67f749d902d9897f08534c0e3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/16/2019
ms.locfileid: "35715331"
---
# <a name="list-manageddeviceencryptionstates"></a><span data-ttu-id="d0b81-103">列出 managedDeviceEncryptionStates</span><span class="sxs-lookup"><span data-stu-id="d0b81-103">List managedDeviceEncryptionStates</span></span>

> <span data-ttu-id="d0b81-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d0b81-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d0b81-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d0b81-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d0b81-106">列出[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d0b81-106">List properties and relationships of the [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d0b81-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d0b81-107">Prerequisites</span></span>
<span data-ttu-id="d0b81-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d0b81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d0b81-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d0b81-110">Permission type</span></span>|<span data-ttu-id="d0b81-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d0b81-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d0b81-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d0b81-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d0b81-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d0b81-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d0b81-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d0b81-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d0b81-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0b81-115">Not supported.</span></span>|
|<span data-ttu-id="d0b81-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d0b81-116">Application</span></span>|<span data-ttu-id="d0b81-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d0b81-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d0b81-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d0b81-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/managedDeviceEncryptionStates
```

## <a name="request-headers"></a><span data-ttu-id="d0b81-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d0b81-119">Request headers</span></span>
|<span data-ttu-id="d0b81-120">标头</span><span class="sxs-lookup"><span data-stu-id="d0b81-120">Header</span></span>|<span data-ttu-id="d0b81-121">值</span><span class="sxs-lookup"><span data-stu-id="d0b81-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d0b81-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d0b81-122">Authorization</span></span>|<span data-ttu-id="d0b81-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d0b81-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d0b81-124">接受</span><span class="sxs-lookup"><span data-stu-id="d0b81-124">Accept</span></span>|<span data-ttu-id="d0b81-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d0b81-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d0b81-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d0b81-126">Request body</span></span>
<span data-ttu-id="d0b81-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d0b81-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d0b81-128">响应</span><span class="sxs-lookup"><span data-stu-id="d0b81-128">Response</span></span>
<span data-ttu-id="d0b81-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="d0b81-129">If successful, this method returns a `200 OK` response code and a collection of [managedDeviceEncryptionState](../resources/intune-deviceconfig-manageddeviceencryptionstate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d0b81-130">示例</span><span class="sxs-lookup"><span data-stu-id="d0b81-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d0b81-131">请求</span><span class="sxs-lookup"><span data-stu-id="d0b81-131">Request</span></span>
<span data-ttu-id="d0b81-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d0b81-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/managedDeviceEncryptionStates
```

### <a name="response"></a><span data-ttu-id="d0b81-133">响应</span><span class="sxs-lookup"><span data-stu-id="d0b81-133">Response</span></span>
<span data-ttu-id="d0b81-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d0b81-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 862

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.managedDeviceEncryptionState",
      "id": "f09b4ab6-4ab6-f09b-b64a-9bf0b64a9bf0",
      "userPrincipalName": "User Principal Name value",
      "deviceType": "windowsRT",
      "osVersion": "Os Version value",
      "tpmSpecificationVersion": "Tpm Specification Version value",
      "deviceName": "Device Name value",
      "encryptionReadinessState": "ready",
      "encryptionState": "encrypted",
      "encryptionPolicySettingState": "notApplicable",
      "advancedBitLockerStates": "noUserConsent",
      "fileVaultStates": "driveEncryptedByUser",
      "policyDetails": [
        {
          "@odata.type": "microsoft.graph.encryptionReportPolicyDetails",
          "policyId": "Policy Id value",
          "policyName": "Policy Name value"
        }
      ]
    }
  ]
}
```





