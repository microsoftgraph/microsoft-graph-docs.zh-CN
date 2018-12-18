---
title: 创建 cartToClassAssociation
description: 创建新的 cartToClassAssociation 对象。
author: tfitzmac
ms.openlocfilehash: 3ed7ef088acca7908ece1e0b5e61797bb54a2e9b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27330651"
---
# <a name="create-carttoclassassociation"></a><span data-ttu-id="645f5-103">创建 cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="645f5-103">Create cartToClassAssociation</span></span>

> <span data-ttu-id="645f5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="645f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="645f5-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="645f5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="645f5-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="645f5-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="645f5-107">创建新的[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="645f5-107">Create a new [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="645f5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="645f5-108">Prerequisites</span></span>
<span data-ttu-id="645f5-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="645f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="645f5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="645f5-111">Permission type</span></span>|<span data-ttu-id="645f5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="645f5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="645f5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="645f5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="645f5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="645f5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="645f5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="645f5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="645f5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="645f5-116">Not supported.</span></span>|
|<span data-ttu-id="645f5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="645f5-117">Application</span></span>|<span data-ttu-id="645f5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="645f5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="645f5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="645f5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/cartToClassAssociations
```

## <a name="request-headers"></a><span data-ttu-id="645f5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="645f5-120">Request headers</span></span>
|<span data-ttu-id="645f5-121">标头</span><span class="sxs-lookup"><span data-stu-id="645f5-121">Header</span></span>|<span data-ttu-id="645f5-122">值</span><span class="sxs-lookup"><span data-stu-id="645f5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="645f5-123">授权</span><span class="sxs-lookup"><span data-stu-id="645f5-123">Authorization</span></span>|<span data-ttu-id="645f5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="645f5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="645f5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="645f5-125">Accept</span></span>|<span data-ttu-id="645f5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="645f5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="645f5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="645f5-127">Request body</span></span>
<span data-ttu-id="645f5-128">在请求正文中，提供 cartToClassAssociation 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="645f5-128">In the request body, supply a JSON representation for the cartToClassAssociation object.</span></span>

<span data-ttu-id="645f5-129">下表显示时创建 cartToClassAssociation 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="645f5-129">The following table shows the properties that are required when you create the cartToClassAssociation.</span></span>

|<span data-ttu-id="645f5-130">属性</span><span class="sxs-lookup"><span data-stu-id="645f5-130">Property</span></span>|<span data-ttu-id="645f5-131">类型</span><span class="sxs-lookup"><span data-stu-id="645f5-131">Type</span></span>|<span data-ttu-id="645f5-132">说明</span><span class="sxs-lookup"><span data-stu-id="645f5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="645f5-133">id</span><span class="sxs-lookup"><span data-stu-id="645f5-133">id</span></span>|<span data-ttu-id="645f5-134">String</span><span class="sxs-lookup"><span data-stu-id="645f5-134">String</span></span>|<span data-ttu-id="645f5-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="645f5-135">Key of the entity.</span></span>|
|<span data-ttu-id="645f5-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="645f5-136">createdDateTime</span></span>|<span data-ttu-id="645f5-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="645f5-137">DateTimeOffset</span></span>|<span data-ttu-id="645f5-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="645f5-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="645f5-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="645f5-139">lastModifiedDateTime</span></span>|<span data-ttu-id="645f5-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="645f5-140">DateTimeOffset</span></span>|<span data-ttu-id="645f5-141">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="645f5-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="645f5-142">version</span><span class="sxs-lookup"><span data-stu-id="645f5-142">version</span></span>|<span data-ttu-id="645f5-143">Int32</span><span class="sxs-lookup"><span data-stu-id="645f5-143">Int32</span></span>|<span data-ttu-id="645f5-144">CartToClassAssociation 版本。</span><span class="sxs-lookup"><span data-stu-id="645f5-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="645f5-145">displayName</span><span class="sxs-lookup"><span data-stu-id="645f5-145">displayName</span></span>|<span data-ttu-id="645f5-146">String</span><span class="sxs-lookup"><span data-stu-id="645f5-146">String</span></span>|<span data-ttu-id="645f5-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="645f5-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="645f5-148">说明</span><span class="sxs-lookup"><span data-stu-id="645f5-148">description</span></span>|<span data-ttu-id="645f5-149">字符串</span><span class="sxs-lookup"><span data-stu-id="645f5-149">String</span></span>|<span data-ttu-id="645f5-150">管理员提供 CartToClassAssociation 的说明。</span><span class="sxs-lookup"><span data-stu-id="645f5-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="645f5-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="645f5-151">deviceCartIds</span></span>|<span data-ttu-id="645f5-152">String 集合</span><span class="sxs-lookup"><span data-stu-id="645f5-152">String collection</span></span>|<span data-ttu-id="645f5-153">设备车与类相关联的标识符。</span><span class="sxs-lookup"><span data-stu-id="645f5-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="645f5-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="645f5-154">classroomIds</span></span>|<span data-ttu-id="645f5-155">String 集合</span><span class="sxs-lookup"><span data-stu-id="645f5-155">String collection</span></span>|<span data-ttu-id="645f5-156">教室与设备车相关联的标识符。</span><span class="sxs-lookup"><span data-stu-id="645f5-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="645f5-157">响应</span><span class="sxs-lookup"><span data-stu-id="645f5-157">Response</span></span>
<span data-ttu-id="645f5-158">如果成功，此方法返回`201 Created`响应代码和响应正文中的[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="645f5-158">If successful, this method returns a `201 Created` response code and a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="645f5-159">示例</span><span class="sxs-lookup"><span data-stu-id="645f5-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="645f5-160">请求</span><span class="sxs-lookup"><span data-stu-id="645f5-160">Request</span></span>
<span data-ttu-id="645f5-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="645f5-161">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations
Content-type: application/json
Content-length: 335

{
  "@odata.type": "#microsoft.graph.cartToClassAssociation",
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

### <a name="response"></a><span data-ttu-id="645f5-162">响应</span><span class="sxs-lookup"><span data-stu-id="645f5-162">Response</span></span>
<span data-ttu-id="645f5-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="645f5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





