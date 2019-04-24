---
title: 创建 mobileAppDependency
description: 创建新的 mobileAppDependency 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 85aeae1d8d76b4c4609ff38f1263aaeb9a634e9f
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32489056"
---
# <a name="create-mobileappdependency"></a><span data-ttu-id="08af1-103">创建 mobileAppDependency</span><span class="sxs-lookup"><span data-stu-id="08af1-103">Create mobileAppDependency</span></span>

> <span data-ttu-id="08af1-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="08af1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08af1-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08af1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08af1-106">创建新的[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="08af1-106">Create a new [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08af1-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="08af1-107">Prerequisites</span></span>
<span data-ttu-id="08af1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08af1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08af1-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="08af1-110">Permission type</span></span>|<span data-ttu-id="08af1-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="08af1-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08af1-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08af1-112">Delegated (work or school account)</span></span>|<span data-ttu-id="08af1-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08af1-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="08af1-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08af1-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08af1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="08af1-115">Not supported.</span></span>|
|<span data-ttu-id="08af1-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="08af1-116">Application</span></span>|<span data-ttu-id="08af1-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="08af1-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="08af1-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08af1-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="08af1-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="08af1-119">Request headers</span></span>
|<span data-ttu-id="08af1-120">标头</span><span class="sxs-lookup"><span data-stu-id="08af1-120">Header</span></span>|<span data-ttu-id="08af1-121">值</span><span class="sxs-lookup"><span data-stu-id="08af1-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08af1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="08af1-122">Authorization</span></span>|<span data-ttu-id="08af1-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="08af1-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08af1-124">接受</span><span class="sxs-lookup"><span data-stu-id="08af1-124">Accept</span></span>|<span data-ttu-id="08af1-125">application/json</span><span class="sxs-lookup"><span data-stu-id="08af1-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08af1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="08af1-126">Request body</span></span>
<span data-ttu-id="08af1-127">在请求正文中, 提供 mobileAppDependency 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08af1-127">In the request body, supply a JSON representation for the mobileAppDependency object.</span></span>

<span data-ttu-id="08af1-128">下表显示创建 mobileAppDependency 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="08af1-128">The following table shows the properties that are required when you create the mobileAppDependency.</span></span>

|<span data-ttu-id="08af1-129">属性</span><span class="sxs-lookup"><span data-stu-id="08af1-129">Property</span></span>|<span data-ttu-id="08af1-130">类型</span><span class="sxs-lookup"><span data-stu-id="08af1-130">Type</span></span>|<span data-ttu-id="08af1-131">说明</span><span class="sxs-lookup"><span data-stu-id="08af1-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08af1-132">id</span><span class="sxs-lookup"><span data-stu-id="08af1-132">id</span></span>|<span data-ttu-id="08af1-133">String</span><span class="sxs-lookup"><span data-stu-id="08af1-133">String</span></span>|<span data-ttu-id="08af1-134">关系实体 id。继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="08af1-134">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="08af1-135">targetId</span><span class="sxs-lookup"><span data-stu-id="08af1-135">targetId</span></span>|<span data-ttu-id="08af1-136">字符串</span><span class="sxs-lookup"><span data-stu-id="08af1-136">String</span></span>|<span data-ttu-id="08af1-137">目标子移动应用程序的应用程序 id。继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="08af1-137">The target child mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="08af1-138">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="08af1-138">targetDisplayName</span></span>|<span data-ttu-id="08af1-139">字符串</span><span class="sxs-lookup"><span data-stu-id="08af1-139">String</span></span>|<span data-ttu-id="08af1-140">目标子移动应用程序的显示名称。</span><span class="sxs-lookup"><span data-stu-id="08af1-140">The target child mobile app's display name.</span></span> <span data-ttu-id="08af1-141">继承自[mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="08af1-141">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="08af1-142">dependencyType</span><span class="sxs-lookup"><span data-stu-id="08af1-142">dependencyType</span></span>|[<span data-ttu-id="08af1-143">mobileAppDependecyType</span><span class="sxs-lookup"><span data-stu-id="08af1-143">mobileAppDependecyType</span></span>](../resources/intune-apps-mobileappdependecytype.md)|<span data-ttu-id="08af1-144">父应用和子应用之间的依赖关系的类型。</span><span class="sxs-lookup"><span data-stu-id="08af1-144">The type of dependency relationship between the parent and child apps.</span></span> <span data-ttu-id="08af1-145">可取值为：`detect`、`autoInstall`。</span><span class="sxs-lookup"><span data-stu-id="08af1-145">Possible values are: `detect`, `autoInstall`.</span></span>|
|<span data-ttu-id="08af1-146">dependentAppCount</span><span class="sxs-lookup"><span data-stu-id="08af1-146">dependentAppCount</span></span>|<span data-ttu-id="08af1-147">Int32</span><span class="sxs-lookup"><span data-stu-id="08af1-147">Int32</span></span>|<span data-ttu-id="08af1-148">子应用程序的依赖项总数。</span><span class="sxs-lookup"><span data-stu-id="08af1-148">The total number of dependencies the child app has.</span></span>|



## <a name="response"></a><span data-ttu-id="08af1-149">响应</span><span class="sxs-lookup"><span data-stu-id="08af1-149">Response</span></span>
<span data-ttu-id="08af1-150">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[mobileAppDependency](../resources/intune-apps-mobileappdependency.md)对象。</span><span class="sxs-lookup"><span data-stu-id="08af1-150">If successful, this method returns a `201 Created` response code and a [mobileAppDependency](../resources/intune-apps-mobileappdependency.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08af1-151">示例</span><span class="sxs-lookup"><span data-stu-id="08af1-151">Example</span></span>

### <a name="request"></a><span data-ttu-id="08af1-152">请求</span><span class="sxs-lookup"><span data-stu-id="08af1-152">Request</span></span>
<span data-ttu-id="08af1-153">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="08af1-153">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="08af1-154">响应</span><span class="sxs-lookup"><span data-stu-id="08af1-154">Response</span></span>
<span data-ttu-id="08af1-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="08af1-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





