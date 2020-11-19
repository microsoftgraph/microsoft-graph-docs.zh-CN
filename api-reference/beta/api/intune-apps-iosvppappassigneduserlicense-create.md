---
title: 创建 iosVppAppAssignedUserLicense
description: 创建新的 iosVppAppAssignedUserLicense 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: da4ff316a703bf928db834d6e1fdabfde6a76c2d
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49251749"
---
# <a name="create-iosvppappassigneduserlicense"></a><span data-ttu-id="37702-103">创建 iosVppAppAssignedUserLicense</span><span class="sxs-lookup"><span data-stu-id="37702-103">Create iosVppAppAssignedUserLicense</span></span>

<span data-ttu-id="37702-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="37702-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="37702-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="37702-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37702-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="37702-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37702-107">创建新的 [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="37702-107">Create a new [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37702-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="37702-108">Prerequisites</span></span>
<span data-ttu-id="37702-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="37702-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37702-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="37702-111">Permission type</span></span>|<span data-ttu-id="37702-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="37702-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37702-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="37702-113">Delegated (work or school account)</span></span>|<span data-ttu-id="37702-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37702-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="37702-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="37702-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37702-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="37702-116">Not supported.</span></span>|
|<span data-ttu-id="37702-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="37702-117">Application</span></span>|<span data-ttu-id="37702-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37702-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37702-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="37702-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
```

## <a name="request-headers"></a><span data-ttu-id="37702-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="37702-120">Request headers</span></span>
|<span data-ttu-id="37702-121">标头</span><span class="sxs-lookup"><span data-stu-id="37702-121">Header</span></span>|<span data-ttu-id="37702-122">值</span><span class="sxs-lookup"><span data-stu-id="37702-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37702-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="37702-123">Authorization</span></span>|<span data-ttu-id="37702-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="37702-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37702-125">接受</span><span class="sxs-lookup"><span data-stu-id="37702-125">Accept</span></span>|<span data-ttu-id="37702-126">application/json</span><span class="sxs-lookup"><span data-stu-id="37702-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37702-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="37702-127">Request body</span></span>
<span data-ttu-id="37702-128">在请求正文中，提供 iosVppAppAssignedUserLicense 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="37702-128">In the request body, supply a JSON representation for the iosVppAppAssignedUserLicense object.</span></span>

<span data-ttu-id="37702-129">下表显示创建 iosVppAppAssignedUserLicense 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="37702-129">The following table shows the properties that are required when you create the iosVppAppAssignedUserLicense.</span></span>

|<span data-ttu-id="37702-130">属性</span><span class="sxs-lookup"><span data-stu-id="37702-130">Property</span></span>|<span data-ttu-id="37702-131">类型</span><span class="sxs-lookup"><span data-stu-id="37702-131">Type</span></span>|<span data-ttu-id="37702-132">说明</span><span class="sxs-lookup"><span data-stu-id="37702-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37702-133">id</span><span class="sxs-lookup"><span data-stu-id="37702-133">id</span></span>|<span data-ttu-id="37702-134">String</span><span class="sxs-lookup"><span data-stu-id="37702-134">String</span></span>|<span data-ttu-id="37702-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="37702-135">Key of the entity.</span></span> <span data-ttu-id="37702-136">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="37702-136">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="37702-137">userEmailAddress</span><span class="sxs-lookup"><span data-stu-id="37702-137">userEmailAddress</span></span>|<span data-ttu-id="37702-138">String</span><span class="sxs-lookup"><span data-stu-id="37702-138">String</span></span>|<span data-ttu-id="37702-139">用户电子邮件地址。</span><span class="sxs-lookup"><span data-stu-id="37702-139">The user email address.</span></span> <span data-ttu-id="37702-140">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="37702-140">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="37702-141">userId</span><span class="sxs-lookup"><span data-stu-id="37702-141">userId</span></span>|<span data-ttu-id="37702-142">String</span><span class="sxs-lookup"><span data-stu-id="37702-142">String</span></span>|<span data-ttu-id="37702-143">用户 ID。</span><span class="sxs-lookup"><span data-stu-id="37702-143">The user ID.</span></span> <span data-ttu-id="37702-144">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="37702-144">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="37702-145">userName</span><span class="sxs-lookup"><span data-stu-id="37702-145">userName</span></span>|<span data-ttu-id="37702-146">String</span><span class="sxs-lookup"><span data-stu-id="37702-146">String</span></span>|<span data-ttu-id="37702-147">用户名。</span><span class="sxs-lookup"><span data-stu-id="37702-147">The user name.</span></span> <span data-ttu-id="37702-148">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="37702-148">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|
|<span data-ttu-id="37702-149">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="37702-149">userPrincipalName</span></span>|<span data-ttu-id="37702-150">String</span><span class="sxs-lookup"><span data-stu-id="37702-150">String</span></span>|<span data-ttu-id="37702-151">用户主体名称。</span><span class="sxs-lookup"><span data-stu-id="37702-151">The user principal name.</span></span> <span data-ttu-id="37702-152">继承自 [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span><span class="sxs-lookup"><span data-stu-id="37702-152">Inherited from [iosVppAppAssignedLicense](../resources/intune-apps-iosvppappassignedlicense.md)</span></span>|



## <a name="response"></a><span data-ttu-id="37702-153">响应</span><span class="sxs-lookup"><span data-stu-id="37702-153">Response</span></span>
<span data-ttu-id="37702-154">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="37702-154">If successful, this method returns a `201 Created` response code and a [iosVppAppAssignedUserLicense](../resources/intune-apps-iosvppappassigneduserlicense.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37702-155">示例</span><span class="sxs-lookup"><span data-stu-id="37702-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="37702-156">请求</span><span class="sxs-lookup"><span data-stu-id="37702-156">Request</span></span>
<span data-ttu-id="37702-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="37702-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/microsoft.graph.iosVppApp/assignedLicenses
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```

### <a name="response"></a><span data-ttu-id="37702-158">响应</span><span class="sxs-lookup"><span data-stu-id="37702-158">Response</span></span>
<span data-ttu-id="37702-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="37702-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.iosVppAppAssignedUserLicense",
  "id": "fedc747d-747d-fedc-7d74-dcfe7d74dcfe",
  "userEmailAddress": "User Email Address value",
  "userId": "User Id value",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value"
}
```




