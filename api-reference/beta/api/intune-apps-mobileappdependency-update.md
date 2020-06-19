---
title: 更新 mobileAppDependency
description: 更新 mobileAppDependency 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 2d1e03fc9772f4fb4d0e7833564563f6c39c399b
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793302"
---
# <a name="update-mobileappdependency"></a><span data-ttu-id="c2f17-103">更新 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="c2f17-103">Update mobileAppDependency</span></span>

<span data-ttu-id="c2f17-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c2f17-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="c2f17-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="c2f17-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="c2f17-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="c2f17-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="c2f17-107">更新[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c2f17-107">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="c2f17-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c2f17-108">Prerequisites</span></span>
<span data-ttu-id="c2f17-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="c2f17-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="c2f17-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="c2f17-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c2f17-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c2f17-111">Permission type</span></span>|<span data-ttu-id="c2f17-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c2f17-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c2f17-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c2f17-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c2f17-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2f17-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="c2f17-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c2f17-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c2f17-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c2f17-116">Not supported.</span></span>|
|<span data-ttu-id="c2f17-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c2f17-117">Application</span></span>|<span data-ttu-id="c2f17-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c2f17-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="c2f17-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c2f17-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a><span data-ttu-id="c2f17-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c2f17-120">Request headers</span></span>
|<span data-ttu-id="c2f17-121">标头</span><span class="sxs-lookup"><span data-stu-id="c2f17-121">Header</span></span>|<span data-ttu-id="c2f17-122">值</span><span class="sxs-lookup"><span data-stu-id="c2f17-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c2f17-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c2f17-123">Authorization</span></span>|<span data-ttu-id="c2f17-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c2f17-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c2f17-125">接受</span><span class="sxs-lookup"><span data-stu-id="c2f17-125">Accept</span></span>|<span data-ttu-id="c2f17-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c2f17-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c2f17-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c2f17-127">Request body</span></span>
<span data-ttu-id="c2f17-128">在请求正文中，提供[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c2f17-128">In the request body, supply a JSON representation for the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

<span data-ttu-id="c2f17-129">下表显示创建[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c2f17-129">The following table shows the properties that are required when you create the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>

|<span data-ttu-id="c2f17-130">属性</span><span class="sxs-lookup"><span data-stu-id="c2f17-130">Property</span></span>|<span data-ttu-id="c2f17-131">类型</span><span class="sxs-lookup"><span data-stu-id="c2f17-131">Type</span></span>|<span data-ttu-id="c2f17-132">说明</span><span class="sxs-lookup"><span data-stu-id="c2f17-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c2f17-133">id</span><span class="sxs-lookup"><span data-stu-id="c2f17-133">id</span></span>|<span data-ttu-id="c2f17-134">String</span><span class="sxs-lookup"><span data-stu-id="c2f17-134">String</span></span>|<span data-ttu-id="c2f17-135">关系实体 id。继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="c2f17-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="c2f17-136">targetId</span><span class="sxs-lookup"><span data-stu-id="c2f17-136">targetId</span></span>|<span data-ttu-id="c2f17-137">String</span><span class="sxs-lookup"><span data-stu-id="c2f17-137">String</span></span>|<span data-ttu-id="c2f17-138">目标移动应用程序的应用程序 id。继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="c2f17-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="c2f17-139">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="c2f17-139">targetDisplayName</span></span>|<span data-ttu-id="c2f17-140">String</span><span class="sxs-lookup"><span data-stu-id="c2f17-140">String</span></span>|<span data-ttu-id="c2f17-141">目标移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c2f17-141">The target mobile app's display name.</span></span> <span data-ttu-id="c2f17-142">继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="c2f17-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="c2f17-143">dependencyType</span><span class="sxs-lookup"><span data-stu-id="c2f17-143">dependencyType</span></span>|[<span data-ttu-id="c2f17-144">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="c2f17-144">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="c2f17-145">父应用和子应用之间的依赖关系的类型。</span><span class="sxs-lookup"><span data-stu-id="c2f17-145">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="c2f17-146">可取值为：`detect`、`autoInstall`。</span><span class="sxs-lookup"><span data-stu-id="c2f17-146">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="c2f17-147">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="c2f17-147">dependentAppCount</span></span>|<span data-ttu-id="c2f17-148">Int32</span><span class="sxs-lookup"><span data-stu-id="c2f17-148">Int32</span></span>|<span data-ttu-id="c2f17-149">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="c2f17-149">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="c2f17-150">响应</span><span class="sxs-lookup"><span data-stu-id="c2f17-150">Response</span></span>
<span data-ttu-id="c2f17-151">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c2f17-151">If successful, this method returns a `200 OK` response code and an updated [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c2f17-152">示例</span><span class="sxs-lookup"><span data-stu-id="c2f17-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="c2f17-153">请求</span><span class="sxs-lookup"><span data-stu-id="c2f17-153">Request</span></span>
<span data-ttu-id="c2f17-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c2f17-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="c2f17-155">响应</span><span class="sxs-lookup"><span data-stu-id="c2f17-155">Response</span></span>
<span data-ttu-id="c2f17-156">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="c2f17-156">Here is an example of the response.</span></span> <span data-ttu-id="c2f17-157">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="c2f17-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="c2f17-158">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="c2f17-158">All of the properties will be returned from an actual call.</span></span>
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



