---
title: 更新 iosVppEBookAssignment
description: 更新 iosVppEBookAssignment 对象的属性。
ms.openlocfilehash: 2eee8125fe9fa6141b84f6d7dbdd74190ddeca6e
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27008311"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="861cc-103">更新 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="861cc-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="861cc-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="861cc-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="861cc-105">更新 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="861cc-105">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="861cc-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="861cc-106">Prerequisites</span></span>
<span data-ttu-id="861cc-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="861cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="861cc-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="861cc-109">Permission type</span></span>|<span data-ttu-id="861cc-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="861cc-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="861cc-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="861cc-111">Delegated (work or school account)</span></span>|<span data-ttu-id="861cc-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="861cc-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="861cc-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="861cc-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="861cc-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="861cc-114">Not supported.</span></span>|
|<span data-ttu-id="861cc-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="861cc-115">Application</span></span>|<span data-ttu-id="861cc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="861cc-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="861cc-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="861cc-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="861cc-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="861cc-118">Request headers</span></span>
|<span data-ttu-id="861cc-119">标头</span><span class="sxs-lookup"><span data-stu-id="861cc-119">Header</span></span>|<span data-ttu-id="861cc-120">值</span><span class="sxs-lookup"><span data-stu-id="861cc-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="861cc-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="861cc-121">Authorization</span></span>|<span data-ttu-id="861cc-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="861cc-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="861cc-123">Accept</span><span class="sxs-lookup"><span data-stu-id="861cc-123">Accept</span></span>|<span data-ttu-id="861cc-124">application/json</span><span class="sxs-lookup"><span data-stu-id="861cc-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="861cc-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="861cc-125">Request body</span></span>
<span data-ttu-id="861cc-126">在请求正文中，提供 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="861cc-126">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="861cc-127">下表显示创建 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="861cc-127">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="861cc-128">属性</span><span class="sxs-lookup"><span data-stu-id="861cc-128">Property</span></span>|<span data-ttu-id="861cc-129">类型</span><span class="sxs-lookup"><span data-stu-id="861cc-129">Type</span></span>|<span data-ttu-id="861cc-130">说明</span><span class="sxs-lookup"><span data-stu-id="861cc-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="861cc-131">id</span><span class="sxs-lookup"><span data-stu-id="861cc-131">id</span></span>|<span data-ttu-id="861cc-132">String</span><span class="sxs-lookup"><span data-stu-id="861cc-132">String</span></span>|<span data-ttu-id="861cc-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="861cc-133">Key of the entity.</span></span> <span data-ttu-id="861cc-134">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="861cc-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="861cc-135">target</span><span class="sxs-lookup"><span data-stu-id="861cc-135">target</span></span>|[<span data-ttu-id="861cc-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="861cc-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="861cc-137">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="861cc-137">The assignment target for eBook.</span></span> <span data-ttu-id="861cc-138">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="861cc-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="861cc-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="861cc-139">installIntent</span></span>|[<span data-ttu-id="861cc-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="861cc-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="861cc-141">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="861cc-141">The install intent for eBook.</span></span> <span data-ttu-id="861cc-142">继承自[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="861cc-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="861cc-143">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="861cc-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="861cc-144">响应</span><span class="sxs-lookup"><span data-stu-id="861cc-144">Response</span></span>
<span data-ttu-id="861cc-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="861cc-145">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="861cc-146">示例</span><span class="sxs-lookup"><span data-stu-id="861cc-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="861cc-147">请求</span><span class="sxs-lookup"><span data-stu-id="861cc-147">Request</span></span>
<span data-ttu-id="861cc-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="861cc-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="861cc-149">响应</span><span class="sxs-lookup"><span data-stu-id="861cc-149">Response</span></span>
<span data-ttu-id="861cc-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="861cc-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



