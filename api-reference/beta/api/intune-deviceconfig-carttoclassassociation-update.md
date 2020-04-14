---
title: 更新 cartToClassAssociation
description: 更新 cartToClassAssociation 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 9d0101004e2824d7a39cf479c9ace9f969c123ba
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43434378"
---
# <a name="update-carttoclassassociation"></a><span data-ttu-id="e7bab-103">更新 cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="e7bab-103">Update cartToClassAssociation</span></span>

<span data-ttu-id="e7bab-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e7bab-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="e7bab-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="e7bab-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e7bab-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="e7bab-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e7bab-107">更新[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="e7bab-107">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e7bab-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e7bab-108">Prerequisites</span></span>
<span data-ttu-id="e7bab-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e7bab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e7bab-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e7bab-111">Permission type</span></span>|<span data-ttu-id="e7bab-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e7bab-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e7bab-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e7bab-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e7bab-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7bab-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e7bab-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e7bab-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e7bab-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e7bab-116">Not supported.</span></span>|
|<span data-ttu-id="e7bab-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e7bab-117">Application</span></span>|<span data-ttu-id="e7bab-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e7bab-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="e7bab-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e7bab-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="request-headers"></a><span data-ttu-id="e7bab-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e7bab-120">Request headers</span></span>
|<span data-ttu-id="e7bab-121">标头</span><span class="sxs-lookup"><span data-stu-id="e7bab-121">Header</span></span>|<span data-ttu-id="e7bab-122">值</span><span class="sxs-lookup"><span data-stu-id="e7bab-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e7bab-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e7bab-123">Authorization</span></span>|<span data-ttu-id="e7bab-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e7bab-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e7bab-125">接受</span><span class="sxs-lookup"><span data-stu-id="e7bab-125">Accept</span></span>|<span data-ttu-id="e7bab-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e7bab-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e7bab-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e7bab-127">Request body</span></span>
<span data-ttu-id="e7bab-128">在请求正文中，提供[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e7bab-128">In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

<span data-ttu-id="e7bab-129">下表显示创建[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e7bab-129">The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>

|<span data-ttu-id="e7bab-130">属性</span><span class="sxs-lookup"><span data-stu-id="e7bab-130">Property</span></span>|<span data-ttu-id="e7bab-131">类型</span><span class="sxs-lookup"><span data-stu-id="e7bab-131">Type</span></span>|<span data-ttu-id="e7bab-132">说明</span><span class="sxs-lookup"><span data-stu-id="e7bab-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e7bab-133">id</span><span class="sxs-lookup"><span data-stu-id="e7bab-133">id</span></span>|<span data-ttu-id="e7bab-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e7bab-134">String</span></span>|<span data-ttu-id="e7bab-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="e7bab-135">Key of the entity.</span></span>|
|<span data-ttu-id="e7bab-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e7bab-136">createdDateTime</span></span>|<span data-ttu-id="e7bab-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7bab-137">DateTimeOffset</span></span>|<span data-ttu-id="e7bab-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e7bab-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="e7bab-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e7bab-139">lastModifiedDateTime</span></span>|<span data-ttu-id="e7bab-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e7bab-140">DateTimeOffset</span></span>|<span data-ttu-id="e7bab-141">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="e7bab-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="e7bab-142">version</span><span class="sxs-lookup"><span data-stu-id="e7bab-142">version</span></span>|<span data-ttu-id="e7bab-143">Int32</span><span class="sxs-lookup"><span data-stu-id="e7bab-143">Int32</span></span>|<span data-ttu-id="e7bab-144">CartToClassAssociation 的版本。</span><span class="sxs-lookup"><span data-stu-id="e7bab-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="e7bab-145">displayName</span><span class="sxs-lookup"><span data-stu-id="e7bab-145">displayName</span></span>|<span data-ttu-id="e7bab-146">String</span><span class="sxs-lookup"><span data-stu-id="e7bab-146">String</span></span>|<span data-ttu-id="e7bab-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="e7bab-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="e7bab-148">description</span><span class="sxs-lookup"><span data-stu-id="e7bab-148">description</span></span>|<span data-ttu-id="e7bab-149">String</span><span class="sxs-lookup"><span data-stu-id="e7bab-149">String</span></span>|<span data-ttu-id="e7bab-150">管理员提供的 CartToClassAssociation 说明。</span><span class="sxs-lookup"><span data-stu-id="e7bab-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="e7bab-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="e7bab-151">deviceCartIds</span></span>|<span data-ttu-id="e7bab-152">String 集合</span><span class="sxs-lookup"><span data-stu-id="e7bab-152">String collection</span></span>|<span data-ttu-id="e7bab-153">要与类关联的设备购物车的标识符。</span><span class="sxs-lookup"><span data-stu-id="e7bab-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="e7bab-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="e7bab-154">classroomIds</span></span>|<span data-ttu-id="e7bab-155">String 集合</span><span class="sxs-lookup"><span data-stu-id="e7bab-155">String collection</span></span>|<span data-ttu-id="e7bab-156">要与设备购物车关联的教室的标识符。</span><span class="sxs-lookup"><span data-stu-id="e7bab-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="e7bab-157">响应</span><span class="sxs-lookup"><span data-stu-id="e7bab-157">Response</span></span>
<span data-ttu-id="e7bab-158">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e7bab-158">If successful, this method returns a `200 OK` response code and an updated [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e7bab-159">示例</span><span class="sxs-lookup"><span data-stu-id="e7bab-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="e7bab-160">请求</span><span class="sxs-lookup"><span data-stu-id="e7bab-160">Request</span></span>
<span data-ttu-id="e7bab-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e7bab-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
Content-type: application/json
Content-length: 271

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="e7bab-162">响应</span><span class="sxs-lookup"><span data-stu-id="e7bab-162">Response</span></span>
<span data-ttu-id="e7bab-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e7bab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 443

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
  "id": "9bdc58dd-58dd-9bdc-dd58-dc9bdd58dc9b",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "version": 7,
  "displayName": "Display Name value",
  "description": "Description value",
  "deviceCartIds": [
    "Device Cart Ids value"
  ],
  "classroomIds": [
    "Classroom Ids value"
  ]
}
```



