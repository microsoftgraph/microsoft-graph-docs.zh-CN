---
title: 更新 officeClientConfigurationAssignment
description: 更新 officeClientConfigurationAssignment 对象的属性。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 4a9befac2a3f15fe3bec3b36a5846872a31ef3f5
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39930434"
---
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="4fc1d-103">更新 officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="4fc1d-103">Update officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="4fc1d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4fc1d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fc1d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4fc1d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fc1d-106">更新[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4fc1d-106">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fc1d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4fc1d-107">Prerequisites</span></span>
<span data-ttu-id="4fc1d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4fc1d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fc1d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4fc1d-110">Permission type</span></span>|<span data-ttu-id="4fc1d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4fc1d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fc1d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4fc1d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4fc1d-113">\* \* TODO：确定作用域 \* \*</span><span class="sxs-lookup"><span data-stu-id="4fc1d-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="4fc1d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4fc1d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fc1d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fc1d-115">Not supported.</span></span>|
|<span data-ttu-id="4fc1d-116">Application</span><span class="sxs-lookup"><span data-stu-id="4fc1d-116">Application</span></span>|<span data-ttu-id="4fc1d-117">\* \* TODO：确定作用域 \* \*</span><span class="sxs-lookup"><span data-stu-id="4fc1d-117">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fc1d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4fc1d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="4fc1d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4fc1d-119">Request headers</span></span>
|<span data-ttu-id="4fc1d-120">标头</span><span class="sxs-lookup"><span data-stu-id="4fc1d-120">Header</span></span>|<span data-ttu-id="4fc1d-121">值</span><span class="sxs-lookup"><span data-stu-id="4fc1d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fc1d-122">授权</span><span class="sxs-lookup"><span data-stu-id="4fc1d-122">Authorization</span></span>|<span data-ttu-id="4fc1d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4fc1d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fc1d-124">接受</span><span class="sxs-lookup"><span data-stu-id="4fc1d-124">Accept</span></span>|<span data-ttu-id="4fc1d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4fc1d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fc1d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4fc1d-126">Request body</span></span>
<span data-ttu-id="4fc1d-127">在请求正文中，提供[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4fc1d-127">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="4fc1d-128">下表显示创建[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4fc1d-128">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="4fc1d-129">属性</span><span class="sxs-lookup"><span data-stu-id="4fc1d-129">Property</span></span>|<span data-ttu-id="4fc1d-130">类型</span><span class="sxs-lookup"><span data-stu-id="4fc1d-130">Type</span></span>|<span data-ttu-id="4fc1d-131">说明</span><span class="sxs-lookup"><span data-stu-id="4fc1d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fc1d-132">id</span><span class="sxs-lookup"><span data-stu-id="4fc1d-132">id</span></span>|<span data-ttu-id="4fc1d-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4fc1d-133">String</span></span>|<span data-ttu-id="4fc1d-134">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4fc1d-134">Not yet documented</span></span>|
|<span data-ttu-id="4fc1d-135">target</span><span class="sxs-lookup"><span data-stu-id="4fc1d-135">target</span></span>|[<span data-ttu-id="4fc1d-136">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="4fc1d-136">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="4fc1d-137">尚未记录</span><span class="sxs-lookup"><span data-stu-id="4fc1d-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="4fc1d-138">响应</span><span class="sxs-lookup"><span data-stu-id="4fc1d-138">Response</span></span>
<span data-ttu-id="4fc1d-139">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4fc1d-139">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fc1d-140">示例</span><span class="sxs-lookup"><span data-stu-id="4fc1d-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fc1d-141">请求</span><span class="sxs-lookup"><span data-stu-id="4fc1d-141">Request</span></span>
<span data-ttu-id="4fc1d-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4fc1d-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
Content-type: application/json
Content-length: 98

{
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="4fc1d-143">响应</span><span class="sxs-lookup"><span data-stu-id="4fc1d-143">Response</span></span>
<span data-ttu-id="4fc1d-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4fc1d-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "804730f3-30f3-8047-f330-4780f3304780",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```





