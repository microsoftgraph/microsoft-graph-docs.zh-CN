---
title: 创建 iosVppEBookAssignment
description: 创建新的 iosVppEBookAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 4f6aa4201d5801f3e235fa28a44d0e38f69fd1bd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133190"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="073b0-103">创建 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="073b0-103">Create iosVppEBookAssignment</span></span>

<span data-ttu-id="073b0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="073b0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="073b0-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="073b0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="073b0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="073b0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="073b0-107">创建新的 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="073b0-107">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="073b0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="073b0-108">Prerequisites</span></span>
<span data-ttu-id="073b0-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="073b0-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="073b0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="073b0-111">Permission type</span></span>|<span data-ttu-id="073b0-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="073b0-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="073b0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="073b0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="073b0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="073b0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="073b0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="073b0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="073b0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="073b0-116">Not supported.</span></span>|
|<span data-ttu-id="073b0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="073b0-117">Application</span></span>|<span data-ttu-id="073b0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="073b0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="073b0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="073b0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="073b0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="073b0-120">Request headers</span></span>
|<span data-ttu-id="073b0-121">标头</span><span class="sxs-lookup"><span data-stu-id="073b0-121">Header</span></span>|<span data-ttu-id="073b0-122">值</span><span class="sxs-lookup"><span data-stu-id="073b0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="073b0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="073b0-123">Authorization</span></span>|<span data-ttu-id="073b0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="073b0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="073b0-125">接受</span><span class="sxs-lookup"><span data-stu-id="073b0-125">Accept</span></span>|<span data-ttu-id="073b0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="073b0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="073b0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="073b0-127">Request body</span></span>
<span data-ttu-id="073b0-128">在请求正文中，提供 iosVppEBookAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="073b0-128">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="073b0-129">下表显示创建 iosVppEBookAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="073b0-129">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="073b0-130">属性</span><span class="sxs-lookup"><span data-stu-id="073b0-130">Property</span></span>|<span data-ttu-id="073b0-131">类型</span><span class="sxs-lookup"><span data-stu-id="073b0-131">Type</span></span>|<span data-ttu-id="073b0-132">说明</span><span class="sxs-lookup"><span data-stu-id="073b0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="073b0-133">id</span><span class="sxs-lookup"><span data-stu-id="073b0-133">id</span></span>|<span data-ttu-id="073b0-134">String</span><span class="sxs-lookup"><span data-stu-id="073b0-134">String</span></span>|<span data-ttu-id="073b0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="073b0-135">Key of the entity.</span></span> <span data-ttu-id="073b0-136">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="073b0-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="073b0-137">target</span><span class="sxs-lookup"><span data-stu-id="073b0-137">target</span></span>|[<span data-ttu-id="073b0-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="073b0-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="073b0-139">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="073b0-139">The assignment target for eBook.</span></span> <span data-ttu-id="073b0-140">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="073b0-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="073b0-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="073b0-141">installIntent</span></span>|[<span data-ttu-id="073b0-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="073b0-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="073b0-143">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="073b0-143">The install intent for eBook.</span></span> <span data-ttu-id="073b0-144">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="073b0-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="073b0-145">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="073b0-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="073b0-146">响应</span><span class="sxs-lookup"><span data-stu-id="073b0-146">Response</span></span>
<span data-ttu-id="073b0-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="073b0-147">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="073b0-148">示例</span><span class="sxs-lookup"><span data-stu-id="073b0-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="073b0-149">请求</span><span class="sxs-lookup"><span data-stu-id="073b0-149">Request</span></span>
<span data-ttu-id="073b0-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="073b0-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 360

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="073b0-151">响应</span><span class="sxs-lookup"><span data-stu-id="073b0-151">Response</span></span>
<span data-ttu-id="073b0-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="073b0-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 409

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "48f05789-5789-48f0-8957-f0488957f048",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "installIntent": "required"
}
```




