---
title: 创建 iosVppEBookAssignment
description: 创建新的 iosVppEBookAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b45e4a986306fbecf039abee29c2a6939f9b4e69
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32577124"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="7ba47-103">创建 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="7ba47-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="7ba47-104">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="7ba47-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="7ba47-105">创建新的 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7ba47-105">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="7ba47-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="7ba47-106">Prerequisites</span></span>
<span data-ttu-id="7ba47-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7ba47-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7ba47-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="7ba47-109">Permission type</span></span>|<span data-ttu-id="7ba47-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="7ba47-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7ba47-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7ba47-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7ba47-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7ba47-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7ba47-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7ba47-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7ba47-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ba47-114">Not supported.</span></span>|
|<span data-ttu-id="7ba47-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="7ba47-115">Application</span></span>|<span data-ttu-id="7ba47-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7ba47-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7ba47-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7ba47-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="7ba47-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="7ba47-118">Request headers</span></span>
|<span data-ttu-id="7ba47-119">标头</span><span class="sxs-lookup"><span data-stu-id="7ba47-119">Header</span></span>|<span data-ttu-id="7ba47-120">值</span><span class="sxs-lookup"><span data-stu-id="7ba47-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7ba47-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7ba47-121">Authorization</span></span>|<span data-ttu-id="7ba47-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="7ba47-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7ba47-123">接受</span><span class="sxs-lookup"><span data-stu-id="7ba47-123">Accept</span></span>|<span data-ttu-id="7ba47-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7ba47-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7ba47-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7ba47-125">Request body</span></span>
<span data-ttu-id="7ba47-126">在请求正文中，提供 iosVppEBookAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7ba47-126">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="7ba47-127">下表显示创建 iosVppEBookAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7ba47-127">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="7ba47-128">属性</span><span class="sxs-lookup"><span data-stu-id="7ba47-128">Property</span></span>|<span data-ttu-id="7ba47-129">类型</span><span class="sxs-lookup"><span data-stu-id="7ba47-129">Type</span></span>|<span data-ttu-id="7ba47-130">说明</span><span class="sxs-lookup"><span data-stu-id="7ba47-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7ba47-131">id</span><span class="sxs-lookup"><span data-stu-id="7ba47-131">id</span></span>|<span data-ttu-id="7ba47-132">String</span><span class="sxs-lookup"><span data-stu-id="7ba47-132">String</span></span>|<span data-ttu-id="7ba47-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="7ba47-133">Key of the entity.</span></span> <span data-ttu-id="7ba47-134">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7ba47-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="7ba47-135">target</span><span class="sxs-lookup"><span data-stu-id="7ba47-135">target</span></span>|[<span data-ttu-id="7ba47-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="7ba47-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="7ba47-137">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="7ba47-137">The assignment target for eBook.</span></span> <span data-ttu-id="7ba47-138">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="7ba47-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="7ba47-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="7ba47-139">installIntent</span></span>|[<span data-ttu-id="7ba47-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="7ba47-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="7ba47-141">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="7ba47-141">The install intent for eBook.</span></span> <span data-ttu-id="7ba47-142">继承自[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="7ba47-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="7ba47-143">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="7ba47-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="7ba47-144">响应</span><span class="sxs-lookup"><span data-stu-id="7ba47-144">Response</span></span>
<span data-ttu-id="7ba47-145">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7ba47-145">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7ba47-146">示例</span><span class="sxs-lookup"><span data-stu-id="7ba47-146">Example</span></span>

### <a name="request"></a><span data-ttu-id="7ba47-147">请求</span><span class="sxs-lookup"><span data-stu-id="7ba47-147">Request</span></span>
<span data-ttu-id="7ba47-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7ba47-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="7ba47-149">响应</span><span class="sxs-lookup"><span data-stu-id="7ba47-149">Response</span></span>
<span data-ttu-id="7ba47-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7ba47-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



