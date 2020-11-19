---
title: 更新 cartToClassAssociation
description: 更新 cartToClassAssociation 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 05e0777ff3a1e576fa5cf574721fec8f45f03672
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49265330"
---
# <a name="update-carttoclassassociation"></a><span data-ttu-id="27417-103">更新 cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="27417-103">Update cartToClassAssociation</span></span>

<span data-ttu-id="27417-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="27417-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="27417-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="27417-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="27417-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="27417-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="27417-107">更新 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="27417-107">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="27417-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="27417-108">Prerequisites</span></span>
<span data-ttu-id="27417-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="27417-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="27417-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="27417-111">Permission type</span></span>|<span data-ttu-id="27417-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="27417-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="27417-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="27417-113">Delegated (work or school account)</span></span>|<span data-ttu-id="27417-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27417-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="27417-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="27417-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="27417-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="27417-116">Not supported.</span></span>|
|<span data-ttu-id="27417-117">Application</span><span class="sxs-lookup"><span data-stu-id="27417-117">Application</span></span>|<span data-ttu-id="27417-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="27417-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="27417-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="27417-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="request-headers"></a><span data-ttu-id="27417-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="27417-120">Request headers</span></span>
|<span data-ttu-id="27417-121">标头</span><span class="sxs-lookup"><span data-stu-id="27417-121">Header</span></span>|<span data-ttu-id="27417-122">值</span><span class="sxs-lookup"><span data-stu-id="27417-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="27417-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="27417-123">Authorization</span></span>|<span data-ttu-id="27417-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="27417-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="27417-125">接受</span><span class="sxs-lookup"><span data-stu-id="27417-125">Accept</span></span>|<span data-ttu-id="27417-126">application/json</span><span class="sxs-lookup"><span data-stu-id="27417-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="27417-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="27417-127">Request body</span></span>
<span data-ttu-id="27417-128">在请求正文中，提供 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="27417-128">In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

<span data-ttu-id="27417-129">下表显示创建 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="27417-129">The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>

|<span data-ttu-id="27417-130">属性</span><span class="sxs-lookup"><span data-stu-id="27417-130">Property</span></span>|<span data-ttu-id="27417-131">类型</span><span class="sxs-lookup"><span data-stu-id="27417-131">Type</span></span>|<span data-ttu-id="27417-132">说明</span><span class="sxs-lookup"><span data-stu-id="27417-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="27417-133">id</span><span class="sxs-lookup"><span data-stu-id="27417-133">id</span></span>|<span data-ttu-id="27417-134">字符串</span><span class="sxs-lookup"><span data-stu-id="27417-134">String</span></span>|<span data-ttu-id="27417-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="27417-135">Key of the entity.</span></span>|
|<span data-ttu-id="27417-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="27417-136">createdDateTime</span></span>|<span data-ttu-id="27417-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27417-137">DateTimeOffset</span></span>|<span data-ttu-id="27417-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="27417-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="27417-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="27417-139">lastModifiedDateTime</span></span>|<span data-ttu-id="27417-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="27417-140">DateTimeOffset</span></span>|<span data-ttu-id="27417-141">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="27417-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="27417-142">version</span><span class="sxs-lookup"><span data-stu-id="27417-142">version</span></span>|<span data-ttu-id="27417-143">Int32</span><span class="sxs-lookup"><span data-stu-id="27417-143">Int32</span></span>|<span data-ttu-id="27417-144">CartToClassAssociation 的版本。</span><span class="sxs-lookup"><span data-stu-id="27417-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="27417-145">displayName</span><span class="sxs-lookup"><span data-stu-id="27417-145">displayName</span></span>|<span data-ttu-id="27417-146">字符串</span><span class="sxs-lookup"><span data-stu-id="27417-146">String</span></span>|<span data-ttu-id="27417-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="27417-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="27417-148">description</span><span class="sxs-lookup"><span data-stu-id="27417-148">description</span></span>|<span data-ttu-id="27417-149">字符串</span><span class="sxs-lookup"><span data-stu-id="27417-149">String</span></span>|<span data-ttu-id="27417-150">管理员提供的 CartToClassAssociation 说明。</span><span class="sxs-lookup"><span data-stu-id="27417-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="27417-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="27417-151">deviceCartIds</span></span>|<span data-ttu-id="27417-152">String 集合</span><span class="sxs-lookup"><span data-stu-id="27417-152">String collection</span></span>|<span data-ttu-id="27417-153">要与类关联的设备购物车的标识符。</span><span class="sxs-lookup"><span data-stu-id="27417-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="27417-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="27417-154">classroomIds</span></span>|<span data-ttu-id="27417-155">String 集合</span><span class="sxs-lookup"><span data-stu-id="27417-155">String collection</span></span>|<span data-ttu-id="27417-156">要与设备购物车关联的教室的标识符。</span><span class="sxs-lookup"><span data-stu-id="27417-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="27417-157">响应</span><span class="sxs-lookup"><span data-stu-id="27417-157">Response</span></span>
<span data-ttu-id="27417-158">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="27417-158">If successful, this method returns a `200 OK` response code and an updated [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="27417-159">示例</span><span class="sxs-lookup"><span data-stu-id="27417-159">Example</span></span>

### <a name="request"></a><span data-ttu-id="27417-160">请求</span><span class="sxs-lookup"><span data-stu-id="27417-160">Request</span></span>
<span data-ttu-id="27417-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="27417-161">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="27417-162">响应</span><span class="sxs-lookup"><span data-stu-id="27417-162">Response</span></span>
<span data-ttu-id="27417-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="27417-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




