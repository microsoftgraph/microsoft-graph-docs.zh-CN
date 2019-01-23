---
title: 创建 iosVppEBookAssignment
description: 创建新的 iosVppEBookAssignment 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3cfebd4f1b61ae7cfc3c4a92d2c3415ce18e4cab
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29424502"
---
# <a name="create-iosvppebookassignment"></a><span data-ttu-id="a33c0-103">创建 iosVppEBookAssignment</span><span class="sxs-lookup"><span data-stu-id="a33c0-103">Create iosVppEBookAssignment</span></span>

> <span data-ttu-id="a33c0-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="a33c0-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a33c0-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a33c0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a33c0-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a33c0-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a33c0-107">创建新的 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a33c0-107">Create a new [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a33c0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a33c0-108">Prerequisites</span></span>
<span data-ttu-id="a33c0-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="a33c0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a33c0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a33c0-111">Permission type</span></span>|<span data-ttu-id="a33c0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a33c0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a33c0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a33c0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a33c0-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a33c0-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a33c0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a33c0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a33c0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a33c0-116">Not supported.</span></span>|
|<span data-ttu-id="a33c0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a33c0-117">Application</span></span>|<span data-ttu-id="a33c0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a33c0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a33c0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a33c0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="a33c0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a33c0-120">Request headers</span></span>
|<span data-ttu-id="a33c0-121">标头</span><span class="sxs-lookup"><span data-stu-id="a33c0-121">Header</span></span>|<span data-ttu-id="a33c0-122">值</span><span class="sxs-lookup"><span data-stu-id="a33c0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a33c0-123">授权</span><span class="sxs-lookup"><span data-stu-id="a33c0-123">Authorization</span></span>|<span data-ttu-id="a33c0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a33c0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a33c0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a33c0-125">Accept</span></span>|<span data-ttu-id="a33c0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a33c0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a33c0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a33c0-127">Request body</span></span>
<span data-ttu-id="a33c0-128">在请求正文中，提供 iosVppEBookAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a33c0-128">In the request body, supply a JSON representation for the iosVppEBookAssignment object.</span></span>

<span data-ttu-id="a33c0-129">下表显示创建 iosVppEBookAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a33c0-129">The following table shows the properties that are required when you create the iosVppEBookAssignment.</span></span>

|<span data-ttu-id="a33c0-130">属性</span><span class="sxs-lookup"><span data-stu-id="a33c0-130">Property</span></span>|<span data-ttu-id="a33c0-131">类型</span><span class="sxs-lookup"><span data-stu-id="a33c0-131">Type</span></span>|<span data-ttu-id="a33c0-132">说明</span><span class="sxs-lookup"><span data-stu-id="a33c0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a33c0-133">id</span><span class="sxs-lookup"><span data-stu-id="a33c0-133">id</span></span>|<span data-ttu-id="a33c0-134">String</span><span class="sxs-lookup"><span data-stu-id="a33c0-134">String</span></span>|<span data-ttu-id="a33c0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a33c0-135">Key of the entity.</span></span> <span data-ttu-id="a33c0-136">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a33c0-136">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="a33c0-137">target</span><span class="sxs-lookup"><span data-stu-id="a33c0-137">target</span></span>|[<span data-ttu-id="a33c0-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="a33c0-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="a33c0-139">电子图书的分配目标。</span><span class="sxs-lookup"><span data-stu-id="a33c0-139">The assignment target for eBook.</span></span> <span data-ttu-id="a33c0-140">继承自 [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span><span class="sxs-lookup"><span data-stu-id="a33c0-140">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md)</span></span>|
|<span data-ttu-id="a33c0-141">installIntent</span><span class="sxs-lookup"><span data-stu-id="a33c0-141">installIntent</span></span>|[<span data-ttu-id="a33c0-142">installIntent</span><span class="sxs-lookup"><span data-stu-id="a33c0-142">installIntent</span></span>](../resources/intune-shared-installintent.md)|<span data-ttu-id="a33c0-143">电子图书的安装意图。</span><span class="sxs-lookup"><span data-stu-id="a33c0-143">The install intent for eBook.</span></span> <span data-ttu-id="a33c0-144">继承自[managedEBookAssignment](../resources/intune-books-managedebookassignment.md)。</span><span class="sxs-lookup"><span data-stu-id="a33c0-144">Inherited from [managedEBookAssignment](../resources/intune-books-managedebookassignment.md).</span></span> <span data-ttu-id="a33c0-145">可取值为：`available`、`required`、`uninstall`、`availableWithoutEnrollment`。</span><span class="sxs-lookup"><span data-stu-id="a33c0-145">Possible values are: `available`, `required`, `uninstall`, `availableWithoutEnrollment`.</span></span>|



## <a name="response"></a><span data-ttu-id="a33c0-146">响应</span><span class="sxs-lookup"><span data-stu-id="a33c0-146">Response</span></span>
<span data-ttu-id="a33c0-147">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a33c0-147">If successful, this method returns a `201 Created` response code and a [iosVppEBookAssignment](../resources/intune-books-iosvppebookassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a33c0-148">示例</span><span class="sxs-lookup"><span data-stu-id="a33c0-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="a33c0-149">请求</span><span class="sxs-lookup"><span data-stu-id="a33c0-149">Request</span></span>
<span data-ttu-id="a33c0-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a33c0-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a33c0-151">响应</span><span class="sxs-lookup"><span data-stu-id="a33c0-151">Response</span></span>
<span data-ttu-id="a33c0-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a33c0-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




