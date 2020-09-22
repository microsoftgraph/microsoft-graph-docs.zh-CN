---
title: 列出 windowsDomainJoinConfigurations
description: 列出 windowsDomainJoinConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6bfd23b3b5b12e6d00d5e823d16b9c8ccd8113a9
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47999633"
---
# <a name="list-windowsdomainjoinconfigurations"></a><span data-ttu-id="eab0c-103">列出 windowsDomainJoinConfigurations</span><span class="sxs-lookup"><span data-stu-id="eab0c-103">List windowsDomainJoinConfigurations</span></span>

<span data-ttu-id="eab0c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="eab0c-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="eab0c-105">**重要说明：** Microsoft Graph 中的/beta 版本下的 Api 可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="eab0c-105">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="eab0c-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eab0c-106">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eab0c-107">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eab0c-107">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eab0c-108">列出 [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="eab0c-108">List properties and relationships of the [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="eab0c-109">先决条件</span><span class="sxs-lookup"><span data-stu-id="eab0c-109">Prerequisites</span></span>
<span data-ttu-id="eab0c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="eab0c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="eab0c-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="eab0c-112">Permission type</span></span>|<span data-ttu-id="eab0c-113">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eab0c-113">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eab0c-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eab0c-114">Delegated (work or school account)</span></span>||
| <span data-ttu-id="eab0c-115">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="eab0c-115">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="eab0c-116">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eab0c-116">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="eab0c-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eab0c-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eab0c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="eab0c-118">Not supported.</span></span>|
|<span data-ttu-id="eab0c-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="eab0c-119">Application</span></span>||
| <span data-ttu-id="eab0c-120">&nbsp; &nbsp; **设备配置**</span><span class="sxs-lookup"><span data-stu-id="eab0c-120">&nbsp; &nbsp; **Device configuration**</span></span> | <span data-ttu-id="eab0c-121">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="eab0c-121">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="eab0c-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eab0c-122">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="eab0c-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="eab0c-123">Request headers</span></span>
|<span data-ttu-id="eab0c-124">标头</span><span class="sxs-lookup"><span data-stu-id="eab0c-124">Header</span></span>|<span data-ttu-id="eab0c-125">值</span><span class="sxs-lookup"><span data-stu-id="eab0c-125">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eab0c-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="eab0c-126">Authorization</span></span>|<span data-ttu-id="eab0c-127">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eab0c-127">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eab0c-128">接受</span><span class="sxs-lookup"><span data-stu-id="eab0c-128">Accept</span></span>|<span data-ttu-id="eab0c-129">application/json</span><span class="sxs-lookup"><span data-stu-id="eab0c-129">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eab0c-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="eab0c-130">Request body</span></span>
<span data-ttu-id="eab0c-131">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="eab0c-131">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="eab0c-132">响应</span><span class="sxs-lookup"><span data-stu-id="eab0c-132">Response</span></span>
<span data-ttu-id="eab0c-133">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="eab0c-133">If successful, this method returns a `200 OK` response code and a collection of [windowsDomainJoinConfiguration](../resources/intune-shared-windowsdomainjoinconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eab0c-134">示例</span><span class="sxs-lookup"><span data-stu-id="eab0c-134">Example</span></span>
### <a name="request"></a><span data-ttu-id="eab0c-135">请求</span><span class="sxs-lookup"><span data-stu-id="eab0c-135">Request</span></span>
<span data-ttu-id="eab0c-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eab0c-136">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="eab0c-137">响应</span><span class="sxs-lookup"><span data-stu-id="eab0c-137">Response</span></span>
<span data-ttu-id="eab0c-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eab0c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 760

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windowsDomainJoinConfiguration",
      "id": "40118d08-8d08-4011-088d-1140088d1140",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "computerNameStaticPrefix": "Computer Name Static Prefix value",
      "computerNameSuffixRandomCharCount": 1,
      "activeDirectoryDomainName": "Active Directory Domain Name value",
      "organizationalUnit": "Organizational Unit value"
    }
  ]
}
```












