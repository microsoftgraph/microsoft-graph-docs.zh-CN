---
title: 创建 iosVppEBookAssignment
description: 创建新的 iosVppEBookAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: bf38da365d8ae09f478f1209b4174985ba92b1f6
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30968831"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="14c77-103">创建 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="14c77-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="14c77-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="14c77-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="14c77-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="14c77-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14c77-106">创建新的 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14c77-106">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14c77-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="14c77-107">Prerequisites</span></span>
<span data-ttu-id="14c77-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="14c77-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="14c77-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="14c77-110">Permission type</span></span>|<span data-ttu-id="14c77-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="14c77-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14c77-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="14c77-112">Delegated (work or school account)</span></span>|<span data-ttu-id="14c77-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14c77-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="14c77-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="14c77-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14c77-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="14c77-115">Not supported.</span></span>|
|<span data-ttu-id="14c77-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="14c77-116">Application</span></span>|<span data-ttu-id="14c77-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="14c77-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14c77-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="14c77-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="14c77-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="14c77-119">Request headers</span></span>
|<span data-ttu-id="14c77-120">标头</span><span class="sxs-lookup"><span data-stu-id="14c77-120">Header</span></span>|<span data-ttu-id="14c77-121">值</span><span class="sxs-lookup"><span data-stu-id="14c77-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14c77-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="14c77-122">Authorization</span></span>|<span data-ttu-id="14c77-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="14c77-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14c77-124">接受</span><span class="sxs-lookup"><span data-stu-id="14c77-124">Accept</span></span>|<span data-ttu-id="14c77-125">application/json</span><span class="sxs-lookup"><span data-stu-id="14c77-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14c77-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="14c77-126">Request body</span></span>
<span data-ttu-id="14c77-127">在请求正文中，提供 iosVppEBookAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="14c77-127">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="14c77-128">下表显示创建 iosVppEBookAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="14c77-128">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="14c77-129">属性</span><span class="sxs-lookup"><span data-stu-id="14c77-129">Property</span></span>|<span data-ttu-id="14c77-130">类型</span><span class="sxs-lookup"><span data-stu-id="14c77-130">Type</span></span>|<span data-ttu-id="14c77-131">说明</span><span class="sxs-lookup"><span data-stu-id="14c77-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14c77-132">id</span><span class="sxs-lookup"><span data-stu-id="14c77-132">id</span></span>|<span data-ttu-id="14c77-133">String</span><span class="sxs-lookup"><span data-stu-id="14c77-133">String</span></span>|<span data-ttu-id="14c77-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="14c77-134">Key of the entity.</span></span> <span data-ttu-id="14c77-135">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="14c77-135">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="14c77-136">target</span><span class="sxs-lookup"><span data-stu-id="14c77-136">target</span></span>|[<span data-ttu-id="14c77-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="14c77-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="14c77-138">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="14c77-138">The assignment target for eBook.</span></span> <span data-ttu-id="14c77-139">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="14c77-139">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="14c77-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="14c77-140">installIntent</span></span>|[<span data-ttu-id="14c77-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="14c77-141">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="14c77-142">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="14c77-142">The install intent for eBook.</span></span> <span data-ttu-id="14c77-143">继承自[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="14c77-143">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="14c77-144">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="14c77-144">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="14c77-145">响应</span><span class="sxs-lookup"><span data-stu-id="14c77-145">Response</span></span>
<span data-ttu-id="14c77-146">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="14c77-146">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14c77-147">示例</span><span class="sxs-lookup"><span data-stu-id="14c77-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="14c77-148">请求</span><span class="sxs-lookup"><span data-stu-id="14c77-148">Request</span></span>
<span data-ttu-id="14c77-149">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="14c77-149">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments
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

### <a name="response"></a><span data-ttu-id="14c77-150">响应</span><span class="sxs-lookup"><span data-stu-id="14c77-150">Response</span></span>
<span data-ttu-id="14c77-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="14c77-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




