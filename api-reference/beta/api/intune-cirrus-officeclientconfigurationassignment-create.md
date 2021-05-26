---
title: 创建 officeClientConfigurationAssignment
description: 向现有策略添加目标组。
localization_priority: Normal
author: dougeby
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 777c26c1a41cf5106d9a3beff713e744190235da
ms.sourcegitcommit: 7b8ad226dc9dfee61b8c3d32892534855dad3fa0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/26/2021
ms.locfileid: "52665705"
---
# <a name="create-officeclientconfigurationassignment"></a><span data-ttu-id="b150a-103">创建 officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="b150a-103">Create officeClientConfigurationAssignment</span></span>

<span data-ttu-id="b150a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b150a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b150a-105">**重要提示：** Microsoft Graph /beta 版本下的 API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b150a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b150a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b150a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b150a-107">向现有策略添加目标组。</span><span class="sxs-lookup"><span data-stu-id="b150a-107">Add a target group to an existing policy.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b150a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b150a-108">Prerequisites</span></span>
<span data-ttu-id="b150a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b150a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b150a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b150a-111">Permission type</span></span>|<span data-ttu-id="b150a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b150a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b150a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b150a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b150a-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b150a-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b150a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b150a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b150a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b150a-116">Not supported.</span></span>|
|<span data-ttu-id="b150a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b150a-117">Application</span></span>|<span data-ttu-id="b150a-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b150a-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b150a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b150a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{key}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="b150a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b150a-120">Request headers</span></span>
|<span data-ttu-id="b150a-121">标头</span><span class="sxs-lookup"><span data-stu-id="b150a-121">Header</span></span>|<span data-ttu-id="b150a-122">值</span><span class="sxs-lookup"><span data-stu-id="b150a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b150a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b150a-123">Authorization</span></span>|<span data-ttu-id="b150a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b150a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b150a-125">接受</span><span class="sxs-lookup"><span data-stu-id="b150a-125">Accept</span></span>|<span data-ttu-id="b150a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b150a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b150a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b150a-127">Request body</span></span>
<span data-ttu-id="b150a-128">在请求正文中，提供 officeClientConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b150a-128">In the request body, supply a JSON representation for the officeClientConfigurationAssignment object.</span></span>

<span data-ttu-id="b150a-129">下表显示创建 officeClientConfigurationAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b150a-129">The following table shows the properties that are required when you create the officeClientConfigurationAssignment.</span></span>

|<span data-ttu-id="b150a-130">属性</span><span class="sxs-lookup"><span data-stu-id="b150a-130">Property</span></span>|<span data-ttu-id="b150a-131">类型</span><span class="sxs-lookup"><span data-stu-id="b150a-131">Type</span></span>|<span data-ttu-id="b150a-132">说明</span><span class="sxs-lookup"><span data-stu-id="b150a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b150a-133">id</span><span class="sxs-lookup"><span data-stu-id="b150a-133">id</span></span>|<span data-ttu-id="b150a-134">String</span><span class="sxs-lookup"><span data-stu-id="b150a-134">String</span></span>|<span data-ttu-id="b150a-135">OfficeConfigurationAssignment 的 ID。</span><span class="sxs-lookup"><span data-stu-id="b150a-135">Id of the OfficeConfigurationAssignment.</span></span>|
|<span data-ttu-id="b150a-136">target</span><span class="sxs-lookup"><span data-stu-id="b150a-136">target</span></span>|[<span data-ttu-id="b150a-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b150a-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="b150a-138">由管理员定义的目标分配。</span><span class="sxs-lookup"><span data-stu-id="b150a-138">The target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="b150a-139">响应</span><span class="sxs-lookup"><span data-stu-id="b150a-139">Response</span></span>
<span data-ttu-id="b150a-140">如果成功，此方法在响应正文中返回 响应代码和 `200 Created` [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b150a-140">If successful, this method returns a `200 Created` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b150a-141">示例</span><span class="sxs-lookup"><span data-stu-id="b150a-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="b150a-142">请求</span><span class="sxs-lookup"><span data-stu-id="b150a-142">Request</span></span>
<span data-ttu-id="b150a-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b150a-143">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b150a-144">响应</span><span class="sxs-lookup"><span data-stu-id="b150a-144">Response</span></span>
<span data-ttu-id="b150a-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b150a-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




