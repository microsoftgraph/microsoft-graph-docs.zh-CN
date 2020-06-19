---
title: 创建 iosVppEBookAssignment
description: 创建新的 iosVppEBookAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a333b000b4e83a5afb50f0402b82dfa2f68778f7
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793239"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="03024-103">创建 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="03024-103">Create iosVppEBookAssignment</span></span>

<span data-ttu-id="03024-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="03024-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="03024-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="03024-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="03024-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="03024-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="03024-107">创建新的 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="03024-107">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="03024-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="03024-108">Prerequisites</span></span>
<span data-ttu-id="03024-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="03024-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="03024-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="03024-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="03024-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="03024-111">Permission type</span></span>|<span data-ttu-id="03024-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="03024-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="03024-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="03024-113">Delegated (work or school account)</span></span>|<span data-ttu-id="03024-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03024-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="03024-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="03024-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="03024-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="03024-116">Not supported.</span></span>|
|<span data-ttu-id="03024-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="03024-117">Application</span></span>|<span data-ttu-id="03024-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="03024-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="03024-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="03024-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="03024-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="03024-120">Request headers</span></span>
|<span data-ttu-id="03024-121">标头</span><span class="sxs-lookup"><span data-stu-id="03024-121">Header</span></span>|<span data-ttu-id="03024-122">值</span><span class="sxs-lookup"><span data-stu-id="03024-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="03024-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="03024-123">Authorization</span></span>|<span data-ttu-id="03024-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="03024-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="03024-125">接受</span><span class="sxs-lookup"><span data-stu-id="03024-125">Accept</span></span>|<span data-ttu-id="03024-126">application/json</span><span class="sxs-lookup"><span data-stu-id="03024-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="03024-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="03024-127">Request body</span></span>
<span data-ttu-id="03024-128">在请求正文中，提供 iosVppEBookAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="03024-128">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="03024-129">下表显示创建 iosVppEBookAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="03024-129">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="03024-130">属性</span><span class="sxs-lookup"><span data-stu-id="03024-130">Property</span></span>|<span data-ttu-id="03024-131">类型</span><span class="sxs-lookup"><span data-stu-id="03024-131">Type</span></span>|<span data-ttu-id="03024-132">说明</span><span class="sxs-lookup"><span data-stu-id="03024-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="03024-133">id</span><span class="sxs-lookup"><span data-stu-id="03024-133">id</span></span>|<span data-ttu-id="03024-134">String</span><span class="sxs-lookup"><span data-stu-id="03024-134">String</span></span>|<span data-ttu-id="03024-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="03024-135">Key of the entity.</span></span> <span data-ttu-id="03024-136">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="03024-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="03024-137">target</span><span class="sxs-lookup"><span data-stu-id="03024-137">target</span></span>|[<span data-ttu-id="03024-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="03024-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="03024-139">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="03024-139">The assignment target for eBook.</span></span> <span data-ttu-id="03024-140">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="03024-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="03024-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="03024-141">installIntent</span></span>|[<span data-ttu-id="03024-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="03024-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="03024-143">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="03024-143">The install intent for eBook.</span></span> <span data-ttu-id="03024-144">继承自[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="03024-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="03024-145">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="03024-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="03024-146">响应</span><span class="sxs-lookup"><span data-stu-id="03024-146">Response</span></span>
<span data-ttu-id="03024-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="03024-147">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="03024-148">示例</span><span class="sxs-lookup"><span data-stu-id="03024-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="03024-149">请求</span><span class="sxs-lookup"><span data-stu-id="03024-149">Request</span></span>
<span data-ttu-id="03024-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="03024-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="03024-151">响应</span><span class="sxs-lookup"><span data-stu-id="03024-151">Response</span></span>
<span data-ttu-id="03024-152">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="03024-152">Here is an example of the response.</span></span> <span data-ttu-id="03024-153">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="03024-153">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="03024-154">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="03024-154">All of the properties will be returned from an actual call.</span></span>
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



