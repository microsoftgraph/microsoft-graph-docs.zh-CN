---
title: 创建 cartToClassAssociation
description: 创建新的 cartToClassAssociation 对象。
author: davidmu1
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: abfd05152a968696e4f35879e7cd5a8bb957bc2f
ms.sourcegitcommit: b38fd4c8c734243f6f82448045a1f6bf63311ec9
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/18/2020
ms.locfileid: "42756987"
---
# <a name="create-carttoclassassociation"></a><span data-ttu-id="b8020-103">创建 cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="b8020-103">Create cartToClassAssociation</span></span>

> <span data-ttu-id="b8020-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b8020-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b8020-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b8020-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b8020-106">创建新的[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b8020-106">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b8020-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="b8020-107">Prerequisites</span></span>
<span data-ttu-id="b8020-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b8020-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b8020-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b8020-110">Permission type</span></span>|<span data-ttu-id="b8020-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b8020-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b8020-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b8020-112">Delegated (work or school account)</span></span>|<span data-ttu-id="b8020-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8020-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b8020-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b8020-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b8020-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="b8020-115">Not supported.</span></span>|
|<span data-ttu-id="b8020-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b8020-116">Application</span></span>|<span data-ttu-id="b8020-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b8020-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b8020-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b8020-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="b8020-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b8020-119">Request headers</span></span>
|<span data-ttu-id="b8020-120">标头</span><span class="sxs-lookup"><span data-stu-id="b8020-120">Header</span></span>|<span data-ttu-id="b8020-121">值</span><span class="sxs-lookup"><span data-stu-id="b8020-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b8020-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b8020-122">Authorization</span></span>|<span data-ttu-id="b8020-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b8020-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b8020-124">接受</span><span class="sxs-lookup"><span data-stu-id="b8020-124">Accept</span></span>|<span data-ttu-id="b8020-125">application/json</span><span class="sxs-lookup"><span data-stu-id="b8020-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b8020-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b8020-126">Request body</span></span>
<span data-ttu-id="b8020-127">在请求正文中，提供 cartToClassAssociation 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b8020-127">In the request body, supply a JSON representation for the cartToClassAssociation object.</span></span>

<span data-ttu-id="b8020-128">下表显示创建 cartToClassAssociation 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b8020-128">The following table shows the properties that are required when you create the cartToClassAssociation.</span></span>

|<span data-ttu-id="b8020-129">属性</span><span class="sxs-lookup"><span data-stu-id="b8020-129">Property</span></span>|<span data-ttu-id="b8020-130">类型</span><span class="sxs-lookup"><span data-stu-id="b8020-130">Type</span></span>|<span data-ttu-id="b8020-131">说明</span><span class="sxs-lookup"><span data-stu-id="b8020-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b8020-132">id</span><span class="sxs-lookup"><span data-stu-id="b8020-132">id</span></span>|<span data-ttu-id="b8020-133">字符串</span><span class="sxs-lookup"><span data-stu-id="b8020-133">String</span></span>|<span data-ttu-id="b8020-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b8020-134">Key of the entity.</span></span>|
|<span data-ttu-id="b8020-135">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b8020-135">createdDateTime</span></span>|<span data-ttu-id="b8020-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8020-136">DateTimeOffset</span></span>|<span data-ttu-id="b8020-137">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b8020-137">DateTime the object was created.</span></span>|
|<span data-ttu-id="b8020-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b8020-138">lastModifiedDateTime</span></span>|<span data-ttu-id="b8020-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b8020-139">DateTimeOffset</span></span>|<span data-ttu-id="b8020-140">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="b8020-140">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="b8020-141">version</span><span class="sxs-lookup"><span data-stu-id="b8020-141">version</span></span>|<span data-ttu-id="b8020-142">Int32</span><span class="sxs-lookup"><span data-stu-id="b8020-142">Int32</span></span>|<span data-ttu-id="b8020-143">CartToClassAssociation 的版本。</span><span class="sxs-lookup"><span data-stu-id="b8020-143">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="b8020-144">displayName</span><span class="sxs-lookup"><span data-stu-id="b8020-144">displayName</span></span>|<span data-ttu-id="b8020-145">String</span><span class="sxs-lookup"><span data-stu-id="b8020-145">String</span></span>|<span data-ttu-id="b8020-146">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="b8020-146">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="b8020-147">说明</span><span class="sxs-lookup"><span data-stu-id="b8020-147">description</span></span>|<span data-ttu-id="b8020-148">String</span><span class="sxs-lookup"><span data-stu-id="b8020-148">String</span></span>|<span data-ttu-id="b8020-149">管理员提供的 CartToClassAssociation 说明。</span><span class="sxs-lookup"><span data-stu-id="b8020-149">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="b8020-150">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="b8020-150">deviceCartIds</span></span>|<span data-ttu-id="b8020-151">String collection</span><span class="sxs-lookup"><span data-stu-id="b8020-151">String collection</span></span>|<span data-ttu-id="b8020-152">要与类关联的设备购物车的标识符。</span><span class="sxs-lookup"><span data-stu-id="b8020-152">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="b8020-153">classroomIds</span><span class="sxs-lookup"><span data-stu-id="b8020-153">classroomIds</span></span>|<span data-ttu-id="b8020-154">String collection</span><span class="sxs-lookup"><span data-stu-id="b8020-154">String collection</span></span>|<span data-ttu-id="b8020-155">要与设备购物车关联的教室的标识符。</span><span class="sxs-lookup"><span data-stu-id="b8020-155">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="b8020-156">响应</span><span class="sxs-lookup"><span data-stu-id="b8020-156">Response</span></span>
<span data-ttu-id="b8020-157">如果成功，此方法在响应`201 Created`正文中返回响应代码和[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b8020-157">If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b8020-158">示例</span><span class="sxs-lookup"><span data-stu-id="b8020-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="b8020-159">请求</span><span class="sxs-lookup"><span data-stu-id="b8020-159">Request</span></span>
<span data-ttu-id="b8020-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b8020-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
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

### <a name="response"></a><span data-ttu-id="b8020-161">响应</span><span class="sxs-lookup"><span data-stu-id="b8020-161">Response</span></span>
<span data-ttu-id="b8020-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b8020-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




