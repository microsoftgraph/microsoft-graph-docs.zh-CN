---
title: 列出 windows10XTrustedRootCertificates
description: 列出 windows10XTrustedRootCertificate 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 75818cad36b196c8b3094bba2f558b3bd5b80454
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51145073"
---
# <a name="list-windows10xtrustedrootcertificates"></a><span data-ttu-id="3c910-103">列出 windows10XTrustedRootCertificates</span><span class="sxs-lookup"><span data-stu-id="3c910-103">List windows10XTrustedRootCertificates</span></span>

<span data-ttu-id="3c910-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c910-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c910-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3c910-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c910-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c910-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c910-107">列出 [windows10XTrustedRootCertificate 对象的属性和](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) 关系。</span><span class="sxs-lookup"><span data-stu-id="3c910-107">List properties and relationships of the [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c910-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3c910-108">Prerequisites</span></span>
<span data-ttu-id="3c910-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c910-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c910-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c910-111">Permission type</span></span>|<span data-ttu-id="3c910-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3c910-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c910-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c910-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c910-114">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c910-114">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="3c910-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c910-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c910-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c910-116">Not supported.</span></span>|
|<span data-ttu-id="3c910-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c910-117">Application</span></span>|<span data-ttu-id="3c910-118">DeviceManagementServiceConfig.Read.All、DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c910-118">DeviceManagementServiceConfig.Read.All, DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c910-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c910-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/resourceAccessProfiles
```

## <a name="request-headers"></a><span data-ttu-id="3c910-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c910-120">Request headers</span></span>
|<span data-ttu-id="3c910-121">标头</span><span class="sxs-lookup"><span data-stu-id="3c910-121">Header</span></span>|<span data-ttu-id="3c910-122">值</span><span class="sxs-lookup"><span data-stu-id="3c910-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c910-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c910-123">Authorization</span></span>|<span data-ttu-id="3c910-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3c910-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c910-125">接受</span><span class="sxs-lookup"><span data-stu-id="3c910-125">Accept</span></span>|<span data-ttu-id="3c910-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c910-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c910-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c910-127">Request body</span></span>
<span data-ttu-id="3c910-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="3c910-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="3c910-129">响应</span><span class="sxs-lookup"><span data-stu-id="3c910-129">Response</span></span>
<span data-ttu-id="3c910-130">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="3c910-130">If successful, this method returns a `200 OK` response code and a collection of [windows10XTrustedRootCertificate](../resources/intune-rapolicy-windows10xtrustedrootcertificate.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c910-131">示例</span><span class="sxs-lookup"><span data-stu-id="3c910-131">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c910-132">请求</span><span class="sxs-lookup"><span data-stu-id="3c910-132">Request</span></span>
<span data-ttu-id="3c910-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c910-133">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/resourceAccessProfiles
```

### <a name="response"></a><span data-ttu-id="3c910-134">响应</span><span class="sxs-lookup"><span data-stu-id="3c910-134">Response</span></span>
<span data-ttu-id="3c910-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3c910-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 654

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10XTrustedRootCertificate",
      "id": "be0bfd01-fd01-be0b-01fd-0bbe01fd0bbe",
      "version": 7,
      "displayName": "Display Name value",
      "description": "Description value",
      "creationDateTime": "2017-01-01T00:00:43.1365422-08:00",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "trustedRootCertificate": "dHJ1c3RlZFJvb3RDZXJ0aWZpY2F0ZQ==",
      "certFileName": "Cert File Name value",
      "destinationStore": "computerCertStoreIntermediate"
    }
  ]
}
```




