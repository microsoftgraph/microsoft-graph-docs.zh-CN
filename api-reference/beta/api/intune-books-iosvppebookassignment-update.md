---
title: 更新 iosVppEBookAssignment
description: 更新 iosVppEBookAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: eded12d6b291cea5247aabac5875cd747cc235c6
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793218"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="b5230-103">更新 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="b5230-103">Update iosVppEBookAssignment</span></span>

<span data-ttu-id="b5230-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5230-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b5230-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b5230-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b5230-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b5230-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b5230-107">更新 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b5230-107">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b5230-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b5230-108">Prerequisites</span></span>
<span data-ttu-id="b5230-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="b5230-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="b5230-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="b5230-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5230-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5230-111">Permission type</span></span>|<span data-ttu-id="b5230-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b5230-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b5230-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5230-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b5230-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5230-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b5230-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5230-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b5230-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b5230-116">Not supported.</span></span>|
|<span data-ttu-id="b5230-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5230-117">Application</span></span>|<span data-ttu-id="b5230-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5230-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b5230-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5230-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="b5230-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5230-120">Request headers</span></span>
|<span data-ttu-id="b5230-121">标头</span><span class="sxs-lookup"><span data-stu-id="b5230-121">Header</span></span>|<span data-ttu-id="b5230-122">值</span><span class="sxs-lookup"><span data-stu-id="b5230-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b5230-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5230-123">Authorization</span></span>|<span data-ttu-id="b5230-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b5230-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b5230-125">接受</span><span class="sxs-lookup"><span data-stu-id="b5230-125">Accept</span></span>|<span data-ttu-id="b5230-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b5230-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5230-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5230-127">Request body</span></span>
<span data-ttu-id="b5230-128">在请求正文中，提供 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b5230-128">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="b5230-129">下表显示创建 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b5230-129">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="b5230-130">属性</span><span class="sxs-lookup"><span data-stu-id="b5230-130">Property</span></span>|<span data-ttu-id="b5230-131">类型</span><span class="sxs-lookup"><span data-stu-id="b5230-131">Type</span></span>|<span data-ttu-id="b5230-132">说明</span><span class="sxs-lookup"><span data-stu-id="b5230-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b5230-133">id</span><span class="sxs-lookup"><span data-stu-id="b5230-133">id</span></span>|<span data-ttu-id="b5230-134">String</span><span class="sxs-lookup"><span data-stu-id="b5230-134">String</span></span>|<span data-ttu-id="b5230-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b5230-135">Key of the entity.</span></span> <span data-ttu-id="b5230-136">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b5230-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="b5230-137">target</span><span class="sxs-lookup"><span data-stu-id="b5230-137">target</span></span>|[<span data-ttu-id="b5230-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="b5230-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="b5230-139">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="b5230-139">The assignment target for eBook.</span></span> <span data-ttu-id="b5230-140">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="b5230-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="b5230-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="b5230-141">installIntent</span></span>|[<span data-ttu-id="b5230-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="b5230-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="b5230-143">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="b5230-143">The install intent for eBook.</span></span> <span data-ttu-id="b5230-144">继承自[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="b5230-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="b5230-145">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="b5230-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="b5230-146">响应</span><span class="sxs-lookup"><span data-stu-id="b5230-146">Response</span></span>
<span data-ttu-id="b5230-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b5230-147">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b5230-148">示例</span><span class="sxs-lookup"><span data-stu-id="b5230-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="b5230-149">请求</span><span class="sxs-lookup"><span data-stu-id="b5230-149">Request</span></span>
<span data-ttu-id="b5230-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5230-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
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

### <a name="response"></a><span data-ttu-id="b5230-151">响应</span><span class="sxs-lookup"><span data-stu-id="b5230-151">Response</span></span>
<span data-ttu-id="b5230-152">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="b5230-152">Here is an example of the response.</span></span> <span data-ttu-id="b5230-153">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="b5230-153">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="b5230-154">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="b5230-154">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



