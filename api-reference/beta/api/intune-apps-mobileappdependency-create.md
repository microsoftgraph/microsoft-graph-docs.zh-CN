---
title: 创建 mobileAppDependency
description: 创建新的 mobileAppDependency 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: be92f602287c16e3481dcfafe9f38c2bff8a26ee
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47977297"
---
# <a name="create-mobileappdependency"></a><span data-ttu-id="b21d1-103">创建 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="b21d1-103">Create mobileAppDependency</span></span>

<span data-ttu-id="b21d1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b21d1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b21d1-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b21d1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b21d1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b21d1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b21d1-107">创建新的 [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b21d1-107">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b21d1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b21d1-108">Prerequisites</span></span>
<span data-ttu-id="b21d1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b21d1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b21d1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b21d1-111">Permission type</span></span>|<span data-ttu-id="b21d1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b21d1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b21d1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b21d1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b21d1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b21d1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b21d1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b21d1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b21d1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b21d1-116">Not supported.</span></span>|
|<span data-ttu-id="b21d1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b21d1-117">Application</span></span>|<span data-ttu-id="b21d1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b21d1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b21d1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b21d1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="b21d1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b21d1-120">Request headers</span></span>
|<span data-ttu-id="b21d1-121">标头</span><span class="sxs-lookup"><span data-stu-id="b21d1-121">Header</span></span>|<span data-ttu-id="b21d1-122">值</span><span class="sxs-lookup"><span data-stu-id="b21d1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b21d1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b21d1-123">Authorization</span></span>|<span data-ttu-id="b21d1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b21d1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b21d1-125">接受</span><span class="sxs-lookup"><span data-stu-id="b21d1-125">Accept</span></span>|<span data-ttu-id="b21d1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b21d1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b21d1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b21d1-127">Request body</span></span>
<span data-ttu-id="b21d1-128">在请求正文中，提供 mobileAppDependency 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b21d1-128">In the request body, supply a JSON representation for the mobileAppDependency object.</span></span>

<span data-ttu-id="b21d1-129">下表显示创建 mobileAppDependency 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b21d1-129">The following table shows the properties that are required when you create the mobileAppDependency.</span></span>

|<span data-ttu-id="b21d1-130">属性</span><span class="sxs-lookup"><span data-stu-id="b21d1-130">Property</span></span>|<span data-ttu-id="b21d1-131">类型</span><span class="sxs-lookup"><span data-stu-id="b21d1-131">Type</span></span>|<span data-ttu-id="b21d1-132">说明</span><span class="sxs-lookup"><span data-stu-id="b21d1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b21d1-133">id</span><span class="sxs-lookup"><span data-stu-id="b21d1-133">id</span></span>|<span data-ttu-id="b21d1-134">String</span><span class="sxs-lookup"><span data-stu-id="b21d1-134">String</span></span>|<span data-ttu-id="b21d1-135">关系实体 id。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="b21d1-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="b21d1-136">targetId</span><span class="sxs-lookup"><span data-stu-id="b21d1-136">targetId</span></span>|<span data-ttu-id="b21d1-137">String</span><span class="sxs-lookup"><span data-stu-id="b21d1-137">String</span></span>|<span data-ttu-id="b21d1-138">目标移动应用程序的应用程序 id。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="b21d1-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="b21d1-139">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="b21d1-139">targetDisplayName</span></span>|<span data-ttu-id="b21d1-140">String</span><span class="sxs-lookup"><span data-stu-id="b21d1-140">String</span></span>|<span data-ttu-id="b21d1-141">目标移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="b21d1-141">The target mobile app's display name.</span></span> <span data-ttu-id="b21d1-142">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="b21d1-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="b21d1-143">targetType</span><span class="sxs-lookup"><span data-stu-id="b21d1-143">targetType</span></span>|[<span data-ttu-id="b21d1-144">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="b21d1-144">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="b21d1-145">表示目标是父项还是子项的关系的类型。</span><span class="sxs-lookup"><span data-stu-id="b21d1-145">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="b21d1-146">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)。</span><span class="sxs-lookup"><span data-stu-id="b21d1-146">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="b21d1-147">可取值为：`child`、`parent`。</span><span class="sxs-lookup"><span data-stu-id="b21d1-147">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="b21d1-148">dependencyType</span><span class="sxs-lookup"><span data-stu-id="b21d1-148">dependencyType</span></span>|[<span data-ttu-id="b21d1-149">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="b21d1-149">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="b21d1-150">父应用和子应用之间的依赖关系的类型。</span><span class="sxs-lookup"><span data-stu-id="b21d1-150">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="b21d1-151">可取值为：`detect`、`autoInstall`。</span><span class="sxs-lookup"><span data-stu-id="b21d1-151">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="b21d1-152">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="b21d1-152">dependentAppCount</span></span>|<span data-ttu-id="b21d1-153">Int32</span><span class="sxs-lookup"><span data-stu-id="b21d1-153">Int32</span></span>|<span data-ttu-id="b21d1-154">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="b21d1-154">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="b21d1-155">响应</span><span class="sxs-lookup"><span data-stu-id="b21d1-155">Response</span></span>
<span data-ttu-id="b21d1-156">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b21d1-156">If successful, this method returns a `201 Created` response code and a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b21d1-157">示例</span><span class="sxs-lookup"><span data-stu-id="b21d1-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="b21d1-158">请求</span><span class="sxs-lookup"><span data-stu-id="b21d1-158">Request</span></span>
<span data-ttu-id="b21d1-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b21d1-159">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
Content-type: application/json
Content-length: 238

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetType": "parent",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```

### <a name="response"></a><span data-ttu-id="b21d1-160">响应</span><span class="sxs-lookup"><span data-stu-id="b21d1-160">Response</span></span>
<span data-ttu-id="b21d1-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b21d1-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 287

{
  "@odata.type": "#microsoft.graph.mobileAppDependency",
  "id": "c7f6f9ab-f9ab-c7f6-abf9-f6c7abf9f6c7",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetType": "parent",
  "dependencyType": "autoInstall",
  "dependentAppCount": 1
}
```






