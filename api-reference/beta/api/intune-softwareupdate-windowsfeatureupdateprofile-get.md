---
title: 获取 windowsFeatureUpdateProfile
description: 读取 windowsFeatureUpdateProfile 对象的属性和关系。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 46131ee1512c47d1d8b1b7afa27f434722566927
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134268"
---
# <a name="get-windowsfeatureupdateprofile"></a><span data-ttu-id="da579-103">获取 windowsFeatureUpdateProfile</span><span class="sxs-lookup"><span data-stu-id="da579-103">Get windowsFeatureUpdateProfile</span></span>

<span data-ttu-id="da579-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="da579-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="da579-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="da579-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da579-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da579-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da579-107">读取 [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) 对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="da579-107">Read properties and relationships of the [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da579-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="da579-108">Prerequisites</span></span>
<span data-ttu-id="da579-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da579-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da579-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="da579-111">Permission type</span></span>|<span data-ttu-id="da579-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="da579-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da579-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da579-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da579-114">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da579-114">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da579-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da579-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da579-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="da579-116">Not supported.</span></span>|
|<span data-ttu-id="da579-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="da579-117">Application</span></span>|<span data-ttu-id="da579-118">DeviceManagementConfiguration.Read.All、DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da579-118">DeviceManagementConfiguration.Read.All, DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da579-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da579-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da579-120">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="da579-120">Optional query parameters</span></span>
<span data-ttu-id="da579-121">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="da579-121">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da579-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="da579-122">Request headers</span></span>
|<span data-ttu-id="da579-123">标头</span><span class="sxs-lookup"><span data-stu-id="da579-123">Header</span></span>|<span data-ttu-id="da579-124">值</span><span class="sxs-lookup"><span data-stu-id="da579-124">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da579-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="da579-125">Authorization</span></span>|<span data-ttu-id="da579-126">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da579-126">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da579-127">接受</span><span class="sxs-lookup"><span data-stu-id="da579-127">Accept</span></span>|<span data-ttu-id="da579-128">application/json</span><span class="sxs-lookup"><span data-stu-id="da579-128">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da579-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="da579-129">Request body</span></span>
<span data-ttu-id="da579-130">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="da579-130">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da579-131">响应</span><span class="sxs-lookup"><span data-stu-id="da579-131">Response</span></span>
<span data-ttu-id="da579-132">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和 [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="da579-132">If successful, this method returns a `200 OK` response code and [windowsFeatureUpdateProfile](../resources/intune-softwareupdate-windowsfeatureupdateprofile.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da579-133">示例</span><span class="sxs-lookup"><span data-stu-id="da579-133">Example</span></span>

### <a name="request"></a><span data-ttu-id="da579-134">请求</span><span class="sxs-lookup"><span data-stu-id="da579-134">Request</span></span>
<span data-ttu-id="da579-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da579-135">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}
```

### <a name="response"></a><span data-ttu-id="da579-136">响应</span><span class="sxs-lookup"><span data-stu-id="da579-136">Response</span></span>
<span data-ttu-id="da579-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da579-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 558

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfile",
    "id": "885bd4ee-d4ee-885b-eed4-5b88eed45b88",
    "displayName": "Display Name value",
    "description": "Description value",
    "featureUpdateVersion": "Feature Update Version value",
    "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
    "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
    "roleScopeTagIds": [
      "Role Scope Tag Ids value"
    ],
    "deployableContentDisplayName": "Deployable Content Display Name value"
  }
}
```




