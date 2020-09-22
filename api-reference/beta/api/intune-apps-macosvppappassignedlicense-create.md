---
title: 创建 macOsVppAppAssignedLicense
description: 创建新的 macOsVppAppAssignedLicense 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 04d70ff17292731336347fdd1c64b969b9b9ffb8
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48000880"
---
# <a name="create-macosvppappassignedlicense"></a><span data-ttu-id="3c840-103">创建 macOsVppAppAssignedLicense</span><span class="sxs-lookup"><span data-stu-id="3c840-103">Create macOsVppAppAssignedLicense</span></span>

<span data-ttu-id="3c840-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c840-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c840-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3c840-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c840-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c840-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c840-107">创建新的 [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3c840-107">Create a new [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c840-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3c840-108">Prerequisites</span></span>
<span data-ttu-id="3c840-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c840-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c840-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c840-111">Permission type</span></span>|<span data-ttu-id="3c840-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3c840-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c840-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c840-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c840-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c840-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3c840-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c840-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c840-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c840-116">Not supported.</span></span>|
|<span data-ttu-id="3c840-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c840-117">Application</span></span>|<span data-ttu-id="3c840-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c840-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c840-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c840-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.macOsVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="3c840-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c840-120">Request headers</span></span>
|<span data-ttu-id="3c840-121">标头</span><span class="sxs-lookup"><span data-stu-id="3c840-121">Header</span></span>|<span data-ttu-id="3c840-122">值</span><span class="sxs-lookup"><span data-stu-id="3c840-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c840-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c840-123">Authorization</span></span>|<span data-ttu-id="3c840-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3c840-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c840-125">接受</span><span class="sxs-lookup"><span data-stu-id="3c840-125">Accept</span></span>|<span data-ttu-id="3c840-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c840-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c840-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c840-127">Request body</span></span>
<span data-ttu-id="3c840-128">在请求正文中，提供 macOsVppAppAssignedLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c840-128">In the request body, supply a JSON representation for the macOsVppAppAssignedLicense object.</span></span>

<span data-ttu-id="3c840-129">下表显示创建 macOsVppAppAssignedLicense 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3c840-129">The following table shows the properties that are required when you create the macOsVppAppAssignedLicense.</span></span>

|<span data-ttu-id="3c840-130">属性</span><span class="sxs-lookup"><span data-stu-id="3c840-130">Property</span></span>|<span data-ttu-id="3c840-131">类型</span><span class="sxs-lookup"><span data-stu-id="3c840-131">Type</span></span>|<span data-ttu-id="3c840-132">说明</span><span class="sxs-lookup"><span data-stu-id="3c840-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c840-133">id</span><span class="sxs-lookup"><span data-stu-id="3c840-133">id</span></span>|<span data-ttu-id="3c840-134">String</span><span class="sxs-lookup"><span data-stu-id="3c840-134">String</span></span>|<span data-ttu-id="3c840-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3c840-135">Key of the entity.</span></span>|
|<span data-ttu-id="3c840-136">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="3c840-136">userEmailAddress</span></span>|<span data-ttu-id="3c840-137">String</span><span class="sxs-lookup"><span data-stu-id="3c840-137">String</span></span>|<span data-ttu-id="3c840-138">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="3c840-138">The user email address.</span></span>|
|<span data-ttu-id="3c840-139">userId</span><span class="sxs-lookup"><span data-stu-id="3c840-139">userId</span></span>|<span data-ttu-id="3c840-140">String</span><span class="sxs-lookup"><span data-stu-id="3c840-140">String</span></span>|<span data-ttu-id="3c840-141">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="3c840-141">The user ID.</span></span>|
|<span data-ttu-id="3c840-142">userName</span><span class="sxs-lookup"><span data-stu-id="3c840-142">userName</span></span>|<span data-ttu-id="3c840-143">String</span><span class="sxs-lookup"><span data-stu-id="3c840-143">String</span></span>|<span data-ttu-id="3c840-144">用户名。</span><span class="sxs-lookup"><span data-stu-id="3c840-144">The user name.</span></span>|
|<span data-ttu-id="3c840-145">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="3c840-145">userPrincipalName</span></span>|<span data-ttu-id="3c840-146">String</span><span class="sxs-lookup"><span data-stu-id="3c840-146">String</span></span>|<span data-ttu-id="3c840-147">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="3c840-147">The user principal name.</span></span>|



## <a name="response"></a><span data-ttu-id="3c840-148">响应</span><span class="sxs-lookup"><span data-stu-id="3c840-148">Response</span></span>
<span data-ttu-id="3c840-149">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3c840-149">If successful, this method returns a `201 Created` response code and a [macOsVppAppAssignedLicense](../resources/intune-apps-macosvppappassignedlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c840-150">示例</span><span class="sxs-lookup"><span data-stu-id="3c840-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c840-151">请求</span><span class="sxs-lookup"><span data-stu-id="3c840-151">Request</span></span>
<span data-ttu-id="3c840-152">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c840-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="3c840-153">响应</span><span class="sxs-lookup"><span data-stu-id="3c840-153">Response</span></span>
<span data-ttu-id="3c840-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3c840-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






