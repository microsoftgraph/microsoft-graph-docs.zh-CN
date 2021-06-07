---
title: 创建 iosVppEBookAssignment
description: 创建新的 iosVppEBookAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 38014d5ad851f44555dd637f62ae4923c12ee4bb
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52758439"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="07830-103">创建 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="07830-103">Create iosVppEBookAssignment</span></span>

<span data-ttu-id="07830-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="07830-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="07830-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="07830-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="07830-106">创建新的 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="07830-106">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="07830-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="07830-107">Prerequisites</span></span>
<span data-ttu-id="07830-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="07830-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="07830-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="07830-110">Permission type</span></span>|<span data-ttu-id="07830-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="07830-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="07830-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="07830-112">Delegated (work or school account)</span></span>|<span data-ttu-id="07830-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07830-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="07830-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="07830-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="07830-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="07830-115">Not supported.</span></span>|
|<span data-ttu-id="07830-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="07830-116">Application</span></span>|<span data-ttu-id="07830-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="07830-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="07830-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="07830-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="07830-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="07830-119">Request headers</span></span>
|<span data-ttu-id="07830-120">标头</span><span class="sxs-lookup"><span data-stu-id="07830-120">Header</span></span>|<span data-ttu-id="07830-121">值</span><span class="sxs-lookup"><span data-stu-id="07830-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="07830-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="07830-122">Authorization</span></span>|<span data-ttu-id="07830-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="07830-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="07830-124">接受</span><span class="sxs-lookup"><span data-stu-id="07830-124">Accept</span></span>|<span data-ttu-id="07830-125">application/json</span><span class="sxs-lookup"><span data-stu-id="07830-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="07830-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="07830-126">Request body</span></span>
<span data-ttu-id="07830-127">在请求正文中，提供 iosVppEBookAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07830-127">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="07830-128">下表显示创建 iosVppEBookAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="07830-128">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="07830-129">属性</span><span class="sxs-lookup"><span data-stu-id="07830-129">Property</span></span>|<span data-ttu-id="07830-130">类型</span><span class="sxs-lookup"><span data-stu-id="07830-130">Type</span></span>|<span data-ttu-id="07830-131">说明</span><span class="sxs-lookup"><span data-stu-id="07830-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="07830-132">id</span><span class="sxs-lookup"><span data-stu-id="07830-132">id</span></span>|<span data-ttu-id="07830-133">String</span><span class="sxs-lookup"><span data-stu-id="07830-133">String</span></span>|<span data-ttu-id="07830-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="07830-134">Key of the entity.</span></span> <span data-ttu-id="07830-135">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="07830-135">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="07830-136">target</span><span class="sxs-lookup"><span data-stu-id="07830-136">target</span></span>|[<span data-ttu-id="07830-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="07830-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="07830-138">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="07830-138">The assignment target for eBook.</span></span> <span data-ttu-id="07830-139">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="07830-139">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="07830-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="07830-140">installIntent</span></span>|[<span data-ttu-id="07830-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="07830-141">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="07830-142">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="07830-142">The install intent for eBook.</span></span> <span data-ttu-id="07830-143">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="07830-143">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="07830-144">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="07830-144">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="07830-145">响应</span><span class="sxs-lookup"><span data-stu-id="07830-145">Response</span></span>
<span data-ttu-id="07830-146">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="07830-146">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="07830-147">示例</span><span class="sxs-lookup"><span data-stu-id="07830-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="07830-148">请求</span><span class="sxs-lookup"><span data-stu-id="07830-148">Request</span></span>
<span data-ttu-id="07830-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="07830-149">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="07830-150">响应</span><span class="sxs-lookup"><span data-stu-id="07830-150">Response</span></span>
<span data-ttu-id="07830-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="07830-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




