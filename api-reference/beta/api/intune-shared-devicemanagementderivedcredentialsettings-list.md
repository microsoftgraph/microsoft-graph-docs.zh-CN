---
title: 列出 deviceManagementDerivedCredentialSettingses
description: 列出 deviceManagementDerivedCredentialSettings 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a7dea6677d69695771674a18fa36d756441d5d1b
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43389870"
---
# <a name="list-devicemanagementderivedcredentialsettingses"></a><span data-ttu-id="f7c60-103">列出 deviceManagementDerivedCredentialSettingses</span><span class="sxs-lookup"><span data-stu-id="f7c60-103">List deviceManagementDerivedCredentialSettingses</span></span>

<span data-ttu-id="f7c60-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f7c60-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="f7c60-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="f7c60-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f7c60-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f7c60-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f7c60-107">列出[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="f7c60-107">List properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f7c60-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f7c60-108">Prerequisites</span></span>
<span data-ttu-id="f7c60-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f7c60-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f7c60-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f7c60-111">Permission type</span></span>|<span data-ttu-id="f7c60-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f7c60-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f7c60-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f7c60-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="f7c60-114">&nbsp;&nbsp; **资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="f7c60-114">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="f7c60-115">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7c60-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="f7c60-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f7c60-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f7c60-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="f7c60-117">Not supported.</span></span>|
|<span data-ttu-id="f7c60-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="f7c60-118">Application</span></span>||
|<span data-ttu-id="f7c60-119">&nbsp;&nbsp; **资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="f7c60-119">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="f7c60-120">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="f7c60-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f7c60-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f7c60-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/derivedCredentials
```

## <a name="request-headers"></a><span data-ttu-id="f7c60-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f7c60-122">Request headers</span></span>
|<span data-ttu-id="f7c60-123">标头</span><span class="sxs-lookup"><span data-stu-id="f7c60-123">Header</span></span>|<span data-ttu-id="f7c60-124">值</span><span class="sxs-lookup"><span data-stu-id="f7c60-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f7c60-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f7c60-125">Authorization</span></span>|<span data-ttu-id="f7c60-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f7c60-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f7c60-127">接受</span><span class="sxs-lookup"><span data-stu-id="f7c60-127">Accept</span></span>|<span data-ttu-id="f7c60-128">application/json</span><span class="sxs-lookup"><span data-stu-id="f7c60-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f7c60-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="f7c60-129">Request body</span></span>
<span data-ttu-id="f7c60-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="f7c60-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="f7c60-131">响应</span><span class="sxs-lookup"><span data-stu-id="f7c60-131">Response</span></span>
<span data-ttu-id="f7c60-132">如果成功，此方法在响应`200 OK`正文中返回响应代码和[deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="f7c60-132">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f7c60-133">示例</span><span class="sxs-lookup"><span data-stu-id="f7c60-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="f7c60-134">请求</span><span class="sxs-lookup"><span data-stu-id="f7c60-134">Request</span></span>
<span data-ttu-id="f7c60-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f7c60-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/derivedCredentials
```

### <a name="response"></a><span data-ttu-id="f7c60-136">响应</span><span class="sxs-lookup"><span data-stu-id="f7c60-136">Response</span></span>
<span data-ttu-id="f7c60-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f7c60-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 347

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.deviceManagementDerivedCredentialSettings",
      "id": "bc650741-0741-bc65-4107-65bc410765bc",
      "helpUrl": "https://example.com/helpUrl/",
      "displayName": "Display Name value",
      "issuer": "entrustDatacard",
      "notificationType": "companyPortal"
    }
  ]
}
```







