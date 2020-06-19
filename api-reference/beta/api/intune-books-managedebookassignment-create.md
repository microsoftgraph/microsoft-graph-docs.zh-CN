---
title: 创建 managedEBookAssignment
description: 创建新的 managedEBookAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 099e0038ad4c5481ac84c9b74a66637b496af16a
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793204"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="e06d0-103">创建 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="e06d0-103">Create managedEBookAssignment</span></span>

<span data-ttu-id="e06d0-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e06d0-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e06d0-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e06d0-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e06d0-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e06d0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e06d0-107">创建新的 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e06d0-107">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e06d0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e06d0-108">Prerequisites</span></span>
<span data-ttu-id="e06d0-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="e06d0-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="e06d0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="e06d0-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e06d0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e06d0-111">Permission type</span></span>|<span data-ttu-id="e06d0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e06d0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e06d0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e06d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e06d0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e06d0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="e06d0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e06d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e06d0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e06d0-116">Not supported.</span></span>|
|<span data-ttu-id="e06d0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e06d0-117">Application</span></span>|<span data-ttu-id="e06d0-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e06d0-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e06d0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e06d0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e06d0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e06d0-120">Request headers</span></span>
|<span data-ttu-id="e06d0-121">标头</span><span class="sxs-lookup"><span data-stu-id="e06d0-121">Header</span></span>|<span data-ttu-id="e06d0-122">值</span><span class="sxs-lookup"><span data-stu-id="e06d0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e06d0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e06d0-123">Authorization</span></span>|<span data-ttu-id="e06d0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e06d0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e06d0-125">接受</span><span class="sxs-lookup"><span data-stu-id="e06d0-125">Accept</span></span>|<span data-ttu-id="e06d0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e06d0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e06d0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e06d0-127">Request body</span></span>
<span data-ttu-id="e06d0-128">在请求正文中，提供 managedEBookAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e06d0-128">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="e06d0-129">下表显示创建 managedEBookAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e06d0-129">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="e06d0-130">属性</span><span class="sxs-lookup"><span data-stu-id="e06d0-130">Property</span></span>|<span data-ttu-id="e06d0-131">类型</span><span class="sxs-lookup"><span data-stu-id="e06d0-131">Type</span></span>|<span data-ttu-id="e06d0-132">说明</span><span class="sxs-lookup"><span data-stu-id="e06d0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e06d0-133">id</span><span class="sxs-lookup"><span data-stu-id="e06d0-133">id</span></span>|<span data-ttu-id="e06d0-134">String</span><span class="sxs-lookup"><span data-stu-id="e06d0-134">String</span></span>|<span data-ttu-id="e06d0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e06d0-135">Key of the entity.</span></span>|
|<span data-ttu-id="e06d0-136">target</span><span class="sxs-lookup"><span data-stu-id="e06d0-136">target</span></span>|[<span data-ttu-id="e06d0-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e06d0-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e06d0-138">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="e06d0-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="e06d0-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="e06d0-139">installIntent</span></span>|[<span data-ttu-id="e06d0-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="e06d0-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="e06d0-141">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="e06d0-141">The install intent for eBook.</span></span> <span data-ttu-id="e06d0-142">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="e06d0-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="e06d0-143">响应</span><span class="sxs-lookup"><span data-stu-id="e06d0-143">Response</span></span>
<span data-ttu-id="e06d0-144">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="e06d0-144">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e06d0-145">示例</span><span class="sxs-lookup"><span data-stu-id="e06d0-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="e06d0-146">请求</span><span class="sxs-lookup"><span data-stu-id="e06d0-146">Request</span></span>
<span data-ttu-id="e06d0-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e06d0-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 355

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="e06d0-148">响应</span><span class="sxs-lookup"><span data-stu-id="e06d0-148">Response</span></span>
<span data-ttu-id="e06d0-149">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="e06d0-149">Here is an example of the response.</span></span> <span data-ttu-id="e06d0-150">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="e06d0-150">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="e06d0-151">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="e06d0-151">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 404

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include"
  },
  "installIntent": "required"
}
```



