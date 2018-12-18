---
title: 更新 iosVppEBookAssignment
description: 更新 iosVppEBookAssignment 对象的属性。
author: tfitzmac
ms.openlocfilehash: 8a4970b41cae2ab164a1164970d15d0a8afec344
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330532"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="a1e73-103">更新 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="a1e73-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="a1e73-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a1e73-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a1e73-105">更新 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a1e73-105">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a1e73-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="a1e73-106">Prerequisites</span></span>
<span data-ttu-id="a1e73-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a1e73-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a1e73-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a1e73-109">Permission type</span></span>|<span data-ttu-id="a1e73-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a1e73-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a1e73-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a1e73-111">Delegated (work or school account)</span></span>|<span data-ttu-id="a1e73-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a1e73-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a1e73-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a1e73-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a1e73-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1e73-114">Not supported.</span></span>|
|<span data-ttu-id="a1e73-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a1e73-115">Application</span></span>|<span data-ttu-id="a1e73-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a1e73-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a1e73-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a1e73-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="a1e73-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="a1e73-118">Request headers</span></span>
|<span data-ttu-id="a1e73-119">标头</span><span class="sxs-lookup"><span data-stu-id="a1e73-119">Header</span></span>|<span data-ttu-id="a1e73-120">值</span><span class="sxs-lookup"><span data-stu-id="a1e73-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a1e73-121">授权</span><span class="sxs-lookup"><span data-stu-id="a1e73-121">Authorization</span></span>|<span data-ttu-id="a1e73-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a1e73-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a1e73-123">Accept</span><span class="sxs-lookup"><span data-stu-id="a1e73-123">Accept</span></span>|<span data-ttu-id="a1e73-124">application/json</span><span class="sxs-lookup"><span data-stu-id="a1e73-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a1e73-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="a1e73-125">Request body</span></span>
<span data-ttu-id="a1e73-126">在请求正文中，提供 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a1e73-126">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="a1e73-127">下表显示创建 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a1e73-127">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="a1e73-128">属性</span><span class="sxs-lookup"><span data-stu-id="a1e73-128">Property</span></span>|<span data-ttu-id="a1e73-129">类型</span><span class="sxs-lookup"><span data-stu-id="a1e73-129">Type</span></span>|<span data-ttu-id="a1e73-130">说明</span><span class="sxs-lookup"><span data-stu-id="a1e73-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a1e73-131">id</span><span class="sxs-lookup"><span data-stu-id="a1e73-131">id</span></span>|<span data-ttu-id="a1e73-132">String</span><span class="sxs-lookup"><span data-stu-id="a1e73-132">String</span></span>|<span data-ttu-id="a1e73-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a1e73-133">Key of the entity.</span></span> <span data-ttu-id="a1e73-134">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a1e73-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="a1e73-135">target</span><span class="sxs-lookup"><span data-stu-id="a1e73-135">target</span></span>|[<span data-ttu-id="a1e73-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a1e73-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a1e73-137">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="a1e73-137">The assignment target for eBook.</span></span> <span data-ttu-id="a1e73-138">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a1e73-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="a1e73-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="a1e73-139">installIntent</span></span>|[<span data-ttu-id="a1e73-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="a1e73-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="a1e73-141">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="a1e73-141">The install intent for eBook.</span></span> <span data-ttu-id="a1e73-142">继承自[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="a1e73-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="a1e73-143">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="a1e73-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="a1e73-144">响应</span><span class="sxs-lookup"><span data-stu-id="a1e73-144">Response</span></span>
<span data-ttu-id="a1e73-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a1e73-145">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a1e73-146">示例</span><span class="sxs-lookup"><span data-stu-id="a1e73-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="a1e73-147">请求</span><span class="sxs-lookup"><span data-stu-id="a1e73-147">Request</span></span>
<span data-ttu-id="a1e73-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a1e73-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a1e73-149">响应</span><span class="sxs-lookup"><span data-stu-id="a1e73-149">Response</span></span>
<span data-ttu-id="a1e73-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a1e73-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



