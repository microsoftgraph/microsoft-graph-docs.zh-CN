---
title: 更新 officeClientConfigurationAssignment
description: 更新 officeClientConfigurationAssignment 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 1d71a6fb57b009b8f5e4de1a794a3d92bcc614dc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421814"
---
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="88607-103">更新 officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="88607-103">Update officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="88607-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="88607-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="88607-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="88607-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="88607-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="88607-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="88607-107">更新[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="88607-107">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="88607-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="88607-108">Prerequisites</span></span>
<span data-ttu-id="88607-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="88607-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="88607-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="88607-111">Permission type</span></span>|<span data-ttu-id="88607-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="88607-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="88607-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="88607-113">Delegated (work or school account)</span></span>|<span data-ttu-id="88607-114">\* \* TODO： 确定范围 \* \*</span><span class="sxs-lookup"><span data-stu-id="88607-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="88607-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="88607-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="88607-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="88607-116">Not supported.</span></span>|
|<span data-ttu-id="88607-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="88607-117">Application</span></span>|<span data-ttu-id="88607-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="88607-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="88607-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="88607-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="88607-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="88607-120">Request headers</span></span>
|<span data-ttu-id="88607-121">标头</span><span class="sxs-lookup"><span data-stu-id="88607-121">Header</span></span>|<span data-ttu-id="88607-122">值</span><span class="sxs-lookup"><span data-stu-id="88607-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="88607-123">授权</span><span class="sxs-lookup"><span data-stu-id="88607-123">Authorization</span></span>|<span data-ttu-id="88607-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="88607-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="88607-125">Accept</span><span class="sxs-lookup"><span data-stu-id="88607-125">Accept</span></span>|<span data-ttu-id="88607-126">application/json</span><span class="sxs-lookup"><span data-stu-id="88607-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="88607-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="88607-127">Request body</span></span>
<span data-ttu-id="88607-128">在请求正文中，提供[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="88607-128">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="88607-129">下表显示时创建[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="88607-129">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="88607-130">属性</span><span class="sxs-lookup"><span data-stu-id="88607-130">Property</span></span>|<span data-ttu-id="88607-131">类型</span><span class="sxs-lookup"><span data-stu-id="88607-131">Type</span></span>|<span data-ttu-id="88607-132">说明</span><span class="sxs-lookup"><span data-stu-id="88607-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="88607-133">id</span><span class="sxs-lookup"><span data-stu-id="88607-133">id</span></span>|<span data-ttu-id="88607-134">String</span><span class="sxs-lookup"><span data-stu-id="88607-134">String</span></span>|<span data-ttu-id="88607-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="88607-135">Not yet documented</span></span>|
|<span data-ttu-id="88607-136">target</span><span class="sxs-lookup"><span data-stu-id="88607-136">target</span></span>|[<span data-ttu-id="88607-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="88607-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="88607-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="88607-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="88607-139">响应</span><span class="sxs-lookup"><span data-stu-id="88607-139">Response</span></span>
<span data-ttu-id="88607-140">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="88607-140">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="88607-141">示例</span><span class="sxs-lookup"><span data-stu-id="88607-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="88607-142">请求</span><span class="sxs-lookup"><span data-stu-id="88607-142">Request</span></span>
<span data-ttu-id="88607-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="88607-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="88607-144">响应</span><span class="sxs-lookup"><span data-stu-id="88607-144">Response</span></span>
<span data-ttu-id="88607-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="88607-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



