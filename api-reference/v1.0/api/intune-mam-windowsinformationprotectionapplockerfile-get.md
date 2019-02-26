---
title: 获取 windowsInformationProtectionAppLockerFile
description: 读取 windowsInformationProtectionAppLockerFile 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 2a5cac97f068d64c85c7456376751dc183fd1c71
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30262074"
---
# <a name="get-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="d5c11-103">获取 windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="d5c11-103">Get windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="d5c11-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d5c11-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d5c11-105">读取 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d5c11-105">Read properties and relationships of the [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d5c11-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d5c11-106">Prerequisites</span></span>
<span data-ttu-id="d5c11-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="d5c11-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d5c11-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d5c11-109">Permission type</span></span>|<span data-ttu-id="d5c11-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d5c11-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d5c11-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d5c11-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d5c11-112">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="d5c11-112">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="d5c11-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d5c11-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d5c11-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5c11-114">Not supported.</span></span>|
|<span data-ttu-id="d5c11-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d5c11-115">Application</span></span>|<span data-ttu-id="d5c11-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d5c11-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d5c11-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d5c11-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
GET /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="d5c11-118">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="d5c11-118">Optional query parameters</span></span>
<span data-ttu-id="d5c11-119">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="d5c11-119">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="d5c11-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d5c11-120">Request headers</span></span>
|<span data-ttu-id="d5c11-121">标头</span><span class="sxs-lookup"><span data-stu-id="d5c11-121">Header</span></span>|<span data-ttu-id="d5c11-122">值</span><span class="sxs-lookup"><span data-stu-id="d5c11-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d5c11-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d5c11-123">Authorization</span></span>|<span data-ttu-id="d5c11-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d5c11-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d5c11-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d5c11-125">Accept</span></span>|<span data-ttu-id="d5c11-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d5c11-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d5c11-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d5c11-127">Request body</span></span>
<span data-ttu-id="d5c11-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d5c11-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d5c11-129">响应</span><span class="sxs-lookup"><span data-stu-id="d5c11-129">Response</span></span>
<span data-ttu-id="d5c11-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d5c11-130">If successful, this method returns a `200 OK` response code and [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d5c11-131">示例</span><span class="sxs-lookup"><span data-stu-id="d5c11-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="d5c11-132">请求</span><span class="sxs-lookup"><span data-stu-id="d5c11-132">Request</span></span>
<span data-ttu-id="d5c11-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d5c11-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

### <a name="response"></a><span data-ttu-id="d5c11-134">响应</span><span class="sxs-lookup"><span data-stu-id="d5c11-134">Response</span></span>
<span data-ttu-id="d5c11-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d5c11-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 291

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsInformationProtectionAppLockerFile",
    "displayName": "Display Name value",
    "fileHash": "File Hash value",
    "file": "ZmlsZQ==",
    "id": "d81f0e40-0e40-d81f-400e-1fd8400e1fd8",
    "version": "Version value"
  }
}
```



