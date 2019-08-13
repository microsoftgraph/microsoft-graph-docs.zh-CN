---
title: 创建 officeClientConfigurationAssignment
description: 将目标组添加到现有策略中。
localization_priority: Normal
author: rolyon
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b028449b33ce062db0899303b3d98b21af8fb8c3
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/13/2019
ms.locfileid: "36322243"
---
# <a name="create-officeclientconfigurationassignment"></a><span data-ttu-id="08f01-103">创建 officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="08f01-103">Create officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="08f01-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="08f01-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08f01-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08f01-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08f01-106">将目标组添加到现有策略中。</span><span class="sxs-lookup"><span data-stu-id="08f01-106">Add a target group to an existing policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08f01-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="08f01-107">Prerequisites</span></span>
<span data-ttu-id="08f01-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08f01-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08f01-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="08f01-110">Permission type</span></span>|<span data-ttu-id="08f01-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="08f01-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08f01-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08f01-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08f01-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08f01-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="08f01-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08f01-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08f01-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="08f01-115">Not supported.</span></span>|
|<span data-ttu-id="08f01-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="08f01-116">Application</span></span>|<span data-ttu-id="08f01-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08f01-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08f01-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08f01-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{key}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="08f01-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="08f01-119">Request headers</span></span>
|<span data-ttu-id="08f01-120">标头</span><span class="sxs-lookup"><span data-stu-id="08f01-120">Header</span></span>|<span data-ttu-id="08f01-121">值</span><span class="sxs-lookup"><span data-stu-id="08f01-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08f01-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="08f01-122">Authorization</span></span>|<span data-ttu-id="08f01-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="08f01-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08f01-124">接受</span><span class="sxs-lookup"><span data-stu-id="08f01-124">Accept</span></span>|<span data-ttu-id="08f01-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08f01-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08f01-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="08f01-126">Request body</span></span>
<span data-ttu-id="08f01-127">在请求正文中, 提供 officeClientConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08f01-127">In the request body, supply a JSON representation for the officeClientConfigurationAssignment object.</span></span>

<span data-ttu-id="08f01-128">下表显示创建 officeClientConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="08f01-128">The following table shows the properties that are required when you create the officeClientConfigurationAssignment.</span></span>

|<span data-ttu-id="08f01-129">属性</span><span class="sxs-lookup"><span data-stu-id="08f01-129">Property</span></span>|<span data-ttu-id="08f01-130">类型</span><span class="sxs-lookup"><span data-stu-id="08f01-130">Type</span></span>|<span data-ttu-id="08f01-131">说明</span><span class="sxs-lookup"><span data-stu-id="08f01-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08f01-132">id</span><span class="sxs-lookup"><span data-stu-id="08f01-132">id</span></span>|<span data-ttu-id="08f01-133">String</span><span class="sxs-lookup"><span data-stu-id="08f01-133">String</span></span>|<span data-ttu-id="08f01-134">OfficeConfigurationAssignment 的 Id。</span><span class="sxs-lookup"><span data-stu-id="08f01-134">Id of the OfficeConfigurationAssignment.</span></span>|
|<span data-ttu-id="08f01-135">target</span><span class="sxs-lookup"><span data-stu-id="08f01-135">target</span></span>|[<span data-ttu-id="08f01-136">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="08f01-136">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="08f01-137">由管理员定义的目标分配。</span><span class="sxs-lookup"><span data-stu-id="08f01-137">The target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="08f01-138">响应</span><span class="sxs-lookup"><span data-stu-id="08f01-138">Response</span></span>
<span data-ttu-id="08f01-139">如果成功, 此方法在响应`200 Created`正文中返回响应代码和[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="08f01-139">If successful, this method returns a `200 Created` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08f01-140">示例</span><span class="sxs-lookup"><span data-stu-id="08f01-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="08f01-141">请求</span><span class="sxs-lookup"><span data-stu-id="08f01-141">Request</span></span>
<span data-ttu-id="08f01-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="08f01-142">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="08f01-143">响应</span><span class="sxs-lookup"><span data-stu-id="08f01-143">Response</span></span>
<span data-ttu-id="08f01-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="08f01-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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






