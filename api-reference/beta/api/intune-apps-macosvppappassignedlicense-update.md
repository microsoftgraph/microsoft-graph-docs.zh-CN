---
title: 更新 macOsVppAppAssignedLicense
description: 更新 macOsVppAppAssignedLicense 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 92502321dc3d8eedb27abe595dc81f3dd0a94519
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51140299"
---
# <a name="update-macosvppappassignedlicense"></a><span data-ttu-id="b6a21-103">更新 macOsVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="b6a21-103">Update macOsVppAppAssignedLicense</span></span>

<span data-ttu-id="b6a21-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b6a21-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b6a21-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b6a21-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b6a21-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b6a21-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b6a21-107">更新 [macOsVppAppAssignedLicense 对象](../resources/intune-apps-macosvppappassignedlicense.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="b6a21-107">Update the properties of a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b6a21-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b6a21-108">Prerequisites</span></span>
<span data-ttu-id="b6a21-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b6a21-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b6a21-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b6a21-111">Permission type</span></span>|<span data-ttu-id="b6a21-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b6a21-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b6a21-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b6a21-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b6a21-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6a21-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b6a21-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b6a21-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b6a21-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b6a21-116">Not supported.</span></span>|
|<span data-ttu-id="b6a21-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b6a21-117">Application</span></span>|<span data-ttu-id="b6a21-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b6a21-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b6a21-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b6a21-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
```

## <a name="request-headers"></a><span data-ttu-id="b6a21-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b6a21-120">Request headers</span></span>
|<span data-ttu-id="b6a21-121">标头</span><span class="sxs-lookup"><span data-stu-id="b6a21-121">Header</span></span>|<span data-ttu-id="b6a21-122">值</span><span class="sxs-lookup"><span data-stu-id="b6a21-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b6a21-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b6a21-123">Authorization</span></span>|<span data-ttu-id="b6a21-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b6a21-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b6a21-125">接受</span><span class="sxs-lookup"><span data-stu-id="b6a21-125">Accept</span></span>|<span data-ttu-id="b6a21-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b6a21-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b6a21-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b6a21-127">Request body</span></span>
<span data-ttu-id="b6a21-128">在请求正文中，提供 [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b6a21-128">In the request body, supply a JSON representation for the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

<span data-ttu-id="b6a21-129">下表显示创建 [macOsVppAppAssignedLicense 时所需的属性](../resources/intune-apps-macosvppappassignedlicense.md)。</span><span class="sxs-lookup"><span data-stu-id="b6a21-129">The following table shows the properties that are required when you create the [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md).</span></span>

|<span data-ttu-id="b6a21-130">属性</span><span class="sxs-lookup"><span data-stu-id="b6a21-130">Property</span></span>|<span data-ttu-id="b6a21-131">类型</span><span class="sxs-lookup"><span data-stu-id="b6a21-131">Type</span></span>|<span data-ttu-id="b6a21-132">说明</span><span class="sxs-lookup"><span data-stu-id="b6a21-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b6a21-133">id</span><span class="sxs-lookup"><span data-stu-id="b6a21-133">id</span></span>|<span data-ttu-id="b6a21-134">String</span><span class="sxs-lookup"><span data-stu-id="b6a21-134">String</span></span>|<span data-ttu-id="b6a21-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b6a21-135">Key of the entity.</span></span>|
|<span data-ttu-id="b6a21-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="b6a21-136">userEmailAddress</span></span>|<span data-ttu-id="b6a21-137">String</span><span class="sxs-lookup"><span data-stu-id="b6a21-137">String</span></span>|<span data-ttu-id="b6a21-138">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="b6a21-138">The user email address.</span></span>|
|<span data-ttu-id="b6a21-139">userId</span><span class="sxs-lookup"><span data-stu-id="b6a21-139">userId</span></span>|<span data-ttu-id="b6a21-140">String</span><span class="sxs-lookup"><span data-stu-id="b6a21-140">String</span></span>|<span data-ttu-id="b6a21-141">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="b6a21-141">The user ID.</span></span>|
|<span data-ttu-id="b6a21-142">userName</span><span class="sxs-lookup"><span data-stu-id="b6a21-142">userName</span></span>|<span data-ttu-id="b6a21-143">String</span><span class="sxs-lookup"><span data-stu-id="b6a21-143">String</span></span>|<span data-ttu-id="b6a21-144">用户名。</span><span class="sxs-lookup"><span data-stu-id="b6a21-144">The user name.</span></span>|
|<span data-ttu-id="b6a21-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="b6a21-145">userPrincipalName</span></span>|<span data-ttu-id="b6a21-146">String</span><span class="sxs-lookup"><span data-stu-id="b6a21-146">String</span></span>|<span data-ttu-id="b6a21-147">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="b6a21-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="b6a21-148">响应</span><span class="sxs-lookup"><span data-stu-id="b6a21-148">Response</span></span>
<span data-ttu-id="b6a21-149">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b6a21-149">If successful, this method returns a `200 OK` response code and an updated [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b6a21-150">示例</span><span class="sxs-lookup"><span data-stu-id="b6a21-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="b6a21-151">请求</span><span class="sxs-lookup"><span data-stu-id="b6a21-151">Request</span></span>
<span data-ttu-id="b6a21-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b6a21-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses/{macOsVppAppAssignedLicenseId}
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

### <a name="response"></a><span data-ttu-id="b6a21-153">响应</span><span class="sxs-lookup"><span data-stu-id="b6a21-153">Response</span></span>
<span data-ttu-id="b6a21-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b6a21-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




