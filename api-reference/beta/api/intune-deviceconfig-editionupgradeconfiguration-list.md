---
title: 列出 editionUpgradeConfigurations
description: 列出 editionUpgradeConfiguration 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 0c99f110e2e3ff9fbc51f93f977e3f9fd6db9e58
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30157888"
---
# <a name="list-editionupgradeconfigurations"></a><span data-ttu-id="69f42-103">列出 editionUpgradeConfigurations</span><span class="sxs-lookup"><span data-stu-id="69f42-103">List editionUpgradeConfigurations</span></span>

> <span data-ttu-id="69f42-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="69f42-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="69f42-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="69f42-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="69f42-106">列出 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="69f42-106">List properties and relationships of the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="69f42-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="69f42-107">Prerequisites</span></span>
<span data-ttu-id="69f42-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="69f42-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="69f42-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="69f42-110">Permission type</span></span>|<span data-ttu-id="69f42-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="69f42-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="69f42-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="69f42-112">Delegated (work or school account)</span></span>|<span data-ttu-id="69f42-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="69f42-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="69f42-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="69f42-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="69f42-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="69f42-115">Not supported.</span></span>|
|<span data-ttu-id="69f42-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="69f42-116">Application</span></span>|<span data-ttu-id="69f42-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="69f42-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="69f42-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="69f42-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="69f42-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="69f42-119">Request headers</span></span>
|<span data-ttu-id="69f42-120">标头</span><span class="sxs-lookup"><span data-stu-id="69f42-120">Header</span></span>|<span data-ttu-id="69f42-121">值</span><span class="sxs-lookup"><span data-stu-id="69f42-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="69f42-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="69f42-122">Authorization</span></span>|<span data-ttu-id="69f42-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="69f42-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="69f42-124">Accept</span><span class="sxs-lookup"><span data-stu-id="69f42-124">Accept</span></span>|<span data-ttu-id="69f42-125">application/json</span><span class="sxs-lookup"><span data-stu-id="69f42-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="69f42-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="69f42-126">Request body</span></span>
<span data-ttu-id="69f42-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="69f42-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="69f42-128">响应</span><span class="sxs-lookup"><span data-stu-id="69f42-128">Response</span></span>
<span data-ttu-id="69f42-129">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="69f42-129">If successful, this method returns a `200 OK` response code and a collection of [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="69f42-130">示例</span><span class="sxs-lookup"><span data-stu-id="69f42-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="69f42-131">请求</span><span class="sxs-lookup"><span data-stu-id="69f42-131">Request</span></span>
<span data-ttu-id="69f42-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="69f42-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="69f42-133">响应</span><span class="sxs-lookup"><span data-stu-id="69f42-133">Response</span></span>
<span data-ttu-id="69f42-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="69f42-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 700

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.editionUpgradeConfiguration",
      "id": "f39fc471-c471-f39f-71c4-9ff371c49ff3",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "licenseType": "licenseFile",
      "targetEdition": "windows10EnterpriseN",
      "license": "License value",
      "productKey": "Product Key value",
      "windowsSMode": "block"
    }
  ]
}
```




