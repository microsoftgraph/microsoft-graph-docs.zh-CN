---
title: 创建 macOsVppAppAssignedLicense
description: 创建新的 macOsVppAppAssignedLicense 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 07c0bafef2eb86128c8d9bc8cfb071b45bc1e913
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29429430"
---
# <a name="create-macosvppappassignedlicense"></a><span data-ttu-id="53e3d-103">创建 macOsVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="53e3d-103">Create macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="53e3d-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="53e3d-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="53e3d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="53e3d-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="53e3d-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="53e3d-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="53e3d-107">创建新的[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="53e3d-107">Create a new [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="53e3d-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="53e3d-108">Prerequisites</span></span>
<span data-ttu-id="53e3d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="53e3d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="53e3d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="53e3d-111">Permission type</span></span>|<span data-ttu-id="53e3d-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="53e3d-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="53e3d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="53e3d-113">Delegated (work or school account)</span></span>|<span data-ttu-id="53e3d-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="53e3d-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="53e3d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="53e3d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="53e3d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="53e3d-116">Not supported.</span></span>|
|<span data-ttu-id="53e3d-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="53e3d-117">Application</span></span>|<span data-ttu-id="53e3d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="53e3d-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="53e3d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="53e3d-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="53e3d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="53e3d-120">Request headers</span></span>
|<span data-ttu-id="53e3d-121">标头</span><span class="sxs-lookup"><span data-stu-id="53e3d-121">Header</span></span>|<span data-ttu-id="53e3d-122">值</span><span class="sxs-lookup"><span data-stu-id="53e3d-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="53e3d-123">授权</span><span class="sxs-lookup"><span data-stu-id="53e3d-123">Authorization</span></span>|<span data-ttu-id="53e3d-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="53e3d-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="53e3d-125">Accept</span><span class="sxs-lookup"><span data-stu-id="53e3d-125">Accept</span></span>|<span data-ttu-id="53e3d-126">application/json</span><span class="sxs-lookup"><span data-stu-id="53e3d-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="53e3d-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="53e3d-127">Request body</span></span>
<span data-ttu-id="53e3d-128">在请求正文中，提供 macOsVppAppAssignedLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="53e3d-128">In the request body, supply a JSON representation for the macOsVppAppAssignedLicense object.</span></span>

<span data-ttu-id="53e3d-129">下表显示时创建 macOsVppAppAssignedLicense 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="53e3d-129">The following table shows the properties that are required when you create the macOsVppAppAssignedLicense.</span></span>

|<span data-ttu-id="53e3d-130">属性</span><span class="sxs-lookup"><span data-stu-id="53e3d-130">Property</span></span>|<span data-ttu-id="53e3d-131">类型</span><span class="sxs-lookup"><span data-stu-id="53e3d-131">Type</span></span>|<span data-ttu-id="53e3d-132">说明</span><span class="sxs-lookup"><span data-stu-id="53e3d-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="53e3d-133">id</span><span class="sxs-lookup"><span data-stu-id="53e3d-133">id</span></span>|<span data-ttu-id="53e3d-134">String</span><span class="sxs-lookup"><span data-stu-id="53e3d-134">String</span></span>|<span data-ttu-id="53e3d-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="53e3d-135">Key of the entity.</span></span>|
|<span data-ttu-id="53e3d-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="53e3d-136">userEmailAddress</span></span>|<span data-ttu-id="53e3d-137">String</span><span class="sxs-lookup"><span data-stu-id="53e3d-137">String</span></span>|<span data-ttu-id="53e3d-138">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="53e3d-138">The user email address.</span></span>|
|<span data-ttu-id="53e3d-139">userId</span><span class="sxs-lookup"><span data-stu-id="53e3d-139">userId</span></span>|<span data-ttu-id="53e3d-140">String</span><span class="sxs-lookup"><span data-stu-id="53e3d-140">String</span></span>|<span data-ttu-id="53e3d-141">用户 id。</span><span class="sxs-lookup"><span data-stu-id="53e3d-141">The user ID.</span></span>|
|<span data-ttu-id="53e3d-142">userName</span><span class="sxs-lookup"><span data-stu-id="53e3d-142">userName</span></span>|<span data-ttu-id="53e3d-143">String</span><span class="sxs-lookup"><span data-stu-id="53e3d-143">String</span></span>|<span data-ttu-id="53e3d-144">用户名。</span><span class="sxs-lookup"><span data-stu-id="53e3d-144">The user name.</span></span>|
|<span data-ttu-id="53e3d-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="53e3d-145">userPrincipalName</span></span>|<span data-ttu-id="53e3d-146">String</span><span class="sxs-lookup"><span data-stu-id="53e3d-146">String</span></span>|<span data-ttu-id="53e3d-147">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="53e3d-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="53e3d-148">响应</span><span class="sxs-lookup"><span data-stu-id="53e3d-148">Response</span></span>
<span data-ttu-id="53e3d-149">如果成功，此方法返回`201 Created`响应代码和响应正文中的[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="53e3d-149">If successful, this method returns a `201 Created` response code and a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="53e3d-150">示例</span><span class="sxs-lookup"><span data-stu-id="53e3d-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="53e3d-151">请求</span><span class="sxs-lookup"><span data-stu-id="53e3d-151">Request</span></span>
<span data-ttu-id="53e3d-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="53e3d-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="53e3d-153">响应</span><span class="sxs-lookup"><span data-stu-id="53e3d-153">Response</span></span>
<span data-ttu-id="53e3d-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="53e3d-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




