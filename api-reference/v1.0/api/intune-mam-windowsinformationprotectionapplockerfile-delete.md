---
title: 删除 windowsInformationProtectionAppLockerFile
description: 删除 windowsInformationProtectionAppLockerFile。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 080bc1c6f285e62342fbf027718d69bed0a0b791
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27961566"
---
# <a name="delete-windowsinformationprotectionapplockerfile"></a><span data-ttu-id="cf521-103">删除 windowsInformationProtectionAppLockerFile</span><span class="sxs-lookup"><span data-stu-id="cf521-103">Delete windowsInformationProtectionAppLockerFile</span></span>

> <span data-ttu-id="cf521-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cf521-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cf521-105">删除 [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md)。</span><span class="sxs-lookup"><span data-stu-id="cf521-105">Deletes a [windowsInformationProtectionAppLockerFile](../resources/intune-mam-windowsinformationprotectionapplockerfile.md).</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cf521-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="cf521-106">Prerequisites</span></span>
<span data-ttu-id="cf521-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cf521-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cf521-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="cf521-109">Permission type</span></span>|<span data-ttu-id="cf521-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cf521-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cf521-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cf521-111">Delegated (work or school account)</span></span>|<span data-ttu-id="cf521-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cf521-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cf521-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cf521-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cf521-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf521-114">Not supported.</span></span>|
|<span data-ttu-id="cf521-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="cf521-115">Application</span></span>|<span data-ttu-id="cf521-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cf521-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cf521-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cf521-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
DELETE /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
DELETE /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
DELETE /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/protectedAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

## <a name="request-headers"></a><span data-ttu-id="cf521-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="cf521-118">Request headers</span></span>
|<span data-ttu-id="cf521-119">标头</span><span class="sxs-lookup"><span data-stu-id="cf521-119">Header</span></span>|<span data-ttu-id="cf521-120">值</span><span class="sxs-lookup"><span data-stu-id="cf521-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cf521-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="cf521-121">Authorization</span></span>|<span data-ttu-id="cf521-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cf521-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cf521-123">Accept</span><span class="sxs-lookup"><span data-stu-id="cf521-123">Accept</span></span>|<span data-ttu-id="cf521-124">application/json</span><span class="sxs-lookup"><span data-stu-id="cf521-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cf521-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="cf521-125">Request body</span></span>
<span data-ttu-id="cf521-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="cf521-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="cf521-127">响应</span><span class="sxs-lookup"><span data-stu-id="cf521-127">Response</span></span>
<span data-ttu-id="cf521-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="cf521-128">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="cf521-129">示例</span><span class="sxs-lookup"><span data-stu-id="cf521-129">Example</span></span>
### <a name="request"></a><span data-ttu-id="cf521-130">请求</span><span class="sxs-lookup"><span data-stu-id="cf521-130">Request</span></span>
<span data-ttu-id="cf521-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cf521-131">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/v1.0/deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/exemptAppLockerFiles/{windowsInformationProtectionAppLockerFileId}
```

### <a name="response"></a><span data-ttu-id="cf521-132">响应</span><span class="sxs-lookup"><span data-stu-id="cf521-132">Response</span></span>
<span data-ttu-id="cf521-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cf521-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 204 No Content
```



