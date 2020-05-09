---
title: 更新 managedEBookAssignment
description: 更新 managedEBookAssignment 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bde99a2577fbca953c9b582c238b428d9492b6d0
ms.sourcegitcommit: d961d83d2792328c9b64421325299e4b56d8dabd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/09/2020
ms.locfileid: "44174907"
---
# <a name="update-managedebookassignment"></a><span data-ttu-id="c3a59-103">更新 managedEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="c3a59-103">Update managedEBookAssignment</span></span>

<span data-ttu-id="c3a59-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c3a59-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c3a59-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c3a59-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c3a59-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c3a59-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c3a59-107">更新 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c3a59-107">Update the properties of a [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c3a59-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c3a59-108">Prerequisites</span></span>
<span data-ttu-id="c3a59-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c3a59-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c3a59-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c3a59-111">Permission type</span></span>|<span data-ttu-id="c3a59-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c3a59-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c3a59-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c3a59-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c3a59-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3a59-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c3a59-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c3a59-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c3a59-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c3a59-116">Not supported.</span></span>|
|<span data-ttu-id="c3a59-117">Application</span><span class="sxs-lookup"><span data-stu-id="c3a59-117">Application</span></span>|<span data-ttu-id="c3a59-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c3a59-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c3a59-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c3a59-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="c3a59-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c3a59-120">Request headers</span></span>
|<span data-ttu-id="c3a59-121">标头</span><span class="sxs-lookup"><span data-stu-id="c3a59-121">Header</span></span>|<span data-ttu-id="c3a59-122">值</span><span class="sxs-lookup"><span data-stu-id="c3a59-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c3a59-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c3a59-123">Authorization</span></span>|<span data-ttu-id="c3a59-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c3a59-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c3a59-125">接受</span><span class="sxs-lookup"><span data-stu-id="c3a59-125">Accept</span></span>|<span data-ttu-id="c3a59-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c3a59-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c3a59-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c3a59-127">Request body</span></span>
<span data-ttu-id="c3a59-128">在请求正文中，提供 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c3a59-128">In the request body, supply a JSON representation for the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object.</span></span>

<span data-ttu-id="c3a59-129">下表显示创建 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c3a59-129">The following table shows the properties that are required when you create the [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span>

|<span data-ttu-id="c3a59-130">属性</span><span class="sxs-lookup"><span data-stu-id="c3a59-130">Property</span></span>|<span data-ttu-id="c3a59-131">类型</span><span class="sxs-lookup"><span data-stu-id="c3a59-131">Type</span></span>|<span data-ttu-id="c3a59-132">说明</span><span class="sxs-lookup"><span data-stu-id="c3a59-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c3a59-133">id</span><span class="sxs-lookup"><span data-stu-id="c3a59-133">id</span></span>|<span data-ttu-id="c3a59-134">字符串</span><span class="sxs-lookup"><span data-stu-id="c3a59-134">String</span></span>|<span data-ttu-id="c3a59-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c3a59-135">Key of the entity.</span></span>|
|<span data-ttu-id="c3a59-136">target</span><span class="sxs-lookup"><span data-stu-id="c3a59-136">target</span></span>|[<span data-ttu-id="c3a59-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="c3a59-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="c3a59-138">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="c3a59-138">The assignment target for eBook.</span></span>|
|<span data-ttu-id="c3a59-139">installIntent</span><span class="sxs-lookup"><span data-stu-id="c3a59-139">installIntent</span></span>|[<span data-ttu-id="c3a59-140">installIntent</span><span class="sxs-lookup"><span data-stu-id="c3a59-140">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="c3a59-141">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="c3a59-141">The install intent for eBook.</span></span> <span data-ttu-id="c3a59-142">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="c3a59-142">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="c3a59-143">响应</span><span class="sxs-lookup"><span data-stu-id="c3a59-143">Response</span></span>
<span data-ttu-id="c3a59-144">如果成功，此方法将在响应正文中返回 `200 OK` 响应代码和更新的 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c3a59-144">If successful, this method returns a `200 OK` response code and an updated [managedEBookAssignment](../resources/intune-books-managedebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c3a59-145">示例</span><span class="sxs-lookup"><span data-stu-id="c3a59-145">Example</span></span>

### <a name="request"></a><span data-ttu-id="c3a59-146">请求</span><span class="sxs-lookup"><span data-stu-id="c3a59-146">Request</span></span>
<span data-ttu-id="c3a59-147">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c3a59-147">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/assignments/{managedEBookAssignmentId}
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

### <a name="response"></a><span data-ttu-id="c3a59-148">响应</span><span class="sxs-lookup"><span data-stu-id="c3a59-148">Response</span></span>
<span data-ttu-id="c3a59-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c3a59-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



