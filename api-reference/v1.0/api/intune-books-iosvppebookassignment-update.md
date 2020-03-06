---
title: 更新 iosVppEBookAssignment
description: 更新 iosVppEBookAssignment 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 044c1dfc5f070392dadbd372d9c99615a237fe53
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515600"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="fcb39-103">更新 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="fcb39-103">Update iosVppEBookAssignment</span></span>

<span data-ttu-id="fcb39-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fcb39-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="fcb39-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fcb39-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fcb39-106">更新 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fcb39-106">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fcb39-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="fcb39-107">Prerequisites</span></span>
<span data-ttu-id="fcb39-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fcb39-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcb39-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fcb39-110">Permission type</span></span>|<span data-ttu-id="fcb39-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fcb39-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcb39-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fcb39-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fcb39-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcb39-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="fcb39-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fcb39-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcb39-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fcb39-115">Not supported.</span></span>|
|<span data-ttu-id="fcb39-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fcb39-116">Application</span></span>|<span data-ttu-id="fcb39-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fcb39-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcb39-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fcb39-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="fcb39-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fcb39-119">Request headers</span></span>
|<span data-ttu-id="fcb39-120">标头</span><span class="sxs-lookup"><span data-stu-id="fcb39-120">Header</span></span>|<span data-ttu-id="fcb39-121">值</span><span class="sxs-lookup"><span data-stu-id="fcb39-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcb39-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fcb39-122">Authorization</span></span>|<span data-ttu-id="fcb39-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fcb39-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcb39-124">接受</span><span class="sxs-lookup"><span data-stu-id="fcb39-124">Accept</span></span>|<span data-ttu-id="fcb39-125">application/json</span><span class="sxs-lookup"><span data-stu-id="fcb39-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcb39-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="fcb39-126">Request body</span></span>
<span data-ttu-id="fcb39-127">在请求正文中，提供 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fcb39-127">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="fcb39-128">下表显示创建 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fcb39-128">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="fcb39-129">属性</span><span class="sxs-lookup"><span data-stu-id="fcb39-129">Property</span></span>|<span data-ttu-id="fcb39-130">类型</span><span class="sxs-lookup"><span data-stu-id="fcb39-130">Type</span></span>|<span data-ttu-id="fcb39-131">说明</span><span class="sxs-lookup"><span data-stu-id="fcb39-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcb39-132">id</span><span class="sxs-lookup"><span data-stu-id="fcb39-132">id</span></span>|<span data-ttu-id="fcb39-133">字符串</span><span class="sxs-lookup"><span data-stu-id="fcb39-133">String</span></span>|<span data-ttu-id="fcb39-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="fcb39-134">Key of the entity.</span></span> <span data-ttu-id="fcb39-135">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="fcb39-135">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="fcb39-136">target</span><span class="sxs-lookup"><span data-stu-id="fcb39-136">target</span></span>|[<span data-ttu-id="fcb39-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="fcb39-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="fcb39-138">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="fcb39-138">The assignment target for eBook.</span></span> <span data-ttu-id="fcb39-139">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="fcb39-139">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="fcb39-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="fcb39-140">installIntent</span></span>|[<span data-ttu-id="fcb39-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="fcb39-141">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="fcb39-142">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="fcb39-142">The install intent for eBook.</span></span> <span data-ttu-id="fcb39-143">继承自[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="fcb39-143">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="fcb39-144">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="fcb39-144">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="fcb39-145">响应</span><span class="sxs-lookup"><span data-stu-id="fcb39-145">Response</span></span>
<span data-ttu-id="fcb39-146">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fcb39-146">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcb39-147">示例</span><span class="sxs-lookup"><span data-stu-id="fcb39-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="fcb39-148">请求</span><span class="sxs-lookup"><span data-stu-id="fcb39-148">Request</span></span>
<span data-ttu-id="fcb39-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fcb39-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
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

### <a name="response"></a><span data-ttu-id="fcb39-150">响应</span><span class="sxs-lookup"><span data-stu-id="fcb39-150">Response</span></span>
<span data-ttu-id="fcb39-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fcb39-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




