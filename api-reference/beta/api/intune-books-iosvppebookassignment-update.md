---
title: 更新 iosVppEBookAssignment
description: 更新 iosVppEBookAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ee151c333b49189b1a95bb5448cfa8321e128336
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47975624"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="196bd-103">更新 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="196bd-103">Update iosVppEBookAssignment</span></span>

<span data-ttu-id="196bd-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="196bd-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="196bd-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="196bd-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="196bd-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="196bd-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="196bd-107">更新 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="196bd-107">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="196bd-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="196bd-108">Prerequisites</span></span>
<span data-ttu-id="196bd-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="196bd-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="196bd-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="196bd-111">Permission type</span></span>|<span data-ttu-id="196bd-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="196bd-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="196bd-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="196bd-113">Delegated (work or school account)</span></span>|<span data-ttu-id="196bd-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="196bd-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="196bd-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="196bd-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="196bd-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="196bd-116">Not supported.</span></span>|
|<span data-ttu-id="196bd-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="196bd-117">Application</span></span>|<span data-ttu-id="196bd-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="196bd-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="196bd-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="196bd-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="196bd-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="196bd-120">Request headers</span></span>
|<span data-ttu-id="196bd-121">标头</span><span class="sxs-lookup"><span data-stu-id="196bd-121">Header</span></span>|<span data-ttu-id="196bd-122">值</span><span class="sxs-lookup"><span data-stu-id="196bd-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="196bd-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="196bd-123">Authorization</span></span>|<span data-ttu-id="196bd-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="196bd-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="196bd-125">接受</span><span class="sxs-lookup"><span data-stu-id="196bd-125">Accept</span></span>|<span data-ttu-id="196bd-126">application/json</span><span class="sxs-lookup"><span data-stu-id="196bd-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="196bd-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="196bd-127">Request body</span></span>
<span data-ttu-id="196bd-128">在请求正文中，提供 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="196bd-128">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="196bd-129">下表显示创建 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="196bd-129">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="196bd-130">属性</span><span class="sxs-lookup"><span data-stu-id="196bd-130">Property</span></span>|<span data-ttu-id="196bd-131">类型</span><span class="sxs-lookup"><span data-stu-id="196bd-131">Type</span></span>|<span data-ttu-id="196bd-132">说明</span><span class="sxs-lookup"><span data-stu-id="196bd-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="196bd-133">id</span><span class="sxs-lookup"><span data-stu-id="196bd-133">id</span></span>|<span data-ttu-id="196bd-134">String</span><span class="sxs-lookup"><span data-stu-id="196bd-134">String</span></span>|<span data-ttu-id="196bd-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="196bd-135">Key of the entity.</span></span> <span data-ttu-id="196bd-136">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="196bd-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="196bd-137">target</span><span class="sxs-lookup"><span data-stu-id="196bd-137">target</span></span>|[<span data-ttu-id="196bd-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="196bd-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="196bd-139">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="196bd-139">The assignment target for eBook.</span></span> <span data-ttu-id="196bd-140">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="196bd-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="196bd-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="196bd-141">installIntent</span></span>|[<span data-ttu-id="196bd-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="196bd-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="196bd-143">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="196bd-143">The install intent for eBook.</span></span> <span data-ttu-id="196bd-144">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="196bd-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="196bd-145">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="196bd-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="196bd-146">响应</span><span class="sxs-lookup"><span data-stu-id="196bd-146">Response</span></span>
<span data-ttu-id="196bd-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="196bd-147">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="196bd-148">示例</span><span class="sxs-lookup"><span data-stu-id="196bd-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="196bd-149">请求</span><span class="sxs-lookup"><span data-stu-id="196bd-149">Request</span></span>
<span data-ttu-id="196bd-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="196bd-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="196bd-151">响应</span><span class="sxs-lookup"><span data-stu-id="196bd-151">Response</span></span>
<span data-ttu-id="196bd-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="196bd-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






