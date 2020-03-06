---
title: 更新 managedEBookAssignment
description: 更新 managedEBookAssignment 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: d9c3d6485ac12ec88c58e16d335028bf1f7afa94
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42515544"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="53900-103">更新 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="53900-103">Update managedEBookAssignment</span></span>

<span data-ttu-id="53900-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="53900-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="53900-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53900-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53900-106">更新 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="53900-106">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53900-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="53900-107">Prerequisites</span></span>
<span data-ttu-id="53900-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="53900-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="53900-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="53900-110">Permission type</span></span>|<span data-ttu-id="53900-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="53900-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53900-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53900-112">Delegated (work or school account)</span></span>|<span data-ttu-id="53900-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53900-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="53900-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53900-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53900-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="53900-115">Not supported.</span></span>|
|<span data-ttu-id="53900-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="53900-116">Application</span></span>|<span data-ttu-id="53900-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="53900-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53900-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53900-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="53900-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="53900-119">Request headers</span></span>
|<span data-ttu-id="53900-120">标头</span><span class="sxs-lookup"><span data-stu-id="53900-120">Header</span></span>|<span data-ttu-id="53900-121">值</span><span class="sxs-lookup"><span data-stu-id="53900-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53900-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="53900-122">Authorization</span></span>|<span data-ttu-id="53900-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="53900-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53900-124">接受</span><span class="sxs-lookup"><span data-stu-id="53900-124">Accept</span></span>|<span data-ttu-id="53900-125">application/json</span><span class="sxs-lookup"><span data-stu-id="53900-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53900-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="53900-126">Request body</span></span>
<span data-ttu-id="53900-127">在请求正文中，提供 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53900-127">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="53900-128">下表显示创建 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="53900-128">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="53900-129">属性</span><span class="sxs-lookup"><span data-stu-id="53900-129">Property</span></span>|<span data-ttu-id="53900-130">类型</span><span class="sxs-lookup"><span data-stu-id="53900-130">Type</span></span>|<span data-ttu-id="53900-131">说明</span><span class="sxs-lookup"><span data-stu-id="53900-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53900-132">id</span><span class="sxs-lookup"><span data-stu-id="53900-132">id</span></span>|<span data-ttu-id="53900-133">字符串</span><span class="sxs-lookup"><span data-stu-id="53900-133">String</span></span>|<span data-ttu-id="53900-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="53900-134">Key of the entity.</span></span>|
|<span data-ttu-id="53900-135">target</span><span class="sxs-lookup"><span data-stu-id="53900-135">target</span></span>|[<span data-ttu-id="53900-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="53900-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="53900-137">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="53900-137">The assignment target for eBook.</span></span>|
|<span data-ttu-id="53900-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="53900-138">installIntent</span></span>|[<span data-ttu-id="53900-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="53900-139">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="53900-140">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="53900-140">The install intent for eBook.</span></span> <span data-ttu-id="53900-141">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="53900-141">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="53900-142">响应</span><span class="sxs-lookup"><span data-stu-id="53900-142">Response</span></span>
<span data-ttu-id="53900-143">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="53900-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53900-144">示例</span><span class="sxs-lookup"><span data-stu-id="53900-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="53900-145">请求</span><span class="sxs-lookup"><span data-stu-id="53900-145">Request</span></span>
<span data-ttu-id="53900-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53900-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 194

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="53900-147">响应</span><span class="sxs-lookup"><span data-stu-id="53900-147">Response</span></span>
<span data-ttu-id="53900-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53900-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 243

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```




