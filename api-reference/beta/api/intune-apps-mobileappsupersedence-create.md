---
title: 创建 mobileAppSupersedence
description: 创建新的 mobileAppSupersedence 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 02410619b871c00b92bfacd8df09ff221baff68e
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143092"
---
# <a name="create-mobileappsupersedence"></a><span data-ttu-id="60c35-103">创建 mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="60c35-103">Create mobileAppSupersedence</span></span>

<span data-ttu-id="60c35-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="60c35-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="60c35-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="60c35-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60c35-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="60c35-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60c35-107">创建新的 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60c35-107">Create a new [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60c35-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="60c35-108">Prerequisites</span></span>
<span data-ttu-id="60c35-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60c35-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60c35-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="60c35-111">Permission type</span></span>|<span data-ttu-id="60c35-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="60c35-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60c35-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60c35-113">Delegated (work or school account)</span></span>|<span data-ttu-id="60c35-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60c35-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="60c35-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60c35-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60c35-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="60c35-116">Not supported.</span></span>|
|<span data-ttu-id="60c35-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="60c35-117">Application</span></span>|<span data-ttu-id="60c35-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60c35-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="60c35-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60c35-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/relationships
```

## <a name="request-headers"></a><span data-ttu-id="60c35-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="60c35-120">Request headers</span></span>
|<span data-ttu-id="60c35-121">标头</span><span class="sxs-lookup"><span data-stu-id="60c35-121">Header</span></span>|<span data-ttu-id="60c35-122">值</span><span class="sxs-lookup"><span data-stu-id="60c35-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60c35-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="60c35-123">Authorization</span></span>|<span data-ttu-id="60c35-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="60c35-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60c35-125">接受</span><span class="sxs-lookup"><span data-stu-id="60c35-125">Accept</span></span>|<span data-ttu-id="60c35-126">application/json</span><span class="sxs-lookup"><span data-stu-id="60c35-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60c35-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="60c35-127">Request body</span></span>
<span data-ttu-id="60c35-128">在请求正文中，提供 mobileAppSupersedence 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60c35-128">In the request body, supply a JSON representation for the mobileAppSupersedence object.</span></span>

<span data-ttu-id="60c35-129">下表显示创建 mobileAppSupersedence 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="60c35-129">The following table shows the properties that are required when you create the mobileAppSupersedence.</span></span>

|<span data-ttu-id="60c35-130">属性</span><span class="sxs-lookup"><span data-stu-id="60c35-130">Property</span></span>|<span data-ttu-id="60c35-131">类型</span><span class="sxs-lookup"><span data-stu-id="60c35-131">Type</span></span>|<span data-ttu-id="60c35-132">说明</span><span class="sxs-lookup"><span data-stu-id="60c35-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60c35-133">id</span><span class="sxs-lookup"><span data-stu-id="60c35-133">id</span></span>|<span data-ttu-id="60c35-134">String</span><span class="sxs-lookup"><span data-stu-id="60c35-134">String</span></span>|<span data-ttu-id="60c35-135">关系实体 ID。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="60c35-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="60c35-136">targetId</span><span class="sxs-lookup"><span data-stu-id="60c35-136">targetId</span></span>|<span data-ttu-id="60c35-137">String</span><span class="sxs-lookup"><span data-stu-id="60c35-137">String</span></span>|<span data-ttu-id="60c35-138">目标移动应用的应用 ID。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="60c35-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="60c35-139">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="60c35-139">targetDisplayName</span></span>|<span data-ttu-id="60c35-140">String</span><span class="sxs-lookup"><span data-stu-id="60c35-140">String</span></span>|<span data-ttu-id="60c35-141">目标移动应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="60c35-141">The target mobile app's display name.</span></span> <span data-ttu-id="60c35-142">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="60c35-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="60c35-143">targetDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="60c35-143">targetDisplayVersion</span></span>|<span data-ttu-id="60c35-144">String</span><span class="sxs-lookup"><span data-stu-id="60c35-144">String</span></span>|<span data-ttu-id="60c35-145">目标移动应用的显示版本。</span><span class="sxs-lookup"><span data-stu-id="60c35-145">The target mobile app's display version.</span></span> <span data-ttu-id="60c35-146">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="60c35-146">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="60c35-147">targetPublisher</span><span class="sxs-lookup"><span data-stu-id="60c35-147">targetPublisher</span></span>|<span data-ttu-id="60c35-148">String</span><span class="sxs-lookup"><span data-stu-id="60c35-148">String</span></span>|<span data-ttu-id="60c35-149">目标移动应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="60c35-149">The target mobile app's publisher.</span></span> <span data-ttu-id="60c35-150">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="60c35-150">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="60c35-151">targetType</span><span class="sxs-lookup"><span data-stu-id="60c35-151">targetType</span></span>|[<span data-ttu-id="60c35-152">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="60c35-152">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="60c35-153">关系类型，指示目标是父对象还是子级。</span><span class="sxs-lookup"><span data-stu-id="60c35-153">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="60c35-154">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)。</span><span class="sxs-lookup"><span data-stu-id="60c35-154">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="60c35-155">可取值为：`child`、`parent`。</span><span class="sxs-lookup"><span data-stu-id="60c35-155">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="60c35-156">supersedenceType</span><span class="sxs-lookup"><span data-stu-id="60c35-156">supersedenceType</span></span>|[<span data-ttu-id="60c35-157">mobileAppSupersedenceType</span><span class="sxs-lookup"><span data-stu-id="60c35-157">mobileAppSupersedenceType</span></span>](../resources/intune-apps-mobileappsupersedencetype.md)|<span data-ttu-id="60c35-158">父应用和子应用之间的取代关系类型。</span><span class="sxs-lookup"><span data-stu-id="60c35-158">The supersedence relationship type between the parent and child apps.</span></span> <span data-ttu-id="60c35-159">可取值为：`update`、`replace`。</span><span class="sxs-lookup"><span data-stu-id="60c35-159">Possible values are: `update`, `replace`.</span></span>|
|<span data-ttu-id="60c35-160">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="60c35-160">supersededAppCount</span></span>|<span data-ttu-id="60c35-161">Int32</span><span class="sxs-lookup"><span data-stu-id="60c35-161">Int32</span></span>|<span data-ttu-id="60c35-162">被子应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="60c35-162">The total number of apps directly or indirectly superseded by the child app.</span></span>|
|<span data-ttu-id="60c35-163">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="60c35-163">supersedingAppCount</span></span>|<span data-ttu-id="60c35-164">Int32</span><span class="sxs-lookup"><span data-stu-id="60c35-164">Int32</span></span>|<span data-ttu-id="60c35-165">直接或间接取代父应用的应用总数。</span><span class="sxs-lookup"><span data-stu-id="60c35-165">The total number of apps directly or indirectly superseding the parent app.</span></span>|



## <a name="response"></a><span data-ttu-id="60c35-166">响应</span><span class="sxs-lookup"><span data-stu-id="60c35-166">Response</span></span>
<span data-ttu-id="60c35-167">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="60c35-167">If successful, this method returns a `201 Created` response code and a [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60c35-168">示例</span><span class="sxs-lookup"><span data-stu-id="60c35-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="60c35-169">请求</span><span class="sxs-lookup"><span data-stu-id="60c35-169">Request</span></span>
<span data-ttu-id="60c35-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="60c35-170">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships
Content-type: application/json
Content-length: 375

{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "supersedenceType": "replace",
  "supersededAppCount": 2,
  "supersedingAppCount": 3
}
```

### <a name="response"></a><span data-ttu-id="60c35-171">响应</span><span class="sxs-lookup"><span data-stu-id="60c35-171">Response</span></span>
<span data-ttu-id="60c35-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="60c35-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 424

{
  "@odata.type": "#microsoft.graph.mobileAppSupersedence",
  "id": "c0254204-4204-c025-0442-25c0044225c0",
  "targetId": "Target Id value",
  "targetDisplayName": "Target Display Name value",
  "targetDisplayVersion": "Target Display Version value",
  "targetPublisher": "Target Publisher value",
  "targetType": "parent",
  "supersedenceType": "replace",
  "supersededAppCount": 2,
  "supersedingAppCount": 3
}
```




