---
title: 创建 managedEBookAssignment
description: 创建新的 managedEBookAssignment 对象。
ms.openlocfilehash: c471362f9f3cfddb9aa2cd3779ac66d28ec5d198
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27011194"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="5c6b8-103">创建 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="5c6b8-103">Create managedEBookAssignment</span></span>

> <span data-ttu-id="5c6b8-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="5c6b8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5c6b8-105">创建新的 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5c6b8-105">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5c6b8-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="5c6b8-106">Prerequisites</span></span>
<span data-ttu-id="5c6b8-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="5c6b8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5c6b8-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5c6b8-109">Permission type</span></span>|<span data-ttu-id="5c6b8-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="5c6b8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5c6b8-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5c6b8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="5c6b8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5c6b8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5c6b8-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5c6b8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5c6b8-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c6b8-114">Not supported.</span></span>|
|<span data-ttu-id="5c6b8-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5c6b8-115">Application</span></span>|<span data-ttu-id="5c6b8-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5c6b8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5c6b8-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5c6b8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="5c6b8-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="5c6b8-118">Request headers</span></span>
|<span data-ttu-id="5c6b8-119">标头</span><span class="sxs-lookup"><span data-stu-id="5c6b8-119">Header</span></span>|<span data-ttu-id="5c6b8-120">值</span><span class="sxs-lookup"><span data-stu-id="5c6b8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5c6b8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="5c6b8-121">Authorization</span></span>|<span data-ttu-id="5c6b8-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5c6b8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5c6b8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="5c6b8-123">Accept</span></span>|<span data-ttu-id="5c6b8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="5c6b8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5c6b8-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="5c6b8-125">Request body</span></span>
<span data-ttu-id="5c6b8-126">在请求正文中，提供 managedEBookAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5c6b8-126">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="5c6b8-127">下表显示创建 managedEBookAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="5c6b8-127">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="5c6b8-128">属性</span><span class="sxs-lookup"><span data-stu-id="5c6b8-128">Property</span></span>|<span data-ttu-id="5c6b8-129">类型</span><span class="sxs-lookup"><span data-stu-id="5c6b8-129">Type</span></span>|<span data-ttu-id="5c6b8-130">说明</span><span class="sxs-lookup"><span data-stu-id="5c6b8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c6b8-131">id</span><span class="sxs-lookup"><span data-stu-id="5c6b8-131">id</span></span>|<span data-ttu-id="5c6b8-132">String</span><span class="sxs-lookup"><span data-stu-id="5c6b8-132">String</span></span>|<span data-ttu-id="5c6b8-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="5c6b8-133">Key of the entity.</span></span>|
|<span data-ttu-id="5c6b8-134">target</span><span class="sxs-lookup"><span data-stu-id="5c6b8-134">target</span></span>|[<span data-ttu-id="5c6b8-135">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="5c6b8-135">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="5c6b8-136">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="5c6b8-136">The assignment target for eBook.</span></span>|
|<span data-ttu-id="5c6b8-137">installIntent</span><span class="sxs-lookup"><span data-stu-id="5c6b8-137">installIntent</span></span>|[<span data-ttu-id="5c6b8-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="5c6b8-138">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="5c6b8-139">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="5c6b8-139">The install intent for eBook.</span></span> <span data-ttu-id="5c6b8-140">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="5c6b8-140">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="5c6b8-141">响应</span><span class="sxs-lookup"><span data-stu-id="5c6b8-141">Response</span></span>
<span data-ttu-id="5c6b8-142">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5c6b8-142">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5c6b8-143">示例</span><span class="sxs-lookup"><span data-stu-id="5c6b8-143">Example</span></span>
### <a name="request"></a><span data-ttu-id="5c6b8-144">请求</span><span class="sxs-lookup"><span data-stu-id="5c6b8-144">Request</span></span>
<span data-ttu-id="5c6b8-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5c6b8-145">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="5c6b8-146">响应</span><span class="sxs-lookup"><span data-stu-id="5c6b8-146">Response</span></span>
<span data-ttu-id="5c6b8-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5c6b8-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



