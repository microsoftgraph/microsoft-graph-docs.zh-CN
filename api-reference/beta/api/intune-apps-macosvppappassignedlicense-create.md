---
title: 创建 macOsVppAppAssignedLicense
description: 创建新的 macOsVppAppAssignedLicense 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 05424b5f8eaff6f3d055fd6f3babe77fb726b194
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30983846"
---
# <a name="create-macosvppappassignedlicense"></a><span data-ttu-id="c2ee1-103">创建 macOsVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="c2ee1-103">Create macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="c2ee1-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c2ee1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2ee1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c2ee1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2ee1-106">创建新的[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c2ee1-106">Create a new [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2ee1-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="c2ee1-107">Prerequisites</span></span>
<span data-ttu-id="c2ee1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c2ee1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2ee1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2ee1-110">Permission type</span></span>|<span data-ttu-id="c2ee1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c2ee1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2ee1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2ee1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="c2ee1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2ee1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c2ee1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2ee1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2ee1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2ee1-115">Not supported.</span></span>|
|<span data-ttu-id="c2ee1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2ee1-116">Application</span></span>|<span data-ttu-id="c2ee1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2ee1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2ee1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2ee1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="c2ee1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2ee1-119">Request headers</span></span>
|<span data-ttu-id="c2ee1-120">标头</span><span class="sxs-lookup"><span data-stu-id="c2ee1-120">Header</span></span>|<span data-ttu-id="c2ee1-121">值</span><span class="sxs-lookup"><span data-stu-id="c2ee1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2ee1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2ee1-122">Authorization</span></span>|<span data-ttu-id="c2ee1-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c2ee1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2ee1-124">接受</span><span class="sxs-lookup"><span data-stu-id="c2ee1-124">Accept</span></span>|<span data-ttu-id="c2ee1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="c2ee1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2ee1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2ee1-126">Request body</span></span>
<span data-ttu-id="c2ee1-127">在请求正文中, 提供 macOsVppAppAssignedLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2ee1-127">In the request body, supply a JSON representation for the macOsVppAppAssignedLicense object.</span></span>

<span data-ttu-id="c2ee1-128">下表显示创建 macOsVppAppAssignedLicense 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c2ee1-128">The following table shows the properties that are required when you create the macOsVppAppAssignedLicense.</span></span>

|<span data-ttu-id="c2ee1-129">属性</span><span class="sxs-lookup"><span data-stu-id="c2ee1-129">Property</span></span>|<span data-ttu-id="c2ee1-130">类型</span><span class="sxs-lookup"><span data-stu-id="c2ee1-130">Type</span></span>|<span data-ttu-id="c2ee1-131">说明</span><span class="sxs-lookup"><span data-stu-id="c2ee1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2ee1-132">id</span><span class="sxs-lookup"><span data-stu-id="c2ee1-132">id</span></span>|<span data-ttu-id="c2ee1-133">String</span><span class="sxs-lookup"><span data-stu-id="c2ee1-133">String</span></span>|<span data-ttu-id="c2ee1-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c2ee1-134">Key of the entity.</span></span>|
|<span data-ttu-id="c2ee1-135">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="c2ee1-135">userEmailAddress</span></span>|<span data-ttu-id="c2ee1-136">String</span><span class="sxs-lookup"><span data-stu-id="c2ee1-136">String</span></span>|<span data-ttu-id="c2ee1-137">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="c2ee1-137">The user email address.</span></span>|
|<span data-ttu-id="c2ee1-138">userId</span><span class="sxs-lookup"><span data-stu-id="c2ee1-138">userId</span></span>|<span data-ttu-id="c2ee1-139">String</span><span class="sxs-lookup"><span data-stu-id="c2ee1-139">String</span></span>|<span data-ttu-id="c2ee1-140">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="c2ee1-140">The user ID.</span></span>|
|<span data-ttu-id="c2ee1-141">userName</span><span class="sxs-lookup"><span data-stu-id="c2ee1-141">userName</span></span>|<span data-ttu-id="c2ee1-142">String</span><span class="sxs-lookup"><span data-stu-id="c2ee1-142">String</span></span>|<span data-ttu-id="c2ee1-143">用户名。</span><span class="sxs-lookup"><span data-stu-id="c2ee1-143">The user name.</span></span>|
|<span data-ttu-id="c2ee1-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="c2ee1-144">userPrincipalName</span></span>|<span data-ttu-id="c2ee1-145">String</span><span class="sxs-lookup"><span data-stu-id="c2ee1-145">String</span></span>|<span data-ttu-id="c2ee1-146">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="c2ee1-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="c2ee1-147">响应</span><span class="sxs-lookup"><span data-stu-id="c2ee1-147">Response</span></span>
<span data-ttu-id="c2ee1-148">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c2ee1-148">If successful, this method returns a `201 Created` response code and a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2ee1-149">示例</span><span class="sxs-lookup"><span data-stu-id="c2ee1-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2ee1-150">请求</span><span class="sxs-lookup"><span data-stu-id="c2ee1-150">Request</span></span>
<span data-ttu-id="c2ee1-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c2ee1-151">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="c2ee1-152">响应</span><span class="sxs-lookup"><span data-stu-id="c2ee1-152">Response</span></span>
<span data-ttu-id="c2ee1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c2ee1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.macOsVppAppAssignedLicense",
  "id": "a1204d8e-4d8e-a120-8e4d-20a18e4d20a1",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```




