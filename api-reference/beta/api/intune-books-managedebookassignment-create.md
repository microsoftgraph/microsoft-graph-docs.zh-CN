---
title: 创建 managedEBookAssignment
description: 创建新的 managedEBookAssignment 对象。
ms.openlocfilehash: 74e65f386d4699010924e9ac616b479f14464f66
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041634"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="1f729-103">创建 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="1f729-103">Create managedEBookAssignment</span></span>

> <span data-ttu-id="1f729-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1f729-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1f729-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1f729-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1f729-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="1f729-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="1f729-107">创建新的 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1f729-107">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="1f729-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="1f729-108">Prerequisites</span></span>
<span data-ttu-id="1f729-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="1f729-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1f729-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="1f729-111">Permission type</span></span>|<span data-ttu-id="1f729-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="1f729-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1f729-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1f729-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1f729-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1f729-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1f729-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1f729-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1f729-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f729-116">Not supported.</span></span>|
|<span data-ttu-id="1f729-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1f729-117">Application</span></span>|<span data-ttu-id="1f729-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1f729-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1f729-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1f729-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="1f729-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1f729-120">Request headers</span></span>
|<span data-ttu-id="1f729-121">标头</span><span class="sxs-lookup"><span data-stu-id="1f729-121">Header</span></span>|<span data-ttu-id="1f729-122">值</span><span class="sxs-lookup"><span data-stu-id="1f729-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1f729-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1f729-123">Authorization</span></span>|<span data-ttu-id="1f729-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="1f729-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1f729-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1f729-125">Accept</span></span>|<span data-ttu-id="1f729-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1f729-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1f729-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="1f729-127">Request body</span></span>
<span data-ttu-id="1f729-128">在请求正文中，提供 managedEBookAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1f729-128">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="1f729-129">下表显示创建 managedEBookAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1f729-129">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="1f729-130">属性</span><span class="sxs-lookup"><span data-stu-id="1f729-130">Property</span></span>|<span data-ttu-id="1f729-131">类型</span><span class="sxs-lookup"><span data-stu-id="1f729-131">Type</span></span>|<span data-ttu-id="1f729-132">说明</span><span class="sxs-lookup"><span data-stu-id="1f729-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1f729-133">id</span><span class="sxs-lookup"><span data-stu-id="1f729-133">id</span></span>|<span data-ttu-id="1f729-134">String</span><span class="sxs-lookup"><span data-stu-id="1f729-134">String</span></span>|<span data-ttu-id="1f729-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="1f729-135">Key of the entity.</span></span>|
|<span data-ttu-id="1f729-136">target</span><span class="sxs-lookup"><span data-stu-id="1f729-136">target</span></span>|[<span data-ttu-id="1f729-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="1f729-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="1f729-138">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="1f729-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="1f729-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="1f729-139">installIntent</span></span>|[<span data-ttu-id="1f729-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="1f729-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="1f729-141">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="1f729-141">The install intent for eBook.</span></span> <span data-ttu-id="1f729-142">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="1f729-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="1f729-143">响应</span><span class="sxs-lookup"><span data-stu-id="1f729-143">Response</span></span>
<span data-ttu-id="1f729-144">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1f729-144">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1f729-145">示例</span><span class="sxs-lookup"><span data-stu-id="1f729-145">Example</span></span>
### <a name="request"></a><span data-ttu-id="1f729-146">请求</span><span class="sxs-lookup"><span data-stu-id="1f729-146">Request</span></span>
<span data-ttu-id="1f729-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1f729-147">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="1f729-148">响应</span><span class="sxs-lookup"><span data-stu-id="1f729-148">Response</span></span>
<span data-ttu-id="1f729-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="1f729-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





