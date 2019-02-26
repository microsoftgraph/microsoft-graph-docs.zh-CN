---
title: 创建 iosVppEBookAssignment
description: 创建新的 iosVppEBookAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ffcf4d13c8c04f5c6fb4c8059ae0e7bc7a4b26ad
ms.sourcegitcommit: 873b99d9001d1b2af21836e47f15360b08e10a40
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/26/2019
ms.locfileid: "30259295"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="652fa-103">创建 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="652fa-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="652fa-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="652fa-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="652fa-105">创建新的 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="652fa-105">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="652fa-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="652fa-106">Prerequisites</span></span>
<span data-ttu-id="652fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="652fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="652fa-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="652fa-109">Permission type</span></span>|<span data-ttu-id="652fa-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="652fa-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="652fa-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="652fa-111">Delegated (work or school account)</span></span>|<span data-ttu-id="652fa-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="652fa-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="652fa-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="652fa-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="652fa-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="652fa-114">Not supported.</span></span>|
|<span data-ttu-id="652fa-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="652fa-115">Application</span></span>|<span data-ttu-id="652fa-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="652fa-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="652fa-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="652fa-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="652fa-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="652fa-118">Request headers</span></span>
|<span data-ttu-id="652fa-119">标头</span><span class="sxs-lookup"><span data-stu-id="652fa-119">Header</span></span>|<span data-ttu-id="652fa-120">值</span><span class="sxs-lookup"><span data-stu-id="652fa-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="652fa-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="652fa-121">Authorization</span></span>|<span data-ttu-id="652fa-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="652fa-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="652fa-123">Accept</span><span class="sxs-lookup"><span data-stu-id="652fa-123">Accept</span></span>|<span data-ttu-id="652fa-124">application/json</span><span class="sxs-lookup"><span data-stu-id="652fa-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="652fa-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="652fa-125">Request body</span></span>
<span data-ttu-id="652fa-126">在请求正文中，提供 iosVppEBookAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="652fa-126">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="652fa-127">下表显示创建 iosVppEBookAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="652fa-127">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="652fa-128">属性</span><span class="sxs-lookup"><span data-stu-id="652fa-128">Property</span></span>|<span data-ttu-id="652fa-129">类型</span><span class="sxs-lookup"><span data-stu-id="652fa-129">Type</span></span>|<span data-ttu-id="652fa-130">说明</span><span class="sxs-lookup"><span data-stu-id="652fa-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="652fa-131">id</span><span class="sxs-lookup"><span data-stu-id="652fa-131">id</span></span>|<span data-ttu-id="652fa-132">String</span><span class="sxs-lookup"><span data-stu-id="652fa-132">String</span></span>|<span data-ttu-id="652fa-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="652fa-133">Key of the entity.</span></span> <span data-ttu-id="652fa-134">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="652fa-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="652fa-135">target</span><span class="sxs-lookup"><span data-stu-id="652fa-135">target</span></span>|[<span data-ttu-id="652fa-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="652fa-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="652fa-137">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="652fa-137">The assignment target for eBook.</span></span> <span data-ttu-id="652fa-138">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="652fa-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="652fa-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="652fa-139">installIntent</span></span>|[<span data-ttu-id="652fa-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="652fa-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="652fa-141">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="652fa-141">The install intent for eBook.</span></span> <span data-ttu-id="652fa-142">继承自[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="652fa-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="652fa-143">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="652fa-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="652fa-144">响应</span><span class="sxs-lookup"><span data-stu-id="652fa-144">Response</span></span>
<span data-ttu-id="652fa-145">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="652fa-145">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="652fa-146">示例</span><span class="sxs-lookup"><span data-stu-id="652fa-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="652fa-147">请求</span><span class="sxs-lookup"><span data-stu-id="652fa-147">Request</span></span>
<span data-ttu-id="652fa-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="652fa-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="652fa-149">响应</span><span class="sxs-lookup"><span data-stu-id="652fa-149">Response</span></span>
<span data-ttu-id="652fa-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="652fa-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



