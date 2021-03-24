---
title: 更新 mobileAppSupersedence
description: 更新 mobileAppSupersedence 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 0397b5a029ca848fa1cb002b0930580b3978f358
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51143036"
---
# <a name="update-mobileappsupersedence"></a><span data-ttu-id="5cd57-103">更新 mobileAppSupersedence</span><span class="sxs-lookup"><span data-stu-id="5cd57-103">Update mobileAppSupersedence</span></span>

<span data-ttu-id="5cd57-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5cd57-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="5cd57-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="5cd57-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="5cd57-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="5cd57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5cd57-107">更新 [mobileAppSupersedence 对象](../resources/intune-apps-mobileappsupersedence.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="5cd57-107">Update the properties of a [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="5cd57-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="5cd57-108">Prerequisites</span></span>
<span data-ttu-id="5cd57-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5cd57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5cd57-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="5cd57-111">Permission type</span></span>|<span data-ttu-id="5cd57-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5cd57-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5cd57-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5cd57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5cd57-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cd57-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5cd57-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5cd57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5cd57-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5cd57-116">Not supported.</span></span>|
|<span data-ttu-id="5cd57-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="5cd57-117">Application</span></span>|<span data-ttu-id="5cd57-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5cd57-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="5cd57-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5cd57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
```

## <a name="request-headers"></a><span data-ttu-id="5cd57-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="5cd57-120">Request headers</span></span>
|<span data-ttu-id="5cd57-121">标头</span><span class="sxs-lookup"><span data-stu-id="5cd57-121">Header</span></span>|<span data-ttu-id="5cd57-122">值</span><span class="sxs-lookup"><span data-stu-id="5cd57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5cd57-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5cd57-123">Authorization</span></span>|<span data-ttu-id="5cd57-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="5cd57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5cd57-125">接受</span><span class="sxs-lookup"><span data-stu-id="5cd57-125">Accept</span></span>|<span data-ttu-id="5cd57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5cd57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5cd57-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="5cd57-127">Request body</span></span>
<span data-ttu-id="5cd57-128">在请求正文中，提供 [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="5cd57-128">In the request body, supply a JSON representation for the [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object.</span></span>

<span data-ttu-id="5cd57-129">下表显示创建 [mobileAppSupersedence 时所需的属性](../resources/intune-apps-mobileappsupersedence.md)。</span><span class="sxs-lookup"><span data-stu-id="5cd57-129">The following table shows the properties that are required when you create the [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md).</span></span>

|<span data-ttu-id="5cd57-130">属性</span><span class="sxs-lookup"><span data-stu-id="5cd57-130">Property</span></span>|<span data-ttu-id="5cd57-131">类型</span><span class="sxs-lookup"><span data-stu-id="5cd57-131">Type</span></span>|<span data-ttu-id="5cd57-132">说明</span><span class="sxs-lookup"><span data-stu-id="5cd57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5cd57-133">id</span><span class="sxs-lookup"><span data-stu-id="5cd57-133">id</span></span>|<span data-ttu-id="5cd57-134">String</span><span class="sxs-lookup"><span data-stu-id="5cd57-134">String</span></span>|<span data-ttu-id="5cd57-135">关系实体 ID。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="5cd57-135">The relationship entity id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="5cd57-136">targetId</span><span class="sxs-lookup"><span data-stu-id="5cd57-136">targetId</span></span>|<span data-ttu-id="5cd57-137">String</span><span class="sxs-lookup"><span data-stu-id="5cd57-137">String</span></span>|<span data-ttu-id="5cd57-138">目标移动应用的应用 ID。继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="5cd57-138">The target mobile app's app id. Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="5cd57-139">targetDisplayName</span><span class="sxs-lookup"><span data-stu-id="5cd57-139">targetDisplayName</span></span>|<span data-ttu-id="5cd57-140">String</span><span class="sxs-lookup"><span data-stu-id="5cd57-140">String</span></span>|<span data-ttu-id="5cd57-141">目标移动应用显示名称。</span><span class="sxs-lookup"><span data-stu-id="5cd57-141">The target mobile app's display name.</span></span> <span data-ttu-id="5cd57-142">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="5cd57-142">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="5cd57-143">targetDisplayVersion</span><span class="sxs-lookup"><span data-stu-id="5cd57-143">targetDisplayVersion</span></span>|<span data-ttu-id="5cd57-144">String</span><span class="sxs-lookup"><span data-stu-id="5cd57-144">String</span></span>|<span data-ttu-id="5cd57-145">目标移动应用的显示版本。</span><span class="sxs-lookup"><span data-stu-id="5cd57-145">The target mobile app's display version.</span></span> <span data-ttu-id="5cd57-146">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="5cd57-146">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="5cd57-147">targetPublisher</span><span class="sxs-lookup"><span data-stu-id="5cd57-147">targetPublisher</span></span>|<span data-ttu-id="5cd57-148">String</span><span class="sxs-lookup"><span data-stu-id="5cd57-148">String</span></span>|<span data-ttu-id="5cd57-149">目标移动应用的发布者。</span><span class="sxs-lookup"><span data-stu-id="5cd57-149">The target mobile app's publisher.</span></span> <span data-ttu-id="5cd57-150">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span><span class="sxs-lookup"><span data-stu-id="5cd57-150">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)</span></span>|
|<span data-ttu-id="5cd57-151">targetType</span><span class="sxs-lookup"><span data-stu-id="5cd57-151">targetType</span></span>|[<span data-ttu-id="5cd57-152">mobileAppRelationshipType</span><span class="sxs-lookup"><span data-stu-id="5cd57-152">mobileAppRelationshipType</span></span>](../resources/intune-apps-mobileapprelationshiptype.md)|<span data-ttu-id="5cd57-153">关系类型，指示目标是父对象还是子级。</span><span class="sxs-lookup"><span data-stu-id="5cd57-153">The type of relationship indicating whether the target is a parent or child.</span></span> <span data-ttu-id="5cd57-154">继承自 [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md)。</span><span class="sxs-lookup"><span data-stu-id="5cd57-154">Inherited from [mobileAppRelationship](../resources/intune-apps-mobileapprelationship.md).</span></span> <span data-ttu-id="5cd57-155">可取值为：`child`、`parent`。</span><span class="sxs-lookup"><span data-stu-id="5cd57-155">Possible values are: `child`, `parent`.</span></span>|
|<span data-ttu-id="5cd57-156">supersedenceType</span><span class="sxs-lookup"><span data-stu-id="5cd57-156">supersedenceType</span></span>|[<span data-ttu-id="5cd57-157">mobileAppSupersedenceType</span><span class="sxs-lookup"><span data-stu-id="5cd57-157">mobileAppSupersedenceType</span></span>](../resources/intune-apps-mobileappsupersedencetype.md)|<span data-ttu-id="5cd57-158">父应用和子应用之间的取代关系类型。</span><span class="sxs-lookup"><span data-stu-id="5cd57-158">The supersedence relationship type between the parent and child apps.</span></span> <span data-ttu-id="5cd57-159">可取值为：`update`、`replace`。</span><span class="sxs-lookup"><span data-stu-id="5cd57-159">Possible values are: `update`, `replace`.</span></span>|
|<span data-ttu-id="5cd57-160">supersededAppCount</span><span class="sxs-lookup"><span data-stu-id="5cd57-160">supersededAppCount</span></span>|<span data-ttu-id="5cd57-161">Int32</span><span class="sxs-lookup"><span data-stu-id="5cd57-161">Int32</span></span>|<span data-ttu-id="5cd57-162">被子应用直接或间接取代的应用总数。</span><span class="sxs-lookup"><span data-stu-id="5cd57-162">The total number of apps directly or indirectly superseded by the child app.</span></span>|
|<span data-ttu-id="5cd57-163">supersedingAppCount</span><span class="sxs-lookup"><span data-stu-id="5cd57-163">supersedingAppCount</span></span>|<span data-ttu-id="5cd57-164">Int32</span><span class="sxs-lookup"><span data-stu-id="5cd57-164">Int32</span></span>|<span data-ttu-id="5cd57-165">直接或间接取代父应用的应用总数。</span><span class="sxs-lookup"><span data-stu-id="5cd57-165">The total number of apps directly or indirectly superseding the parent app.</span></span>|



## <a name="response"></a><span data-ttu-id="5cd57-166">响应</span><span class="sxs-lookup"><span data-stu-id="5cd57-166">Response</span></span>
<span data-ttu-id="5cd57-167">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5cd57-167">If successful, this method returns a `200 OK` response code and an updated [mobileAppSupersedence](../resources/intune-apps-mobileappsupersedence.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5cd57-168">示例</span><span class="sxs-lookup"><span data-stu-id="5cd57-168">Example</span></span>

### <a name="request"></a><span data-ttu-id="5cd57-169">请求</span><span class="sxs-lookup"><span data-stu-id="5cd57-169">Request</span></span>
<span data-ttu-id="5cd57-170">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="5cd57-170">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/relationships/{mobileAppRelationshipId}
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

### <a name="response"></a><span data-ttu-id="5cd57-171">响应</span><span class="sxs-lookup"><span data-stu-id="5cd57-171">Response</span></span>
<span data-ttu-id="5cd57-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="5cd57-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




