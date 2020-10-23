---
title: 更新 cartToClassAssociation
description: 更新 cartToClassAssociation 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: bc7d72d2d78046654e42007570db26eaaa10102f
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48722653"
---
# <a name="update-carttoclassassociation"></a><span data-ttu-id="884b2-103">更新 cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="884b2-103">Update cartToClassAssociation</span></span>

<span data-ttu-id="884b2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="884b2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="884b2-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="884b2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="884b2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="884b2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="884b2-107">更新 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="884b2-107">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="884b2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="884b2-108">Prerequisites</span></span>
<span data-ttu-id="884b2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="884b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="884b2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="884b2-111">Permission type</span></span>|<span data-ttu-id="884b2-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="884b2-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="884b2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="884b2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="884b2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="884b2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="884b2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="884b2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="884b2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="884b2-116">Not supported.</span></span>|
|<span data-ttu-id="884b2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="884b2-117">Application</span></span>|<span data-ttu-id="884b2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="884b2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="884b2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="884b2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="request-headers"></a><span data-ttu-id="884b2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="884b2-120">Request headers</span></span>
|<span data-ttu-id="884b2-121">标头</span><span class="sxs-lookup"><span data-stu-id="884b2-121">Header</span></span>|<span data-ttu-id="884b2-122">值</span><span class="sxs-lookup"><span data-stu-id="884b2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="884b2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="884b2-123">Authorization</span></span>|<span data-ttu-id="884b2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="884b2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="884b2-125">接受</span><span class="sxs-lookup"><span data-stu-id="884b2-125">Accept</span></span>|<span data-ttu-id="884b2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="884b2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="884b2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="884b2-127">Request body</span></span>
<span data-ttu-id="884b2-128">在请求正文中，提供 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="884b2-128">In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

<span data-ttu-id="884b2-129">下表显示创建 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="884b2-129">The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>

|<span data-ttu-id="884b2-130">属性</span><span class="sxs-lookup"><span data-stu-id="884b2-130">Property</span></span>|<span data-ttu-id="884b2-131">类型</span><span class="sxs-lookup"><span data-stu-id="884b2-131">Type</span></span>|<span data-ttu-id="884b2-132">说明</span><span class="sxs-lookup"><span data-stu-id="884b2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="884b2-133">id</span><span class="sxs-lookup"><span data-stu-id="884b2-133">id</span></span>|<span data-ttu-id="884b2-134">String</span><span class="sxs-lookup"><span data-stu-id="884b2-134">String</span></span>|<span data-ttu-id="884b2-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="884b2-135">Key of the entity.</span></span>|
|<span data-ttu-id="884b2-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="884b2-136">createdDateTime</span></span>|<span data-ttu-id="884b2-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="884b2-137">DateTimeOffset</span></span>|<span data-ttu-id="884b2-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="884b2-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="884b2-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="884b2-139">lastModifiedDateTime</span></span>|<span data-ttu-id="884b2-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="884b2-140">DateTimeOffset</span></span>|<span data-ttu-id="884b2-141">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="884b2-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="884b2-142">version</span><span class="sxs-lookup"><span data-stu-id="884b2-142">version</span></span>|<span data-ttu-id="884b2-143">Int32</span><span class="sxs-lookup"><span data-stu-id="884b2-143">Int32</span></span>|<span data-ttu-id="884b2-144">CartToClassAssociation 的版本。</span><span class="sxs-lookup"><span data-stu-id="884b2-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="884b2-145">displayName</span><span class="sxs-lookup"><span data-stu-id="884b2-145">displayName</span></span>|<span data-ttu-id="884b2-146">String</span><span class="sxs-lookup"><span data-stu-id="884b2-146">String</span></span>|<span data-ttu-id="884b2-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="884b2-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="884b2-148">说明</span><span class="sxs-lookup"><span data-stu-id="884b2-148">description</span></span>|<span data-ttu-id="884b2-149">String</span><span class="sxs-lookup"><span data-stu-id="884b2-149">String</span></span>|<span data-ttu-id="884b2-150">管理员提供的 CartToClassAssociation 说明。</span><span class="sxs-lookup"><span data-stu-id="884b2-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="884b2-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="884b2-151">deviceCartIds</span></span>|<span data-ttu-id="884b2-152">String collection</span><span class="sxs-lookup"><span data-stu-id="884b2-152">String collection</span></span>|<span data-ttu-id="884b2-153">要与类关联的设备购物车的标识符。</span><span class="sxs-lookup"><span data-stu-id="884b2-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="884b2-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="884b2-154">classroomIds</span></span>|<span data-ttu-id="884b2-155">String collection</span><span class="sxs-lookup"><span data-stu-id="884b2-155">String collection</span></span>|<span data-ttu-id="884b2-156">要与设备购物车关联的教室的标识符。</span><span class="sxs-lookup"><span data-stu-id="884b2-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="884b2-157">响应</span><span class="sxs-lookup"><span data-stu-id="884b2-157">Response</span></span>
<span data-ttu-id="884b2-158">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="884b2-158">If successful, this method returns a `200 OK` response code and an updated [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="884b2-159">示例</span><span class="sxs-lookup"><span data-stu-id="884b2-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="884b2-160">请求</span><span class="sxs-lookup"><span data-stu-id="884b2-160">Request</span></span>
<span data-ttu-id="884b2-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="884b2-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="884b2-162">响应</span><span class="sxs-lookup"><span data-stu-id="884b2-162">Response</span></span>
<span data-ttu-id="884b2-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="884b2-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





