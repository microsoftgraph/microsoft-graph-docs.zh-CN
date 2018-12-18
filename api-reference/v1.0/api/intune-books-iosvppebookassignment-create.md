---
title: 创建 iosVppEBookAssignment
description: 创建新的 iosVppEBookAssignment 对象。
author: tfitzmac
ms.openlocfilehash: b9a3bf5ba8c3eb0c8d2f92e66361ce7afa875c4d
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27334403"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="f9c88-103">创建 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="f9c88-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="f9c88-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="f9c88-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f9c88-105">创建新的 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f9c88-105">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f9c88-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="f9c88-106">Prerequisites</span></span>
<span data-ttu-id="f9c88-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="f9c88-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9c88-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f9c88-109">Permission type</span></span>|<span data-ttu-id="f9c88-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f9c88-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9c88-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f9c88-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f9c88-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9c88-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f9c88-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f9c88-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9c88-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9c88-114">Not supported.</span></span>|
|<span data-ttu-id="f9c88-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f9c88-115">Application</span></span>|<span data-ttu-id="f9c88-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f9c88-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9c88-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f9c88-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="f9c88-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f9c88-118">Request headers</span></span>
|<span data-ttu-id="f9c88-119">标头</span><span class="sxs-lookup"><span data-stu-id="f9c88-119">Header</span></span>|<span data-ttu-id="f9c88-120">值</span><span class="sxs-lookup"><span data-stu-id="f9c88-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9c88-121">授权</span><span class="sxs-lookup"><span data-stu-id="f9c88-121">Authorization</span></span>|<span data-ttu-id="f9c88-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f9c88-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9c88-123">Accept</span><span class="sxs-lookup"><span data-stu-id="f9c88-123">Accept</span></span>|<span data-ttu-id="f9c88-124">application/json</span><span class="sxs-lookup"><span data-stu-id="f9c88-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9c88-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="f9c88-125">Request body</span></span>
<span data-ttu-id="f9c88-126">在请求正文中，提供 iosVppEBookAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9c88-126">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="f9c88-127">下表显示创建 iosVppEBookAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f9c88-127">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="f9c88-128">属性</span><span class="sxs-lookup"><span data-stu-id="f9c88-128">Property</span></span>|<span data-ttu-id="f9c88-129">类型</span><span class="sxs-lookup"><span data-stu-id="f9c88-129">Type</span></span>|<span data-ttu-id="f9c88-130">说明</span><span class="sxs-lookup"><span data-stu-id="f9c88-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9c88-131">id</span><span class="sxs-lookup"><span data-stu-id="f9c88-131">id</span></span>|<span data-ttu-id="f9c88-132">String</span><span class="sxs-lookup"><span data-stu-id="f9c88-132">String</span></span>|<span data-ttu-id="f9c88-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="f9c88-133">Key of the entity.</span></span> <span data-ttu-id="f9c88-134">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f9c88-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="f9c88-135">target</span><span class="sxs-lookup"><span data-stu-id="f9c88-135">target</span></span>|[<span data-ttu-id="f9c88-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="f9c88-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="f9c88-137">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="f9c88-137">The assignment target for eBook.</span></span> <span data-ttu-id="f9c88-138">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="f9c88-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="f9c88-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="f9c88-139">installIntent</span></span>|[<span data-ttu-id="f9c88-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="f9c88-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="f9c88-141">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="f9c88-141">The install intent for eBook.</span></span> <span data-ttu-id="f9c88-142">继承自[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="f9c88-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="f9c88-143">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="f9c88-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="f9c88-144">响应</span><span class="sxs-lookup"><span data-stu-id="f9c88-144">Response</span></span>
<span data-ttu-id="f9c88-145">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f9c88-145">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9c88-146">示例</span><span class="sxs-lookup"><span data-stu-id="f9c88-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="f9c88-147">请求</span><span class="sxs-lookup"><span data-stu-id="f9c88-147">Request</span></span>
<span data-ttu-id="f9c88-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f9c88-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f9c88-149">响应</span><span class="sxs-lookup"><span data-stu-id="f9c88-149">Response</span></span>
<span data-ttu-id="f9c88-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f9c88-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



