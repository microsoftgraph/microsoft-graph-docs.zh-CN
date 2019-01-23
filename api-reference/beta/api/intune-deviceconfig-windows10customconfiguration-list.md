---
title: 列出 windows10CustomConfigurations
description: 列出 windows10CustomConfiguration 对象的属性和关系。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 43019ac1e602131fceeb1296ed6aca10947ad588
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29402228"
---
# <a name="list-windows10customconfigurations"></a><span data-ttu-id="77c78-103">列出 windows10CustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="77c78-103">List windows10CustomConfigurations</span></span>

> <span data-ttu-id="77c78-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="77c78-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="77c78-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="77c78-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="77c78-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="77c78-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="77c78-107">列出 [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="77c78-107">List properties and relationships of the [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="77c78-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="77c78-108">Prerequisites</span></span>
<span data-ttu-id="77c78-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="77c78-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="77c78-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="77c78-111">Permission type</span></span>|<span data-ttu-id="77c78-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="77c78-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="77c78-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="77c78-113">Delegated (work or school account)</span></span>|<span data-ttu-id="77c78-114">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="77c78-114">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="77c78-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="77c78-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="77c78-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="77c78-116">Not supported.</span></span>|
|<span data-ttu-id="77c78-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="77c78-117">Application</span></span>|<span data-ttu-id="77c78-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="77c78-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="77c78-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="77c78-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="77c78-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="77c78-120">Request headers</span></span>
|<span data-ttu-id="77c78-121">标头</span><span class="sxs-lookup"><span data-stu-id="77c78-121">Header</span></span>|<span data-ttu-id="77c78-122">值</span><span class="sxs-lookup"><span data-stu-id="77c78-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="77c78-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="77c78-123">Authorization</span></span>|<span data-ttu-id="77c78-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="77c78-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="77c78-125">Accept</span><span class="sxs-lookup"><span data-stu-id="77c78-125">Accept</span></span>|<span data-ttu-id="77c78-126">application/json</span><span class="sxs-lookup"><span data-stu-id="77c78-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="77c78-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="77c78-127">Request body</span></span>
<span data-ttu-id="77c78-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="77c78-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="77c78-129">响应</span><span class="sxs-lookup"><span data-stu-id="77c78-129">Response</span></span>
<span data-ttu-id="77c78-130">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="77c78-130">If successful, this method returns a `200 OK` response code and a collection of [windows10CustomConfiguration](../resources/intune-deviceconfig-windows10customconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="77c78-131">示例</span><span class="sxs-lookup"><span data-stu-id="77c78-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="77c78-132">请求</span><span class="sxs-lookup"><span data-stu-id="77c78-132">Request</span></span>
<span data-ttu-id="77c78-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="77c78-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="77c78-134">响应</span><span class="sxs-lookup"><span data-stu-id="77c78-134">Response</span></span>
<span data-ttu-id="77c78-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="77c78-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 781

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10CustomConfiguration",
      "id": "d8ae266e-266e-d8ae-6e26-aed86e26aed8",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "omaSettings": [
        {
          "@odata.type": "microsoft.graph.omaSettingInteger",
          "displayName": "Display Name value",
          "description": "Description value",
          "omaUri": "Oma Uri value",
          "value": 5
        }
      ]
    }
  ]
}
```




