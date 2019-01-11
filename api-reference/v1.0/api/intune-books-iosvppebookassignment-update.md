---
title: 更新 iosVppEBookAssignment
description: 更新 iosVppEBookAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 8b1d4bec696b247e1e234e4329b60af4315e3cc4
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876487"
---
# <a name="update-iosvppebookassignment"></a><span data-ttu-id="d9c26-103">更新 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="d9c26-103">Update iosVppEBookAssignment</span></span>

> <span data-ttu-id="d9c26-104">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="d9c26-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d9c26-105">更新 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d9c26-105">Update the properties of a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d9c26-106">先决条件</span><span class="sxs-lookup"><span data-stu-id="d9c26-106">Prerequisites</span></span>
<span data-ttu-id="d9c26-p101">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="d9c26-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d9c26-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="d9c26-109">Permission type</span></span>|<span data-ttu-id="d9c26-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d9c26-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d9c26-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d9c26-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d9c26-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d9c26-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d9c26-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d9c26-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d9c26-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9c26-114">Not supported.</span></span>|
|<span data-ttu-id="d9c26-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="d9c26-115">Application</span></span>|<span data-ttu-id="d9c26-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d9c26-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d9c26-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d9c26-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="d9c26-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="d9c26-118">Request headers</span></span>
|<span data-ttu-id="d9c26-119">标头</span><span class="sxs-lookup"><span data-stu-id="d9c26-119">Header</span></span>|<span data-ttu-id="d9c26-120">值</span><span class="sxs-lookup"><span data-stu-id="d9c26-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d9c26-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d9c26-121">Authorization</span></span>|<span data-ttu-id="d9c26-122">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d9c26-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d9c26-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d9c26-123">Accept</span></span>|<span data-ttu-id="d9c26-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d9c26-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d9c26-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="d9c26-125">Request body</span></span>
<span data-ttu-id="d9c26-126">在请求正文中，提供 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9c26-126">In the request body, supply a JSON representation for the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

<span data-ttu-id="d9c26-127">下表显示创建 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d9c26-127">The following table shows the properties that are required when you create the [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md).</span></span>

|<span data-ttu-id="d9c26-128">属性</span><span class="sxs-lookup"><span data-stu-id="d9c26-128">Property</span></span>|<span data-ttu-id="d9c26-129">类型</span><span class="sxs-lookup"><span data-stu-id="d9c26-129">Type</span></span>|<span data-ttu-id="d9c26-130">说明</span><span class="sxs-lookup"><span data-stu-id="d9c26-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d9c26-131">id</span><span class="sxs-lookup"><span data-stu-id="d9c26-131">id</span></span>|<span data-ttu-id="d9c26-132">String</span><span class="sxs-lookup"><span data-stu-id="d9c26-132">String</span></span>|<span data-ttu-id="d9c26-133">实体的键。</span><span class="sxs-lookup"><span data-stu-id="d9c26-133">Key of the entity.</span></span> <span data-ttu-id="d9c26-134">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d9c26-134">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="d9c26-135">target</span><span class="sxs-lookup"><span data-stu-id="d9c26-135">target</span></span>|[<span data-ttu-id="d9c26-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="d9c26-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="d9c26-137">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="d9c26-137">The assignment target for eBook.</span></span> <span data-ttu-id="d9c26-138">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="d9c26-138">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="d9c26-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="d9c26-139">installIntent</span></span>|[<span data-ttu-id="d9c26-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="d9c26-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="d9c26-141">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="d9c26-141">The install intent for eBook.</span></span> <span data-ttu-id="d9c26-142">继承自[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="d9c26-142">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="d9c26-143">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="d9c26-143">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="d9c26-144">响应</span><span class="sxs-lookup"><span data-stu-id="d9c26-144">Response</span></span>
<span data-ttu-id="d9c26-145">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d9c26-145">If successful, this method returns a `200 OK` response code and an updated [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d9c26-146">示例</span><span class="sxs-lookup"><span data-stu-id="d9c26-146">Example</span></span>
### <a name="request"></a><span data-ttu-id="d9c26-147">请求</span><span class="sxs-lookup"><span data-stu-id="d9c26-147">Request</span></span>
<span data-ttu-id="d9c26-148">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d9c26-148">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d9c26-149">响应</span><span class="sxs-lookup"><span data-stu-id="d9c26-149">Response</span></span>
<span data-ttu-id="d9c26-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d9c26-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



