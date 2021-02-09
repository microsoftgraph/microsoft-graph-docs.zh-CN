---
title: 更新 mobileAppDependency
description: 更新 mobileAppDependency 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 45bb4504fc2d65a7d9284e15e73d6c5da575f881
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50155312"
---
# <a name="update-mobileappdependency"></a><span data-ttu-id="4fbaf-103">更新 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="4fbaf-103">Update mobileAppDependency</span></span>

<span data-ttu-id="4fbaf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="4fbaf-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="4fbaf-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4fbaf-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4fbaf-107">更新 [mobileAppDependency 对象](../resources/intune-apps-mobileappdependency.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-107">Update the properties of a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4fbaf-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="4fbaf-108">Prerequisites</span></span>
<span data-ttu-id="4fbaf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4fbaf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="4fbaf-111">Permission type</span></span>|<span data-ttu-id="4fbaf-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4fbaf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4fbaf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4fbaf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="4fbaf-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fbaf-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="4fbaf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4fbaf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4fbaf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-116">Not supported.</span></span>|
|<span data-ttu-id="4fbaf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="4fbaf-117">Application</span></span>|<span data-ttu-id="4fbaf-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4fbaf-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4fbaf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4fbaf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a><span data-ttu-id="4fbaf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="4fbaf-120">Request headers</span></span>
|<span data-ttu-id="4fbaf-121">标头</span><span class="sxs-lookup"><span data-stu-id="4fbaf-121">Header</span></span>|<span data-ttu-id="4fbaf-122">值</span><span class="sxs-lookup"><span data-stu-id="4fbaf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4fbaf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="4fbaf-123">Authorization</span></span>|<span data-ttu-id="4fbaf-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4fbaf-125">接受</span><span class="sxs-lookup"><span data-stu-id="4fbaf-125">Accept</span></span>|<span data-ttu-id="4fbaf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="4fbaf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4fbaf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="4fbaf-127">Request body</span></span>
<span data-ttu-id="4fbaf-128">在请求正文中，提供 [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-128">In the request body, supply a JSON representation for the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

<span data-ttu-id="4fbaf-129">下表显示创建 [mobileAppDependency 时所需的属性](../resources/intune-apps-mobileappdependency.md)。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-129">The following table shows the properties that are required when you create the [mobileAppDependency](../resources/intune-apps-mobileappdependency.md).</span></span>

|<span data-ttu-id="4fbaf-130">属性</span><span class="sxs-lookup"><span data-stu-id="4fbaf-130">Property</span></span>|<span data-ttu-id="4fbaf-131">类型</span><span class="sxs-lookup"><span data-stu-id="4fbaf-131">Type</span></span>|<span data-ttu-id="4fbaf-132">说明</span><span class="sxs-lookup"><span data-stu-id="4fbaf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4fbaf-133">id</span><span class="sxs-lookup"><span data-stu-id="4fbaf-133">id</span></span>|<span data-ttu-id="4fbaf-134">String</span><span class="sxs-lookup"><span data-stu-id="4fbaf-134">String</span></span>|<span data-ttu-id="4fbaf-135">关系实体 ID。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="4fbaf-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="4fbaf-136">targetId</span><span class="sxs-lookup"><span data-stu-id="4fbaf-136">targetId</span></span>|<span data-ttu-id="4fbaf-137">String</span><span class="sxs-lookup"><span data-stu-id="4fbaf-137">String</span></span>|<span data-ttu-id="4fbaf-138">目标移动应用的应用 ID。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="4fbaf-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="4fbaf-139">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="4fbaf-139">targetDisplayName</span></span>|<span data-ttu-id="4fbaf-140">String</span><span class="sxs-lookup"><span data-stu-id="4fbaf-140">String</span></span>|<span data-ttu-id="4fbaf-141">目标移动应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-141">The target mobile app's display name.</span></span> <span data-ttu-id="4fbaf-142">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="4fbaf-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="4fbaf-143">targetDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="4fbaf-143">targetDisplayVersion</span></span>|<span data-ttu-id="4fbaf-144">String</span><span class="sxs-lookup"><span data-stu-id="4fbaf-144">String</span></span>|<span data-ttu-id="4fbaf-145">目标移动应用的显示版本。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-145">The target mobile app's display version.</span></span> <span data-ttu-id="4fbaf-146">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="4fbaf-146">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="4fbaf-147">targetPublisher</span><span class="sxs-lookup"><span data-stu-id="4fbaf-147">targetPublisher</span></span>|<span data-ttu-id="4fbaf-148">String</span><span class="sxs-lookup"><span data-stu-id="4fbaf-148">String</span></span>|<span data-ttu-id="4fbaf-149">目标移动应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-149">The target mobile app's publisher.</span></span> <span data-ttu-id="4fbaf-150">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="4fbaf-150">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="4fbaf-151">targetType</span><span class="sxs-lookup"><span data-stu-id="4fbaf-151">targetType</span></span>|[<span data-ttu-id="4fbaf-152">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="4fbaf-152">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="4fbaf-153">关系类型，指示目标是父级还是子级。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-153">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="4fbaf-154">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-154">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="4fbaf-155">可取值为：`child`、`parent`。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-155">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="4fbaf-156">dependencyType</span><span class="sxs-lookup"><span data-stu-id="4fbaf-156">dependencyType</span></span>|[<span data-ttu-id="4fbaf-157">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="4fbaf-157">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="4fbaf-158">父应用和子应用之间的依赖关系类型。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-158">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="4fbaf-159">可取值为：`detect`、`autoInstall`。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-159">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="4fbaf-160">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="4fbaf-160">dependentAppCount</span></span>|<span data-ttu-id="4fbaf-161">Int32</span><span class="sxs-lookup"><span data-stu-id="4fbaf-161">Int32</span></span>|<span data-ttu-id="4fbaf-162">直接或间接依赖于父应用的应用总数。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-162">The total number of apps that directly or indirectly depend on the parent app.</span></span>|
|<span data-ttu-id="4fbaf-163">dependsOnAppCount</span><span class="sxs-lookup"><span data-stu-id="4fbaf-163">dependsOnAppCount</span></span>|<span data-ttu-id="4fbaf-164">Int32</span><span class="sxs-lookup"><span data-stu-id="4fbaf-164">Int32</span></span>|<span data-ttu-id="4fbaf-165">子应用直接或间接依赖的应用总数。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-165">The total number of apps the child app directly or indirectly depends on.</span></span>|



## <a name="response"></a><span data-ttu-id="4fbaf-166">响应</span><span class="sxs-lookup"><span data-stu-id="4fbaf-166">Response</span></span>
<span data-ttu-id="4fbaf-167">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4fbaf-168">示例</span><span class="sxs-lookup"><span data-stu-id="4fbaf-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="4fbaf-169">请求</span><span class="sxs-lookup"><span data-stu-id="4fbaf-169">Request</span></span>
<span data-ttu-id="4fbaf-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
Content-type: application/json
Content-length: 372

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1,
  "dependsOnAppCount": 1
}
```

### <a name="response"></a><span data-ttu-id="4fbaf-171">响应</span><span class="sxs-lookup"><span data-stu-id="4fbaf-171">Response</span></span>
<span data-ttu-id="4fbaf-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4fbaf-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 421

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1,
  "dependsOnAppCount": 1
}
```




