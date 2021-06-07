---
title: 更新 managedEBookAssignment
description: 更新 managedEBookAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: c3078497aba9a9532d4ab911b78ea318d5168ce1
ms.sourcegitcommit: 13f474d3e71d32a5dfe2efebb351e3a1a5aa9685
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2021
ms.locfileid: "52756734"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="034af-103">更新 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="034af-103">Update managedEBookAssignment</span></span>

<span data-ttu-id="034af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="034af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="034af-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="034af-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="034af-106">更新 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="034af-106">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="034af-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="034af-107">Prerequisites</span></span>
<span data-ttu-id="034af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="034af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="034af-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="034af-110">Permission type</span></span>|<span data-ttu-id="034af-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="034af-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="034af-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="034af-112">Delegated (work or school account)</span></span>|<span data-ttu-id="034af-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="034af-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="034af-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="034af-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="034af-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="034af-115">Not supported.</span></span>|
|<span data-ttu-id="034af-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="034af-116">Application</span></span>|<span data-ttu-id="034af-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="034af-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="034af-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="034af-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="034af-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="034af-119">Request headers</span></span>
|<span data-ttu-id="034af-120">标头</span><span class="sxs-lookup"><span data-stu-id="034af-120">Header</span></span>|<span data-ttu-id="034af-121">值</span><span class="sxs-lookup"><span data-stu-id="034af-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="034af-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="034af-122">Authorization</span></span>|<span data-ttu-id="034af-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="034af-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="034af-124">接受</span><span class="sxs-lookup"><span data-stu-id="034af-124">Accept</span></span>|<span data-ttu-id="034af-125">application/json</span><span class="sxs-lookup"><span data-stu-id="034af-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="034af-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="034af-126">Request body</span></span>
<span data-ttu-id="034af-127">在请求正文中，提供 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="034af-127">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="034af-128">下表显示创建 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="034af-128">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="034af-129">属性</span><span class="sxs-lookup"><span data-stu-id="034af-129">Property</span></span>|<span data-ttu-id="034af-130">类型</span><span class="sxs-lookup"><span data-stu-id="034af-130">Type</span></span>|<span data-ttu-id="034af-131">说明</span><span class="sxs-lookup"><span data-stu-id="034af-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="034af-132">id</span><span class="sxs-lookup"><span data-stu-id="034af-132">id</span></span>|<span data-ttu-id="034af-133">String</span><span class="sxs-lookup"><span data-stu-id="034af-133">String</span></span>|<span data-ttu-id="034af-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="034af-134">Key of the entity.</span></span>|
|<span data-ttu-id="034af-135">target</span><span class="sxs-lookup"><span data-stu-id="034af-135">target</span></span>|[<span data-ttu-id="034af-136">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="034af-136">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="034af-137">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="034af-137">The assignment target for eBook.</span></span>|
|<span data-ttu-id="034af-138">installIntent</span><span class="sxs-lookup"><span data-stu-id="034af-138">installIntent</span></span>|[<span data-ttu-id="034af-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="034af-139">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="034af-140">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="034af-140">The install intent for eBook.</span></span> <span data-ttu-id="034af-141">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="034af-141">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="034af-142">响应</span><span class="sxs-lookup"><span data-stu-id="034af-142">Response</span></span>
<span data-ttu-id="034af-143">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="034af-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="034af-144">示例</span><span class="sxs-lookup"><span data-stu-id="034af-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="034af-145">请求</span><span class="sxs-lookup"><span data-stu-id="034af-145">Request</span></span>
<span data-ttu-id="034af-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="034af-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
Content-type: application/json
Content-length: 188

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "installIntent": "required"
}
```

### <a name="response"></a><span data-ttu-id="034af-147">响应</span><span class="sxs-lookup"><span data-stu-id="034af-147">Response</span></span>
<span data-ttu-id="034af-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="034af-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 237

{
  "@odata.type": "#microsoft.graph.managedEBookAssignment",
  "id": "ae8b0d27-0d27-ae8b-270d-8bae270d8bae",
  "target": {
    "@odata.type": "microsoft.graph.allLicensedUsersAssignmentTarget"
  },
  "installIntent": "required"
}
```




