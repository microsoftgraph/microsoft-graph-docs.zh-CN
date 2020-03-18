---
title: 更新 mobileAppDependency
description: 更新 mobileAppDependency 对象的属性。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 026194d2bf4bf6de2b657acd386a813915adae95
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42761242"
---
# <a name="update-mobileappdependency"></a><span data-ttu-id="d6128-103">更新 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="d6128-103">Update mobileAppDependency</span></span>

> <span data-ttu-id="d6128-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d6128-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d6128-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d6128-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d6128-106">更新[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="d6128-106">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d6128-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="d6128-107">Prerequisites</span></span>
<span data-ttu-id="d6128-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d6128-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d6128-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="d6128-110">Permission type</span></span>|<span data-ttu-id="d6128-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="d6128-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d6128-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d6128-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d6128-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6128-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d6128-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d6128-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d6128-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="d6128-115">Not supported.</span></span>|
|<span data-ttu-id="d6128-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="d6128-116">Application</span></span>|<span data-ttu-id="d6128-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d6128-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d6128-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d6128-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a><span data-ttu-id="d6128-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="d6128-119">Request headers</span></span>
|<span data-ttu-id="d6128-120">标头</span><span class="sxs-lookup"><span data-stu-id="d6128-120">Header</span></span>|<span data-ttu-id="d6128-121">值</span><span class="sxs-lookup"><span data-stu-id="d6128-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d6128-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d6128-122">Authorization</span></span>|<span data-ttu-id="d6128-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d6128-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d6128-124">接受</span><span class="sxs-lookup"><span data-stu-id="d6128-124">Accept</span></span>|<span data-ttu-id="d6128-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d6128-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d6128-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="d6128-126">Request body</span></span>
<span data-ttu-id="d6128-127">在请求正文中，提供[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d6128-127">In the request body, supply a JSON representation for the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

<span data-ttu-id="d6128-128">下表显示创建[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="d6128-128">The following table shows the properties that are required when you create the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>

|<span data-ttu-id="d6128-129">属性</span><span class="sxs-lookup"><span data-stu-id="d6128-129">Property</span></span>|<span data-ttu-id="d6128-130">类型</span><span class="sxs-lookup"><span data-stu-id="d6128-130">Type</span></span>|<span data-ttu-id="d6128-131">说明</span><span class="sxs-lookup"><span data-stu-id="d6128-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d6128-132">id</span><span class="sxs-lookup"><span data-stu-id="d6128-132">id</span></span>|<span data-ttu-id="d6128-133">String</span><span class="sxs-lookup"><span data-stu-id="d6128-133">String</span></span>|<span data-ttu-id="d6128-134">关系实体 id。继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d6128-134">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d6128-135">targetId</span><span class="sxs-lookup"><span data-stu-id="d6128-135">targetId</span></span>|<span data-ttu-id="d6128-136">String</span><span class="sxs-lookup"><span data-stu-id="d6128-136">String</span></span>|<span data-ttu-id="d6128-137">目标子移动应用程序的应用程序 id。继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d6128-137">The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d6128-138">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="d6128-138">targetDisplayName</span></span>|<span data-ttu-id="d6128-139">String</span><span class="sxs-lookup"><span data-stu-id="d6128-139">String</span></span>|<span data-ttu-id="d6128-140">目标子移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="d6128-140">The target child mobile app's display name.</span></span> <span data-ttu-id="d6128-141">继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="d6128-141">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="d6128-142">dependencyType</span><span class="sxs-lookup"><span data-stu-id="d6128-142">dependencyType</span></span>|[<span data-ttu-id="d6128-143">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="d6128-143">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="d6128-144">父应用和子应用之间的依赖关系的类型。</span><span class="sxs-lookup"><span data-stu-id="d6128-144">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="d6128-145">可取值为：`detect`、`autoInstall`。</span><span class="sxs-lookup"><span data-stu-id="d6128-145">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="d6128-146">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="d6128-146">dependentAppCount</span></span>|<span data-ttu-id="d6128-147">Int32</span><span class="sxs-lookup"><span data-stu-id="d6128-147">Int32</span></span>|<span data-ttu-id="d6128-148">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="d6128-148">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="d6128-149">响应</span><span class="sxs-lookup"><span data-stu-id="d6128-149">Response</span></span>
<span data-ttu-id="d6128-150">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="d6128-150">If successful, this method returns a `200 OK` response code and an updated [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d6128-151">示例</span><span class="sxs-lookup"><span data-stu-id="d6128-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="d6128-152">请求</span><span class="sxs-lookup"><span data-stu-id="d6128-152">Request</span></span>
<span data-ttu-id="d6128-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d6128-153">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
Content-type: application/json
Content-length: 211

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```

### <a name="response"></a><span data-ttu-id="d6128-154">响应</span><span class="sxs-lookup"><span data-stu-id="d6128-154">Response</span></span>
<span data-ttu-id="d6128-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d6128-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 260

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```




