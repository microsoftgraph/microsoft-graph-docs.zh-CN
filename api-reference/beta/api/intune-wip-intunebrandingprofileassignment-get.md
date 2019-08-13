---
title: 获取 intuneBrandingProfileAssignment
description: 读取 intuneBrandingProfileAssignment 对象的属性和关系。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: c661cb97601e44b44684f9dde4433168e5c957bb
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36350116"
---
# <a name="get-intunebrandingprofileassignment"></a><span data-ttu-id="da358-103">获取 intuneBrandingProfileAssignment</span><span class="sxs-lookup"><span data-stu-id="da358-103">Get intuneBrandingProfileAssignment</span></span>

> <span data-ttu-id="da358-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="da358-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="da358-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="da358-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="da358-106">读取[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)对象的属性和关系。</span><span class="sxs-lookup"><span data-stu-id="da358-106">Read properties and relationships of the [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="da358-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="da358-107">Prerequisites</span></span>
<span data-ttu-id="da358-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="da358-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da358-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="da358-110">Permission type</span></span>|<span data-ttu-id="da358-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="da358-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da358-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da358-112">Delegated (work or school account)</span></span>|<span data-ttu-id="da358-113">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="da358-113">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|
|<span data-ttu-id="da358-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da358-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da358-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="da358-115">Not supported.</span></span>|
|<span data-ttu-id="da358-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="da358-116">Application</span></span>|<span data-ttu-id="da358-117">DeviceManagementApps.ReadWrite.All、DeviceManagementApps.Read.All</span><span class="sxs-lookup"><span data-stu-id="da358-117">DeviceManagementApps.ReadWrite.All, DeviceManagementApps.Read.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="da358-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da358-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

## <a name="optional-query-parameters"></a><span data-ttu-id="da358-119">可选的查询参数</span><span class="sxs-lookup"><span data-stu-id="da358-119">Optional query parameters</span></span>
<span data-ttu-id="da358-120">此方法支持 [OData 查询参数](https://docs.microsoft.com/en-us/graph/query-parameters) 来帮助自定义响应。</span><span class="sxs-lookup"><span data-stu-id="da358-120">This method supports the [OData Query Parameters](https://docs.microsoft.com/en-us/graph/query-parameters) to help customize the response.</span></span>

## <a name="request-headers"></a><span data-ttu-id="da358-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="da358-121">Request headers</span></span>
|<span data-ttu-id="da358-122">标头</span><span class="sxs-lookup"><span data-stu-id="da358-122">Header</span></span>|<span data-ttu-id="da358-123">值</span><span class="sxs-lookup"><span data-stu-id="da358-123">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da358-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="da358-124">Authorization</span></span>|<span data-ttu-id="da358-125">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da358-125">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da358-126">接受</span><span class="sxs-lookup"><span data-stu-id="da358-126">Accept</span></span>|<span data-ttu-id="da358-127">application/json</span><span class="sxs-lookup"><span data-stu-id="da358-127">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da358-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="da358-128">Request body</span></span>
<span data-ttu-id="da358-129">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="da358-129">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="da358-130">响应</span><span class="sxs-lookup"><span data-stu-id="da358-130">Response</span></span>
<span data-ttu-id="da358-131">如果成功, 此方法在响应`200 OK`正文中返回响应代码和[intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="da358-131">If successful, this method returns a `200 OK` response code and [intuneBrandingProfileAssignment](../resources/intune-wip-intunebrandingprofileassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da358-132">示例</span><span class="sxs-lookup"><span data-stu-id="da358-132">Example</span></span>

### <a name="request"></a><span data-ttu-id="da358-133">请求</span><span class="sxs-lookup"><span data-stu-id="da358-133">Request</span></span>
<span data-ttu-id="da358-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da358-134">Here is an example of the request.</span></span>
``` http
GET https://graph.microsoft.com/beta/deviceManagement/intuneBrandingProfiles/{intuneBrandingProfileId}/assignments/{intuneBrandingProfileAssignmentId}
```

### <a name="response"></a><span data-ttu-id="da358-135">响应</span><span class="sxs-lookup"><span data-stu-id="da358-135">Response</span></span>
<span data-ttu-id="da358-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da358-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 249

{
  "value": {
    "@odata.type": "#microsoft.graph.intuneBrandingProfileAssignment",
    "id": "ee38a117-a117-ee38-17a1-38ee17a138ee",
    "target": {
      "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
    }
  }
}
```






