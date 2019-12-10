---
title: 获取 windowsFeatureUpdateProfileAssignment
description: 读取 windowsFeatureUpdateProfileAssignment 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 64e1d686ae849a4b77525a35b820a58dd4f9135a
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39939246"
---
# <a name="get-windowsfeatureupdateprofileassignment"></a><span data-ttu-id="97520-103">获取 windowsFeatureUpdateProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="97520-103">Get windowsFeatureUpdateProfileAssignment</span></span>

> <span data-ttu-id="97520-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="97520-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="97520-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="97520-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="97520-106">读取[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="97520-106">Read properties and relationships of the [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="97520-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="97520-107">Prerequisites</span></span>
<span data-ttu-id="97520-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="97520-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="97520-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="97520-110">Permission type</span></span>|<span data-ttu-id="97520-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="97520-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="97520-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="97520-112">Delegated (work or school account)</span></span>|<span data-ttu-id="97520-113">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="97520-113">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|
|<span data-ttu-id="97520-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="97520-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="97520-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="97520-115">Not supported.</span></span>|
|<span data-ttu-id="97520-116">Application</span><span class="sxs-lookup"><span data-stu-id="97520-116">Application</span></span>|<span data-ttu-id="97520-117">DeviceManagementConfiguration.ReadWrite.All、DeviceManagementConfiguration.Read.All</span><span class="sxs-lookup"><span data-stu-id="97520-117">DeviceManagementConfiguration.ReadWrite.All, DeviceManagementConfiguration.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="97520-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="97520-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="97520-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="97520-119">Optional query parameters</span></span>
<span data-ttu-id="97520-120">此方法支持 [OData 查询参数](/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="97520-120">This method supports the [OData Query Parameters](/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="97520-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="97520-121">Request headers</span></span>
|<span data-ttu-id="97520-122">标头</span><span class="sxs-lookup"><span data-stu-id="97520-122">Header</span></span>|<span data-ttu-id="97520-123">值</span><span class="sxs-lookup"><span data-stu-id="97520-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="97520-124">授权</span><span class="sxs-lookup"><span data-stu-id="97520-124">Authorization</span></span>|<span data-ttu-id="97520-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="97520-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="97520-126">接受</span><span class="sxs-lookup"><span data-stu-id="97520-126">Accept</span></span>|<span data-ttu-id="97520-127">application/json</span><span class="sxs-lookup"><span data-stu-id="97520-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="97520-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="97520-128">Request body</span></span>
<span data-ttu-id="97520-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="97520-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="97520-130">响应</span><span class="sxs-lookup"><span data-stu-id="97520-130">Response</span></span>
<span data-ttu-id="97520-131">如果成功，此方法在响应`200 OK`正文中返回响应代码和[windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="97520-131">If successful, this method returns a `200 OK` response code and [windowsFeatureUpdateProfileAssignment](../resources/intune-softwareupdate-windowsfeatureupdateprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="97520-132">示例</span><span class="sxs-lookup"><span data-stu-id="97520-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="97520-133">请求</span><span class="sxs-lookup"><span data-stu-id="97520-133">Request</span></span>
<span data-ttu-id="97520-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="97520-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/windowsFeatureUpdateProfiles/{windowsFeatureUpdateProfileId}/assignments/{windowsFeatureUpdateProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="97520-135">响应</span><span class="sxs-lookup"><span data-stu-id="97520-135">Response</span></span>
<span data-ttu-id="97520-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="97520-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 255

{
  "value": {
    "@odata.type": "#microsoft.graph.windowsFeatureUpdateProfileAssignment",
    "id": "567a744f-744f-567a-4f74-7a564f747a56",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```





