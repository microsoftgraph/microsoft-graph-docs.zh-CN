---
title: 更新 targetedManagedAppPolicyAssignment
description: 更新 targetedManagedAppPolicyAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 196caa481a4ad22e9f77459335c08ca4975a3e24
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27935029"
---
# <a name="update-targetedmanagedapppolicyassignment"></a><span data-ttu-id="83a72-103">更新 targetedManagedAppPolicyAssignment</span><span class="sxs-lookup"><span data-stu-id="83a72-103">Update targetedManagedAppPolicyAssignment</span></span>

> <span data-ttu-id="83a72-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="83a72-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="83a72-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="83a72-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="83a72-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="83a72-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="83a72-107">更新 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="83a72-107">Update the properties of a [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="83a72-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="83a72-108">Prerequisites</span></span>
<span data-ttu-id="83a72-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="83a72-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="83a72-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="83a72-111">Permission type</span></span>|<span data-ttu-id="83a72-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="83a72-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="83a72-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="83a72-113">Delegated (work or school account)</span></span>|<span data-ttu-id="83a72-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="83a72-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="83a72-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="83a72-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="83a72-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="83a72-116">Not supported.</span></span>|
|<span data-ttu-id="83a72-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="83a72-117">Application</span></span>|<span data-ttu-id="83a72-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="83a72-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="83a72-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="83a72-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/androidManagedAppProtections/{androidManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/targetedManagedAppConfigurations/{targetedManagedAppConfigurationId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/windowsInformationProtectionPolicies/{windowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
PATCH /deviceAppManagement/mdmWindowsInformationProtectionPolicies/{mdmWindowsInformationProtectionPolicyId}/assignments/{targetedManagedAppPolicyAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="83a72-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="83a72-120">Request headers</span></span>
|<span data-ttu-id="83a72-121">标头</span><span class="sxs-lookup"><span data-stu-id="83a72-121">Header</span></span>|<span data-ttu-id="83a72-122">值</span><span class="sxs-lookup"><span data-stu-id="83a72-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="83a72-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="83a72-123">Authorization</span></span>|<span data-ttu-id="83a72-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="83a72-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="83a72-125">Accept</span><span class="sxs-lookup"><span data-stu-id="83a72-125">Accept</span></span>|<span data-ttu-id="83a72-126">application/json</span><span class="sxs-lookup"><span data-stu-id="83a72-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="83a72-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="83a72-127">Request body</span></span>
<span data-ttu-id="83a72-128">在请求正文中，提供 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="83a72-128">In the request body, supply a JSON representation for the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object.</span></span>

<span data-ttu-id="83a72-129">下表显示创建 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="83a72-129">The following table shows the properties that are required when you create the [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md).</span></span>

|<span data-ttu-id="83a72-130">属性</span><span class="sxs-lookup"><span data-stu-id="83a72-130">Property</span></span>|<span data-ttu-id="83a72-131">类型</span><span class="sxs-lookup"><span data-stu-id="83a72-131">Type</span></span>|<span data-ttu-id="83a72-132">说明</span><span class="sxs-lookup"><span data-stu-id="83a72-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="83a72-133">id</span><span class="sxs-lookup"><span data-stu-id="83a72-133">id</span></span>|<span data-ttu-id="83a72-134">String</span><span class="sxs-lookup"><span data-stu-id="83a72-134">String</span></span>|<span data-ttu-id="83a72-135">Id</span><span class="sxs-lookup"><span data-stu-id="83a72-135">Id</span></span>|
|<span data-ttu-id="83a72-136">target</span><span class="sxs-lookup"><span data-stu-id="83a72-136">target</span></span>|[<span data-ttu-id="83a72-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="83a72-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="83a72-138">组或应用的部署标识符</span><span class="sxs-lookup"><span data-stu-id="83a72-138">Identifier for deployment of a group or app</span></span>|



## <a name="response"></a><span data-ttu-id="83a72-139">响应</span><span class="sxs-lookup"><span data-stu-id="83a72-139">Response</span></span>
<span data-ttu-id="83a72-140">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="83a72-140">If successful, this method returns a `200 OK` response code and an updated [targetedManagedAppPolicyAssignment](../resources/intune-mam-targetedmanagedapppolicyassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="83a72-141">示例</span><span class="sxs-lookup"><span data-stu-id="83a72-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="83a72-142">请求</span><span class="sxs-lookup"><span data-stu-id="83a72-142">Request</span></span>
<span data-ttu-id="83a72-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="83a72-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/iosManagedAppProtections/{iosManagedAppProtectionId}/assignments/{targetedManagedAppPolicyAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="83a72-144">响应</span><span class="sxs-lookup"><span data-stu-id="83a72-144">Response</span></span>
<span data-ttu-id="83a72-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="83a72-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 223

{
  "@odata.type": "#microsoft.graph.targetedManagedAppPolicyAssignment",
  "id": "8b68c4a6-c4a6-8b68-a6c4-688ba6c4688b",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





