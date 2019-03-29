---
title: 列出 windows10PFXImportCertificateProfiles
description: 列出 windows10PFXImportCertificateProfile 对象的属性和关系。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 7527fb34fa6750f89b7e2173cd7b0a4053f79673
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30976524"
---
# <a name="list-windows10pfximportcertificateprofiles"></a><span data-ttu-id="d4edd-103">列出 windows10PFXImportCertificateProfiles</span><span class="sxs-lookup"><span data-stu-id="d4edd-103">List windows10PFXImportCertificateProfiles</span></span>

> <span data-ttu-id="d4edd-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d4edd-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d4edd-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d4edd-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d4edd-106">列出[windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="d4edd-106">List properties and relationships of the [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) objects.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d4edd-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d4edd-107">Prerequisites</span></span>
<span data-ttu-id="d4edd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d4edd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4edd-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d4edd-110">Permission type</span></span>|<span data-ttu-id="d4edd-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d4edd-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4edd-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d4edd-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d4edd-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="d4edd-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="d4edd-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d4edd-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4edd-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4edd-115">Not supported.</span></span>|
|<span data-ttu-id="d4edd-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d4edd-116">Application</span></span>|<span data-ttu-id="d4edd-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="d4edd-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4edd-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d4edd-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/deviceConfigurations
GET /deviceManagement/deviceConfigurations/{deviceConfigurationId}/microsoft.graph.windowsDomainJoinConfiguration/networkAccessConfigurations
```

## <a name="request-headers"></a><span data-ttu-id="d4edd-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d4edd-119">Request headers</span></span>
|<span data-ttu-id="d4edd-120">标头</span><span class="sxs-lookup"><span data-stu-id="d4edd-120">Header</span></span>|<span data-ttu-id="d4edd-121">值</span><span class="sxs-lookup"><span data-stu-id="d4edd-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4edd-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4edd-122">Authorization</span></span>|<span data-ttu-id="d4edd-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d4edd-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4edd-124">接受</span><span class="sxs-lookup"><span data-stu-id="d4edd-124">Accept</span></span>|<span data-ttu-id="d4edd-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d4edd-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4edd-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d4edd-126">Request body</span></span>
<span data-ttu-id="d4edd-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="d4edd-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="d4edd-128">响应</span><span class="sxs-lookup"><span data-stu-id="d4edd-128">Response</span></span>
<span data-ttu-id="d4edd-129">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md)对象集合。</span><span class="sxs-lookup"><span data-stu-id="d4edd-129">If successful, this method returns a `200 OK` response code and a collection of [windows10PFXImportCertificateProfile](../resources/intune-deviceconfig-windows10pfximportcertificateprofile.md) objects in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4edd-130">示例</span><span class="sxs-lookup"><span data-stu-id="d4edd-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="d4edd-131">请求</span><span class="sxs-lookup"><span data-stu-id="d4edd-131">Request</span></span>
<span data-ttu-id="d4edd-132">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d4edd-132">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/deviceConfigurations
```

### <a name="response"></a><span data-ttu-id="d4edd-133">响应</span><span class="sxs-lookup"><span data-stu-id="d4edd-133">Response</span></span>
<span data-ttu-id="d4edd-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d4edd-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 570

{
  "value": [
    {
      "@odata.type": "#microsoft.graph.windows10PFXImportCertificateProfile",
      "id": "4244277a-277a-4244-7a27-44427a274442",
      "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
      "roleScopeTagIds": [
        "Role Scope Tag Ids value"
      ],
      "supportsScopeTags": true,
      "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
      "description": "Description value",
      "displayName": "Display Name value",
      "version": 7,
      "keyStorageProvider": "useTpmKspOtherwiseFail"
    }
  ]
}
```




