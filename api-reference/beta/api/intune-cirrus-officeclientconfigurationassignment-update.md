---
title: 更新 officeClientConfigurationAssignment
description: 更新 officeClientConfigurationAssignment 对象的属性。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: b8546e12dd6f6945240c5dc46e07f281015b3047
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665743"
---
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="6d1ee-103">更新 officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="6d1ee-103">Update officeClientConfigurationAssignment</span></span>

<span data-ttu-id="6d1ee-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6d1ee-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6d1ee-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6d1ee-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6d1ee-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6d1ee-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6d1ee-107">更新 [officeClientConfigurationAssignment 对象](../resources/intune-cirrus-officeclientconfigurationassignment.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="6d1ee-107">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6d1ee-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6d1ee-108">Prerequisites</span></span>
<span data-ttu-id="6d1ee-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6d1ee-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6d1ee-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6d1ee-111">Permission type</span></span>|<span data-ttu-id="6d1ee-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6d1ee-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6d1ee-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6d1ee-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6d1ee-114">\*\*TODO： Determine scopes \*\*</span><span class="sxs-lookup"><span data-stu-id="6d1ee-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="6d1ee-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6d1ee-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6d1ee-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6d1ee-116">Not supported.</span></span>|
|<span data-ttu-id="6d1ee-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6d1ee-117">Application</span></span>|<span data-ttu-id="6d1ee-118">\*\*TODO： Determine scopes \*\*</span><span class="sxs-lookup"><span data-stu-id="6d1ee-118">\*\*TODO: Determine scopes \*\*</span></span>|

## <a name="http-request"></a><span data-ttu-id="6d1ee-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6d1ee-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="6d1ee-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6d1ee-120">Request headers</span></span>
|<span data-ttu-id="6d1ee-121">标头</span><span class="sxs-lookup"><span data-stu-id="6d1ee-121">Header</span></span>|<span data-ttu-id="6d1ee-122">值</span><span class="sxs-lookup"><span data-stu-id="6d1ee-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6d1ee-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6d1ee-123">Authorization</span></span>|<span data-ttu-id="6d1ee-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6d1ee-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6d1ee-125">接受</span><span class="sxs-lookup"><span data-stu-id="6d1ee-125">Accept</span></span>|<span data-ttu-id="6d1ee-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6d1ee-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6d1ee-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6d1ee-127">Request body</span></span>
<span data-ttu-id="6d1ee-128">在请求正文中，提供 [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6d1ee-128">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="6d1ee-129">下表显示创建 [officeClientConfigurationAssignment 时所需的属性](../resources/intune-cirrus-officeclientconfigurationassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="6d1ee-129">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="6d1ee-130">属性</span><span class="sxs-lookup"><span data-stu-id="6d1ee-130">Property</span></span>|<span data-ttu-id="6d1ee-131">类型</span><span class="sxs-lookup"><span data-stu-id="6d1ee-131">Type</span></span>|<span data-ttu-id="6d1ee-132">说明</span><span class="sxs-lookup"><span data-stu-id="6d1ee-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6d1ee-133">id</span><span class="sxs-lookup"><span data-stu-id="6d1ee-133">id</span></span>|<span data-ttu-id="6d1ee-134">String</span><span class="sxs-lookup"><span data-stu-id="6d1ee-134">String</span></span>|<span data-ttu-id="6d1ee-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6d1ee-135">Not yet documented</span></span>|
|<span data-ttu-id="6d1ee-136">target</span><span class="sxs-lookup"><span data-stu-id="6d1ee-136">target</span></span>|[<span data-ttu-id="6d1ee-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="6d1ee-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="6d1ee-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="6d1ee-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="6d1ee-139">响应</span><span class="sxs-lookup"><span data-stu-id="6d1ee-139">Response</span></span>
<span data-ttu-id="6d1ee-140">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="6d1ee-140">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6d1ee-141">示例</span><span class="sxs-lookup"><span data-stu-id="6d1ee-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="6d1ee-142">请求</span><span class="sxs-lookup"><span data-stu-id="6d1ee-142">Request</span></span>
<span data-ttu-id="6d1ee-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6d1ee-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="6d1ee-144">响应</span><span class="sxs-lookup"><span data-stu-id="6d1ee-144">Response</span></span>
<span data-ttu-id="6d1ee-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6d1ee-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




