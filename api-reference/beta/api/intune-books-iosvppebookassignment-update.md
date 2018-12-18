---
title: 更新 iosVppEBookAssignment
description: 更新 iosVppEBookAssignment 对象的属性。
author: tfitzmac
ms.openlocfilehash: 537c2ef5838dc68881f3de693a6591570219ece4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27338148"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="cae25-103">更新 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="cae25-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="cae25-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="cae25-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="cae25-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="cae25-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="cae25-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="cae25-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="cae25-107">更新 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cae25-107">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="cae25-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="cae25-108">Prerequisites</span></span>
<span data-ttu-id="cae25-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="cae25-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cae25-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="cae25-111">Permission type</span></span>|<span data-ttu-id="cae25-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cae25-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cae25-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cae25-113">Delegated (work or school account)</span></span>|<span data-ttu-id="cae25-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cae25-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="cae25-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cae25-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cae25-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="cae25-116">Not supported.</span></span>|
|<span data-ttu-id="cae25-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="cae25-117">Application</span></span>|<span data-ttu-id="cae25-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="cae25-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cae25-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cae25-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="cae25-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="cae25-120">Request headers</span></span>
|<span data-ttu-id="cae25-121">标头</span><span class="sxs-lookup"><span data-stu-id="cae25-121">Header</span></span>|<span data-ttu-id="cae25-122">值</span><span class="sxs-lookup"><span data-stu-id="cae25-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="cae25-123">授权</span><span class="sxs-lookup"><span data-stu-id="cae25-123">Authorization</span></span>|<span data-ttu-id="cae25-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="cae25-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="cae25-125">Accept</span><span class="sxs-lookup"><span data-stu-id="cae25-125">Accept</span></span>|<span data-ttu-id="cae25-126">application/json</span><span class="sxs-lookup"><span data-stu-id="cae25-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="cae25-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="cae25-127">Request body</span></span>
<span data-ttu-id="cae25-128">在请求正文中，提供 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cae25-128">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="cae25-129">下表显示创建 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cae25-129">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="cae25-130">属性</span><span class="sxs-lookup"><span data-stu-id="cae25-130">Property</span></span>|<span data-ttu-id="cae25-131">类型</span><span class="sxs-lookup"><span data-stu-id="cae25-131">Type</span></span>|<span data-ttu-id="cae25-132">说明</span><span class="sxs-lookup"><span data-stu-id="cae25-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cae25-133">id</span><span class="sxs-lookup"><span data-stu-id="cae25-133">id</span></span>|<span data-ttu-id="cae25-134">String</span><span class="sxs-lookup"><span data-stu-id="cae25-134">String</span></span>|<span data-ttu-id="cae25-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="cae25-135">Key of the entity.</span></span> <span data-ttu-id="cae25-136">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cae25-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="cae25-137">target</span><span class="sxs-lookup"><span data-stu-id="cae25-137">target</span></span>|[<span data-ttu-id="cae25-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="cae25-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="cae25-139">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="cae25-139">The assignment target for eBook.</span></span> <span data-ttu-id="cae25-140">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="cae25-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="cae25-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="cae25-141">installIntent</span></span>|[<span data-ttu-id="cae25-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="cae25-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="cae25-143">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="cae25-143">The install intent for eBook.</span></span> <span data-ttu-id="cae25-144">继承自[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="cae25-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="cae25-145">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="cae25-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="cae25-146">响应</span><span class="sxs-lookup"><span data-stu-id="cae25-146">Response</span></span>
<span data-ttu-id="cae25-147">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cae25-147">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="cae25-148">示例</span><span class="sxs-lookup"><span data-stu-id="cae25-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="cae25-149">请求</span><span class="sxs-lookup"><span data-stu-id="cae25-149">Request</span></span>
<span data-ttu-id="cae25-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="cae25-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 133

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="cae25-151">响应</span><span class="sxs-lookup"><span data-stu-id="cae25-151">Response</span></span>
<span data-ttu-id="cae25-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="cae25-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





