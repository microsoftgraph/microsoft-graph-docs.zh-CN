---
title: 创建 macOsVppAppAssignedLicense
description: 创建新的 macOsVppAppAssignedLicense 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: b21b002e7cae3f3b52967cb320caa43e67c10a9d
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32495321"
---
# <a name="create-macosvppappassignedlicense"></a><span data-ttu-id="8b950-103">创建 macOsVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="8b950-103">Create macOsVppAppAssignedLicense</span></span>

> <span data-ttu-id="8b950-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="8b950-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8b950-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="8b950-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8b950-106">创建新的[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8b950-106">Create a new [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8b950-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="8b950-107">Prerequisites</span></span>
<span data-ttu-id="8b950-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="8b950-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8b950-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="8b950-110">Permission type</span></span>|<span data-ttu-id="8b950-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="8b950-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8b950-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="8b950-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8b950-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8b950-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8b950-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="8b950-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8b950-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b950-115">Not supported.</span></span>|
|<span data-ttu-id="8b950-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="8b950-116">Application</span></span>|<span data-ttu-id="8b950-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="8b950-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="8b950-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="8b950-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="8b950-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="8b950-119">Request headers</span></span>
|<span data-ttu-id="8b950-120">标头</span><span class="sxs-lookup"><span data-stu-id="8b950-120">Header</span></span>|<span data-ttu-id="8b950-121">值</span><span class="sxs-lookup"><span data-stu-id="8b950-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8b950-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8b950-122">Authorization</span></span>|<span data-ttu-id="8b950-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="8b950-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8b950-124">接受</span><span class="sxs-lookup"><span data-stu-id="8b950-124">Accept</span></span>|<span data-ttu-id="8b950-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8b950-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8b950-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="8b950-126">Request body</span></span>
<span data-ttu-id="8b950-127">在请求正文中, 提供 macOsVppAppAssignedLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8b950-127">In the request body, supply a JSON representation for the macOsVppAppAssignedLicense object.</span></span>

<span data-ttu-id="8b950-128">下表显示创建 macOsVppAppAssignedLicense 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="8b950-128">The following table shows the properties that are required when you create the macOsVppAppAssignedLicense.</span></span>

|<span data-ttu-id="8b950-129">属性</span><span class="sxs-lookup"><span data-stu-id="8b950-129">Property</span></span>|<span data-ttu-id="8b950-130">类型</span><span class="sxs-lookup"><span data-stu-id="8b950-130">Type</span></span>|<span data-ttu-id="8b950-131">说明</span><span class="sxs-lookup"><span data-stu-id="8b950-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8b950-132">id</span><span class="sxs-lookup"><span data-stu-id="8b950-132">id</span></span>|<span data-ttu-id="8b950-133">String</span><span class="sxs-lookup"><span data-stu-id="8b950-133">String</span></span>|<span data-ttu-id="8b950-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="8b950-134">Key of the entity.</span></span>|
|<span data-ttu-id="8b950-135">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="8b950-135">userEmailAddress</span></span>|<span data-ttu-id="8b950-136">字符串</span><span class="sxs-lookup"><span data-stu-id="8b950-136">String</span></span>|<span data-ttu-id="8b950-137">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="8b950-137">The user email address.</span></span>|
|<span data-ttu-id="8b950-138">userId</span><span class="sxs-lookup"><span data-stu-id="8b950-138">userId</span></span>|<span data-ttu-id="8b950-139">字符串</span><span class="sxs-lookup"><span data-stu-id="8b950-139">String</span></span>|<span data-ttu-id="8b950-140">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="8b950-140">The user ID.</span></span>|
|<span data-ttu-id="8b950-141">userName</span><span class="sxs-lookup"><span data-stu-id="8b950-141">userName</span></span>|<span data-ttu-id="8b950-142">String</span><span class="sxs-lookup"><span data-stu-id="8b950-142">String</span></span>|<span data-ttu-id="8b950-143">用户名。</span><span class="sxs-lookup"><span data-stu-id="8b950-143">The user name.</span></span>|
|<span data-ttu-id="8b950-144">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="8b950-144">userPrincipalName</span></span>|<span data-ttu-id="8b950-145">String</span><span class="sxs-lookup"><span data-stu-id="8b950-145">String</span></span>|<span data-ttu-id="8b950-146">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="8b950-146">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="8b950-147">响应</span><span class="sxs-lookup"><span data-stu-id="8b950-147">Response</span></span>
<span data-ttu-id="8b950-148">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md)对象。</span><span class="sxs-lookup"><span data-stu-id="8b950-148">If successful, this method returns a `201 Created` response code and a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8b950-149">示例</span><span class="sxs-lookup"><span data-stu-id="8b950-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="8b950-150">请求</span><span class="sxs-lookup"><span data-stu-id="8b950-150">Request</span></span>
<span data-ttu-id="8b950-151">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="8b950-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8b950-152">响应</span><span class="sxs-lookup"><span data-stu-id="8b950-152">Response</span></span>
<span data-ttu-id="8b950-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="8b950-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





