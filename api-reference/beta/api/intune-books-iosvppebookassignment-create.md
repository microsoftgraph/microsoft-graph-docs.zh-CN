---
title: 创建 iosVppEBookAssignment
description: 创建新的 iosVppEBookAssignment 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b8170738d48811d8d4b9a1e672d6284fcb115f76
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42760471"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="bae28-103">创建 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="bae28-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="bae28-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bae28-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bae28-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bae28-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bae28-106">创建新的 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bae28-106">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bae28-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="bae28-107">Prerequisites</span></span>
<span data-ttu-id="bae28-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bae28-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bae28-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="bae28-110">Permission type</span></span>|<span data-ttu-id="bae28-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bae28-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bae28-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bae28-112">Delegated (work or school account)</span></span>|<span data-ttu-id="bae28-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bae28-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bae28-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bae28-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bae28-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="bae28-115">Not supported.</span></span>|
|<span data-ttu-id="bae28-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="bae28-116">Application</span></span>|<span data-ttu-id="bae28-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bae28-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bae28-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bae28-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="bae28-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="bae28-119">Request headers</span></span>
|<span data-ttu-id="bae28-120">标头</span><span class="sxs-lookup"><span data-stu-id="bae28-120">Header</span></span>|<span data-ttu-id="bae28-121">值</span><span class="sxs-lookup"><span data-stu-id="bae28-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bae28-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="bae28-122">Authorization</span></span>|<span data-ttu-id="bae28-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bae28-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bae28-124">接受</span><span class="sxs-lookup"><span data-stu-id="bae28-124">Accept</span></span>|<span data-ttu-id="bae28-125">application/json</span><span class="sxs-lookup"><span data-stu-id="bae28-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bae28-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="bae28-126">Request body</span></span>
<span data-ttu-id="bae28-127">在请求正文中，提供 iosVppEBookAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bae28-127">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="bae28-128">下表显示创建 iosVppEBookAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bae28-128">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="bae28-129">属性</span><span class="sxs-lookup"><span data-stu-id="bae28-129">Property</span></span>|<span data-ttu-id="bae28-130">类型</span><span class="sxs-lookup"><span data-stu-id="bae28-130">Type</span></span>|<span data-ttu-id="bae28-131">说明</span><span class="sxs-lookup"><span data-stu-id="bae28-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bae28-132">id</span><span class="sxs-lookup"><span data-stu-id="bae28-132">id</span></span>|<span data-ttu-id="bae28-133">String</span><span class="sxs-lookup"><span data-stu-id="bae28-133">String</span></span>|<span data-ttu-id="bae28-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bae28-134">Key of the entity.</span></span> <span data-ttu-id="bae28-135">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="bae28-135">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="bae28-136">target</span><span class="sxs-lookup"><span data-stu-id="bae28-136">target</span></span>|[<span data-ttu-id="bae28-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="bae28-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="bae28-138">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="bae28-138">The assignment target for eBook.</span></span> <span data-ttu-id="bae28-139">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="bae28-139">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="bae28-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="bae28-140">installIntent</span></span>|[<span data-ttu-id="bae28-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="bae28-141">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="bae28-142">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="bae28-142">The install intent for eBook.</span></span> <span data-ttu-id="bae28-143">继承自[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="bae28-143">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="bae28-144">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="bae28-144">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="bae28-145">响应</span><span class="sxs-lookup"><span data-stu-id="bae28-145">Response</span></span>
<span data-ttu-id="bae28-146">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="bae28-146">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bae28-147">示例</span><span class="sxs-lookup"><span data-stu-id="bae28-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="bae28-148">请求</span><span class="sxs-lookup"><span data-stu-id="bae28-148">Request</span></span>
<span data-ttu-id="bae28-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bae28-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="bae28-150">响应</span><span class="sxs-lookup"><span data-stu-id="bae28-150">Response</span></span>
<span data-ttu-id="bae28-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bae28-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




