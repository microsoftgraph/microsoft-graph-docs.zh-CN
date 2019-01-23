---
title: 列出 editionUpgradeConfigurations
description: 列出 editionUpgradeConfiguration 对象的属性和关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: c6cd9ab1721a4979b76c26f63199c224637b6404
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413106"
---
# <a name="list-editionupgradeconfigurations"></a><span data-ttu-id="b6c96-103">列出 editionUpgradeConfigurations</span><span class="sxs-lookup"><span data-stu-id="b6c96-103">List editionUpgradeConfigurations</span></span>

> <span data-ttu-id="b6c96-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b6c96-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b6c96-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b6c96-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b6c96-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b6c96-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6c96-107">列出 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="b6c96-107">List properties and relationships of the [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6c96-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b6c96-108">Prerequisites</span></span>
<span data-ttu-id="b6c96-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b6c96-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b6c96-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6c96-111">Permission type</span></span>|<span data-ttu-id="b6c96-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b6c96-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6c96-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6c96-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6c96-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="b6c96-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="b6c96-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6c96-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6c96-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6c96-116">Not supported.</span></span>|
|<span data-ttu-id="b6c96-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6c96-117">Application</span></span>|<span data-ttu-id="b6c96-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6c96-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6c96-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6c96-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="b6c96-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6c96-120">Request headers</span></span>
|<span data-ttu-id="b6c96-121">标头</span><span class="sxs-lookup"><span data-stu-id="b6c96-121">Header</span></span>|<span data-ttu-id="b6c96-122">值</span><span class="sxs-lookup"><span data-stu-id="b6c96-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6c96-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6c96-123">Authorization</span></span>|<span data-ttu-id="b6c96-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b6c96-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6c96-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b6c96-125">Accept</span></span>|<span data-ttu-id="b6c96-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6c96-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6c96-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6c96-127">Request body</span></span>
<span data-ttu-id="b6c96-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b6c96-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b6c96-129">响应</span><span class="sxs-lookup"><span data-stu-id="b6c96-129">Response</span></span>
<span data-ttu-id="b6c96-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="b6c96-130">If successful, this method returns a `200 OK` response code and a collection of [editionUpgradeConfiguration](../resources/intune-deviceconfig-editionupgradeconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6c96-131">示例</span><span class="sxs-lookup"><span data-stu-id="b6c96-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6c96-132">请求</span><span class="sxs-lookup"><span data-stu-id="b6c96-132">Request</span></span>
<span data-ttu-id="b6c96-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b6c96-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="b6c96-134">响应</span><span class="sxs-lookup"><span data-stu-id="b6c96-134">Response</span></span>
<span data-ttu-id="b6c96-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b6c96-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




