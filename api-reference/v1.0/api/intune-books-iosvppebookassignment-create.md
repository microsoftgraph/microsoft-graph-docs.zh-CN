---
title: 创建 iosVppEBookAssignment
description: 创建新的 iosVppEBookAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 56a560c45be3c1932636c988c11359125469b6b3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013582"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="678c8-103">创建 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="678c8-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="678c8-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="678c8-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="678c8-105">创建新的 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="678c8-105">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="678c8-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="678c8-106">Prerequisites</span></span>
<span data-ttu-id="678c8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="678c8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="678c8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="678c8-109">Permission type</span></span>|<span data-ttu-id="678c8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="678c8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="678c8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="678c8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="678c8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="678c8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="678c8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="678c8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="678c8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="678c8-114">Not supported.</span></span>|
|<span data-ttu-id="678c8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="678c8-115">Application</span></span>|<span data-ttu-id="678c8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="678c8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="678c8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="678c8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="678c8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="678c8-118">Request headers</span></span>
|<span data-ttu-id="678c8-119">标头</span><span class="sxs-lookup"><span data-stu-id="678c8-119">Header</span></span>|<span data-ttu-id="678c8-120">值</span><span class="sxs-lookup"><span data-stu-id="678c8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="678c8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="678c8-121">Authorization</span></span>|<span data-ttu-id="678c8-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="678c8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="678c8-123">接受</span><span class="sxs-lookup"><span data-stu-id="678c8-123">Accept</span></span>|<span data-ttu-id="678c8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="678c8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="678c8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="678c8-125">Request body</span></span>
<span data-ttu-id="678c8-126">在请求正文中，提供 iosVppEBookAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="678c8-126">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="678c8-127">下表显示创建 iosVppEBookAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="678c8-127">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="678c8-128">属性</span><span class="sxs-lookup"><span data-stu-id="678c8-128">Property</span></span>|<span data-ttu-id="678c8-129">类型</span><span class="sxs-lookup"><span data-stu-id="678c8-129">Type</span></span>|<span data-ttu-id="678c8-130">说明</span><span class="sxs-lookup"><span data-stu-id="678c8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="678c8-131">id</span><span class="sxs-lookup"><span data-stu-id="678c8-131">id</span></span>|<span data-ttu-id="678c8-132">String</span><span class="sxs-lookup"><span data-stu-id="678c8-132">String</span></span>|<span data-ttu-id="678c8-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="678c8-133">Key of the entity.</span></span> <span data-ttu-id="678c8-134">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="678c8-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="678c8-135">target</span><span class="sxs-lookup"><span data-stu-id="678c8-135">target</span></span>|[<span data-ttu-id="678c8-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="678c8-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="678c8-137">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="678c8-137">The assignment target for eBook.</span></span> <span data-ttu-id="678c8-138">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="678c8-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="678c8-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="678c8-139">installIntent</span></span>|[<span data-ttu-id="678c8-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="678c8-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="678c8-141">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="678c8-141">The install intent for eBook.</span></span> <span data-ttu-id="678c8-142">继承自[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="678c8-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="678c8-143">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="678c8-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="678c8-144">响应</span><span class="sxs-lookup"><span data-stu-id="678c8-144">Response</span></span>
<span data-ttu-id="678c8-145">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="678c8-145">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="678c8-146">示例</span><span class="sxs-lookup"><span data-stu-id="678c8-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="678c8-147">请求</span><span class="sxs-lookup"><span data-stu-id="678c8-147">Request</span></span>
<span data-ttu-id="678c8-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="678c8-148">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
Content-type: application/json
Content-length: 193

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="678c8-149">响应</span><span class="sxs-lookup"><span data-stu-id="678c8-149">Response</span></span>
<span data-ttu-id="678c8-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="678c8-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 242

{
  "@odata.type": "#microsoft.graph.iosVppEBookAssignment",
  "id": "48f05789-5789-48f0-8957-f0488957f048",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```



