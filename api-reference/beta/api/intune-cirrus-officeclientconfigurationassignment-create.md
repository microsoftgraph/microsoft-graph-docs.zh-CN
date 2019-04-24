---
title: 创建 officeClientConfigurationAssignment
description: 将目标组添加到现有策略中。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3e646b70ea3e18a79aaee5b4129e54da833c5c4a
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32483822"
---
# <a name="create-officeclientconfigurationassignment"></a><span data-ttu-id="0cc23-103">创建 officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="0cc23-103">Create officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="0cc23-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="0cc23-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="0cc23-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="0cc23-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="0cc23-106">将目标组添加到现有策略中。</span><span class="sxs-lookup"><span data-stu-id="0cc23-106">Add a target group to an existing policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="0cc23-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="0cc23-107">Prerequisites</span></span>
<span data-ttu-id="0cc23-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0cc23-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0cc23-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="0cc23-110">Permission type</span></span>|<span data-ttu-id="0cc23-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="0cc23-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="0cc23-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0cc23-112">Delegated (work or school account)</span></span>|<span data-ttu-id="0cc23-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0cc23-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="0cc23-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0cc23-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0cc23-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cc23-115">Not supported.</span></span>|
|<span data-ttu-id="0cc23-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="0cc23-116">Application</span></span>|<span data-ttu-id="0cc23-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="0cc23-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0cc23-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0cc23-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{key}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="0cc23-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="0cc23-119">Request headers</span></span>
|<span data-ttu-id="0cc23-120">标头</span><span class="sxs-lookup"><span data-stu-id="0cc23-120">Header</span></span>|<span data-ttu-id="0cc23-121">值</span><span class="sxs-lookup"><span data-stu-id="0cc23-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="0cc23-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="0cc23-122">Authorization</span></span>|<span data-ttu-id="0cc23-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="0cc23-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="0cc23-124">接受</span><span class="sxs-lookup"><span data-stu-id="0cc23-124">Accept</span></span>|<span data-ttu-id="0cc23-125">application/json</span><span class="sxs-lookup"><span data-stu-id="0cc23-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="0cc23-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="0cc23-126">Request body</span></span>
<span data-ttu-id="0cc23-127">在请求正文中, 提供 officeClientConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="0cc23-127">In the request body, supply a JSON representation for the officeClientConfigurationAssignment object.</span></span>

<span data-ttu-id="0cc23-128">下表显示创建 officeClientConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="0cc23-128">The following table shows the properties that are required when you create the officeClientConfigurationAssignment.</span></span>

|<span data-ttu-id="0cc23-129">属性</span><span class="sxs-lookup"><span data-stu-id="0cc23-129">Property</span></span>|<span data-ttu-id="0cc23-130">类型</span><span class="sxs-lookup"><span data-stu-id="0cc23-130">Type</span></span>|<span data-ttu-id="0cc23-131">说明</span><span class="sxs-lookup"><span data-stu-id="0cc23-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="0cc23-132">id</span><span class="sxs-lookup"><span data-stu-id="0cc23-132">id</span></span>|<span data-ttu-id="0cc23-133">String</span><span class="sxs-lookup"><span data-stu-id="0cc23-133">String</span></span>|<span data-ttu-id="0cc23-134">OfficeConfigurationAssignment 的 Id。</span><span class="sxs-lookup"><span data-stu-id="0cc23-134">Id of the OfficeConfigurationAssignment.</span></span>|
|<span data-ttu-id="0cc23-135">target</span><span class="sxs-lookup"><span data-stu-id="0cc23-135">target</span></span>|[<span data-ttu-id="0cc23-136">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="0cc23-136">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="0cc23-137">由管理员定义的目标分配。</span><span class="sxs-lookup"><span data-stu-id="0cc23-137">The target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="0cc23-138">响应</span><span class="sxs-lookup"><span data-stu-id="0cc23-138">Response</span></span>
<span data-ttu-id="0cc23-139">如果成功, 此方法在响应`200 Created`正文中返回响应代码和[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="0cc23-139">If successful, this method returns a `200 Created` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="0cc23-140">示例</span><span class="sxs-lookup"><span data-stu-id="0cc23-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="0cc23-141">请求</span><span class="sxs-lookup"><span data-stu-id="0cc23-141">Request</span></span>
<span data-ttu-id="0cc23-142">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0cc23-142">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="0cc23-143">响应</span><span class="sxs-lookup"><span data-stu-id="0cc23-143">Response</span></span>
<span data-ttu-id="0cc23-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0cc23-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



