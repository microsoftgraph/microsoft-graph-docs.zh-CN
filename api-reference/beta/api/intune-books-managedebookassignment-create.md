---
title: 创建 managedEBookAssignment
description: 创建新的 managedEBookAssignment 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7ebb4f0bede59a636085c813fa49533015802b6a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35959192"
---
# <a name="create-managedebookassignment"></a><span data-ttu-id="509d2-103">创建 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="509d2-103">Create managedEBookAssignment</span></span>

> <span data-ttu-id="509d2-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="509d2-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="509d2-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="509d2-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="509d2-106">创建新的 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="509d2-106">Create a new [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="509d2-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="509d2-107">Prerequisites</span></span>
<span data-ttu-id="509d2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="509d2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="509d2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="509d2-110">Permission type</span></span>|<span data-ttu-id="509d2-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="509d2-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="509d2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="509d2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="509d2-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="509d2-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="509d2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="509d2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="509d2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="509d2-115">Not supported.</span></span>|
|<span data-ttu-id="509d2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="509d2-116">Application</span></span>|<span data-ttu-id="509d2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="509d2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="509d2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="509d2-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="509d2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="509d2-119">Request headers</span></span>
|<span data-ttu-id="509d2-120">标头</span><span class="sxs-lookup"><span data-stu-id="509d2-120">Header</span></span>|<span data-ttu-id="509d2-121">值</span><span class="sxs-lookup"><span data-stu-id="509d2-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="509d2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="509d2-122">Authorization</span></span>|<span data-ttu-id="509d2-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="509d2-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="509d2-124">接受</span><span class="sxs-lookup"><span data-stu-id="509d2-124">Accept</span></span>|<span data-ttu-id="509d2-125">application/json</span><span class="sxs-lookup"><span data-stu-id="509d2-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="509d2-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="509d2-126">Request body</span></span>
<span data-ttu-id="509d2-127">在请求正文中，提供 managedEBookAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="509d2-127">In the request body, supply a JSON representation for the managedEBookAssignment object.</span></span>

<span data-ttu-id="509d2-128">下表显示创建 managedEBookAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="509d2-128">The following table shows the properties that are required when you create the managedEBookAssignment.</span></span>

|<span data-ttu-id="509d2-129">属性</span><span class="sxs-lookup"><span data-stu-id="509d2-129">Property</span></span>|<span data-ttu-id="509d2-130">类型</span><span class="sxs-lookup"><span data-stu-id="509d2-130">Type</span></span>|<span data-ttu-id="509d2-131">说明</span><span class="sxs-lookup"><span data-stu-id="509d2-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="509d2-132">id</span><span class="sxs-lookup"><span data-stu-id="509d2-132">id</span></span>|<span data-ttu-id="509d2-133">String</span><span class="sxs-lookup"><span data-stu-id="509d2-133">String</span></span>|<span data-ttu-id="509d2-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="509d2-134">Key of the entity.</span></span>|
|<span data-ttu-id="509d2-135">target</span><span class="sxs-lookup"><span data-stu-id="509d2-135">target</span></span>|[<span data-ttu-id="509d2-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="509d2-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="509d2-137">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="509d2-137">The assignment target for eBook.</span></span>|
|<span data-ttu-id="509d2-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="509d2-138">installIntent</span></span>|[<span data-ttu-id="509d2-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="509d2-139">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="509d2-140">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="509d2-140">The install intent for eBook.</span></span> <span data-ttu-id="509d2-141">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="509d2-141">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="509d2-142">响应</span><span class="sxs-lookup"><span data-stu-id="509d2-142">Response</span></span>
<span data-ttu-id="509d2-143">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="509d2-143">If successful, this method returns a `201 Created` response code and a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="509d2-144">示例</span><span class="sxs-lookup"><span data-stu-id="509d2-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="509d2-145">请求</span><span class="sxs-lookup"><span data-stu-id="509d2-145">Request</span></span>
<span data-ttu-id="509d2-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="509d2-146">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="509d2-147">响应</span><span class="sxs-lookup"><span data-stu-id="509d2-147">Response</span></span>
<span data-ttu-id="509d2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="509d2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





