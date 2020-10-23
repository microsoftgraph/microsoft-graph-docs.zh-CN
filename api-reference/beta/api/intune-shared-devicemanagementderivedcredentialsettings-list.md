---
title: 列出 deviceManagementDerivedCredentialSettingses
description: 列出 deviceManagementDerivedCredentialSettings 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a5e9a9e6cdccce37fefb92093f24923ab9f2fe47
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48706294"
---
# <a name="list-devicemanagementderivedcredentialsettingses"></a><span data-ttu-id="96936-103">列出 deviceManagementDerivedCredentialSettingses</span><span class="sxs-lookup"><span data-stu-id="96936-103">List deviceManagementDerivedCredentialSettingses</span></span>

<span data-ttu-id="96936-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96936-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96936-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="96936-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96936-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96936-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96936-107">列出 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="96936-107">List properties and relationships of the [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96936-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="96936-108">Prerequisites</span></span>
<span data-ttu-id="96936-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96936-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96936-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="96936-111">Permission type</span></span>|<span data-ttu-id="96936-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="96936-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96936-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96936-113">Delegated (work or school account)</span></span>||
|<span data-ttu-id="96936-114">&nbsp;&nbsp;**资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="96936-114">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="96936-115">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="96936-115">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|
|<span data-ttu-id="96936-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96936-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96936-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="96936-117">Not supported.</span></span>|
|<span data-ttu-id="96936-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="96936-118">Application</span></span>||
|<span data-ttu-id="96936-119">&nbsp;&nbsp;**资源访问策略**</span><span class="sxs-lookup"><span data-stu-id="96936-119">&nbsp; &nbsp; **Resource Access Policy**</span></span>|<span data-ttu-id="96936-120">DeviceManagementServiceConfig.ReadWrite.All、DeviceManagementServiceConfig.Read.All</span><span class="sxs-lookup"><span data-stu-id="96936-120">DeviceManagementServiceConfig.ReadWrite.All, DeviceManagementServiceConfig.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96936-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96936-121">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/derivedCredentials
```

## <a name="request-headers"></a><span data-ttu-id="96936-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="96936-122">Request headers</span></span>
|<span data-ttu-id="96936-123">标头</span><span class="sxs-lookup"><span data-stu-id="96936-123">Header</span></span>|<span data-ttu-id="96936-124">值</span><span class="sxs-lookup"><span data-stu-id="96936-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96936-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="96936-125">Authorization</span></span>|<span data-ttu-id="96936-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="96936-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96936-127">接受</span><span class="sxs-lookup"><span data-stu-id="96936-127">Accept</span></span>|<span data-ttu-id="96936-128">application/json</span><span class="sxs-lookup"><span data-stu-id="96936-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96936-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="96936-129">Request body</span></span>
<span data-ttu-id="96936-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="96936-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="96936-131">响应</span><span class="sxs-lookup"><span data-stu-id="96936-131">Response</span></span>
<span data-ttu-id="96936-132">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="96936-132">If successful, this method returns a `200 OK` response code and a collection of [deviceManagementDerivedCredentialSettings](../resources/intune-shared-devicemanagementderivedcredentialsettings.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96936-133">示例</span><span class="sxs-lookup"><span data-stu-id="96936-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="96936-134">请求</span><span class="sxs-lookup"><span data-stu-id="96936-134">Request</span></span>
<span data-ttu-id="96936-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="96936-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/derivedCredentials
```

### <a name="response"></a><span data-ttu-id="96936-136">响应</span><span class="sxs-lookup"><span data-stu-id="96936-136">Response</span></span>
<span data-ttu-id="96936-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="96936-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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









