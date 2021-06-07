---
title: 列出 androidWorkProfileCustomConfigurations
description: 列出 androidWorkProfileCustomConfiguration 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: fac08a8a30f0e743d7a5a2643ec1d86f8fba85e3
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52757155"
---
# <a name="list-androidworkprofilecustomconfigurations"></a><span data-ttu-id="0fb06-103">列出 androidWorkProfileCustomConfigurations</span><span class="sxs-lookup"><span data-stu-id="0fb06-103">List androidWorkProfileCustomConfigurations</span></span>

<span data-ttu-id="0fb06-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0fb06-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="0fb06-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0fb06-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0fb06-106">列出 [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="0fb06-106">List properties and relationships of the [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0fb06-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0fb06-107">Prerequisites</span></span>
<span data-ttu-id="0fb06-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0fb06-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0fb06-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0fb06-110">Permission type</span></span>|<span data-ttu-id="0fb06-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0fb06-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0fb06-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0fb06-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0fb06-113">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fb06-113">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0fb06-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0fb06-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0fb06-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0fb06-115">Not supported.</span></span>|
|<span data-ttu-id="0fb06-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0fb06-116">Application</span></span>|<span data-ttu-id="0fb06-117">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0fb06-117">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="0fb06-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0fb06-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="0fb06-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0fb06-119">Request headers</span></span>
|<span data-ttu-id="0fb06-120">标头</span><span class="sxs-lookup"><span data-stu-id="0fb06-120">Header</span></span>|<span data-ttu-id="0fb06-121">值</span><span class="sxs-lookup"><span data-stu-id="0fb06-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0fb06-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0fb06-122">Authorization</span></span>|<span data-ttu-id="0fb06-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0fb06-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0fb06-124">接受</span><span class="sxs-lookup"><span data-stu-id="0fb06-124">Accept</span></span>|<span data-ttu-id="0fb06-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0fb06-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0fb06-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0fb06-126">Request body</span></span>
<span data-ttu-id="0fb06-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0fb06-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0fb06-128">响应</span><span class="sxs-lookup"><span data-stu-id="0fb06-128">Response</span></span>
<span data-ttu-id="0fb06-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="0fb06-129">If successful, this method returns a `200 OK` response code and a collection of [androidWorkProfileCustomConfiguration](../resources/intune-deviceconfig-androidworkprofilecustomconfiguration.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0fb06-130">示例</span><span class="sxs-lookup"><span data-stu-id="0fb06-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="0fb06-131">请求</span><span class="sxs-lookup"><span data-stu-id="0fb06-131">Request</span></span>
<span data-ttu-id="0fb06-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0fb06-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/v1.0/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="0fb06-133">响应</span><span class="sxs-lookup"><span data-stu-id="0fb06-133">Response</span></span>
<span data-ttu-id="0fb06-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0fb06-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 652

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.androidWorkProfileCustomConfiguration",
      "id": "76c5d59b-d59b-76c5-9bd5-c5769bd5c576",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "omaSettings": [
        {
          "@odata.type": "microsoft.graph.omaSetting",
          "displayName": "Display Name value",
          "description": "Description value",
          "omaUri": "Oma Uri value"
        }
      ]
    }
  ]
}
```




