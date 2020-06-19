---
title: 创建 mobileAppDependency
description: 创建新的 mobileAppDependency 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 7e2b493c7ca3201be4ac765add8877c176824d36
ms.sourcegitcommit: 0be363e309fa40f1fbb2de85b3b559105b178c0c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/18/2020
ms.locfileid: "44793309"
---
# <a name="create-mobileappdependency"></a><span data-ttu-id="47d5a-103">创建 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="47d5a-103">Create mobileAppDependency</span></span>

<span data-ttu-id="47d5a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="47d5a-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="47d5a-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="47d5a-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="47d5a-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="47d5a-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="47d5a-107">创建新的[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="47d5a-107">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="47d5a-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="47d5a-108">Prerequisites</span></span>
<span data-ttu-id="47d5a-109">One of the following permissions is required to call this API.</span><span class="sxs-lookup"><span data-stu-id="47d5a-109">One of the following permissions is required to call this API.</span></span> <span data-ttu-id="47d5a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span><span class="sxs-lookup"><span data-stu-id="47d5a-110">To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="47d5a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="47d5a-111">Permission type</span></span>|<span data-ttu-id="47d5a-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="47d5a-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="47d5a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="47d5a-113">Delegated (work or school account)</span></span>|<span data-ttu-id="47d5a-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47d5a-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="47d5a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="47d5a-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="47d5a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="47d5a-116">Not supported.</span></span>|
|<span data-ttu-id="47d5a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="47d5a-117">Application</span></span>|<span data-ttu-id="47d5a-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="47d5a-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="47d5a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="47d5a-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="47d5a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="47d5a-120">Request headers</span></span>
|<span data-ttu-id="47d5a-121">标头</span><span class="sxs-lookup"><span data-stu-id="47d5a-121">Header</span></span>|<span data-ttu-id="47d5a-122">值</span><span class="sxs-lookup"><span data-stu-id="47d5a-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="47d5a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="47d5a-123">Authorization</span></span>|<span data-ttu-id="47d5a-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="47d5a-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="47d5a-125">接受</span><span class="sxs-lookup"><span data-stu-id="47d5a-125">Accept</span></span>|<span data-ttu-id="47d5a-126">application/json</span><span class="sxs-lookup"><span data-stu-id="47d5a-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="47d5a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="47d5a-127">Request body</span></span>
<span data-ttu-id="47d5a-128">在请求正文中，提供 mobileAppDependency 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="47d5a-128">In the request body, supply a JSON representation for the mobileAppDependency object.</span></span>

<span data-ttu-id="47d5a-129">下表显示创建 mobileAppDependency 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="47d5a-129">The following table shows the properties that are required when you create the mobileAppDependency.</span></span>

|<span data-ttu-id="47d5a-130">属性</span><span class="sxs-lookup"><span data-stu-id="47d5a-130">Property</span></span>|<span data-ttu-id="47d5a-131">类型</span><span class="sxs-lookup"><span data-stu-id="47d5a-131">Type</span></span>|<span data-ttu-id="47d5a-132">说明</span><span class="sxs-lookup"><span data-stu-id="47d5a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="47d5a-133">id</span><span class="sxs-lookup"><span data-stu-id="47d5a-133">id</span></span>|<span data-ttu-id="47d5a-134">String</span><span class="sxs-lookup"><span data-stu-id="47d5a-134">String</span></span>|<span data-ttu-id="47d5a-135">关系实体 id。继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="47d5a-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="47d5a-136">targetId</span><span class="sxs-lookup"><span data-stu-id="47d5a-136">targetId</span></span>|<span data-ttu-id="47d5a-137">String</span><span class="sxs-lookup"><span data-stu-id="47d5a-137">String</span></span>|<span data-ttu-id="47d5a-138">目标移动应用程序的应用程序 id。继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="47d5a-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="47d5a-139">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="47d5a-139">targetDisplayName</span></span>|<span data-ttu-id="47d5a-140">String</span><span class="sxs-lookup"><span data-stu-id="47d5a-140">String</span></span>|<span data-ttu-id="47d5a-141">目标移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="47d5a-141">The target mobile app's display name.</span></span> <span data-ttu-id="47d5a-142">继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="47d5a-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="47d5a-143">dependencyType</span><span class="sxs-lookup"><span data-stu-id="47d5a-143">dependencyType</span></span>|[<span data-ttu-id="47d5a-144">mobileAppDependencyType</span><span class="sxs-lookup"><span data-stu-id="47d5a-144">mobileAppDependencyType</span></span>](../resources/intune-apps-mobileappdependencytype.md)|<span data-ttu-id="47d5a-145">父应用和子应用之间的依赖关系的类型。</span><span class="sxs-lookup"><span data-stu-id="47d5a-145">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="47d5a-146">可取值为：`detect`、`autoInstall`。</span><span class="sxs-lookup"><span data-stu-id="47d5a-146">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="47d5a-147">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="47d5a-147">dependentAppCount</span></span>|<span data-ttu-id="47d5a-148">Int32</span><span class="sxs-lookup"><span data-stu-id="47d5a-148">Int32</span></span>|<span data-ttu-id="47d5a-149">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="47d5a-149">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="47d5a-150">响应</span><span class="sxs-lookup"><span data-stu-id="47d5a-150">Response</span></span>
<span data-ttu-id="47d5a-151">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="47d5a-151">If successful, this method returns a `201 Created` response code and a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="47d5a-152">示例</span><span class="sxs-lookup"><span data-stu-id="47d5a-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="47d5a-153">请求</span><span class="sxs-lookup"><span data-stu-id="47d5a-153">Request</span></span>
<span data-ttu-id="47d5a-154">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="47d5a-154">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
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

### <a name="response"></a><span data-ttu-id="47d5a-155">响应</span><span class="sxs-lookup"><span data-stu-id="47d5a-155">Response</span></span>
<span data-ttu-id="47d5a-156">Here is an example of the response.</span><span class="sxs-lookup"><span data-stu-id="47d5a-156">Here is an example of the response.</span></span> <span data-ttu-id="47d5a-157">Note: The response object shown here may be truncated for brevity.</span><span class="sxs-lookup"><span data-stu-id="47d5a-157">Note: The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="47d5a-158">All of the properties will be returned from an actual call.</span><span class="sxs-lookup"><span data-stu-id="47d5a-158">All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



