---
title: 更新 cartToClassAssociation
description: 更新 cartToClassAssociation 对象的属性。
ms.openlocfilehash: ecdfdca855920c26e607f24771e41392f74d7095
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046614"
---
# <a name="update-carttoclassassociation"></a><span data-ttu-id="c37d0-103">更新 cartToClassAssociation</span><span class="sxs-lookup"><span data-stu-id="c37d0-103">Update cartToClassAssociation</span></span>

> <span data-ttu-id="c37d0-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="c37d0-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="c37d0-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="c37d0-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="c37d0-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="c37d0-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="c37d0-107">更新[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="c37d0-107">Update the properties of a [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="c37d0-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="c37d0-108">Prerequisites</span></span>
<span data-ttu-id="c37d0-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="c37d0-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c37d0-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c37d0-111">Permission type</span></span>|<span data-ttu-id="c37d0-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c37d0-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c37d0-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c37d0-113">Delegated (work or school account)</span></span>|<span data-ttu-id="c37d0-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c37d0-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="c37d0-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c37d0-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c37d0-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c37d0-116">Not supported.</span></span>|
|<span data-ttu-id="c37d0-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c37d0-117">Application</span></span>|<span data-ttu-id="c37d0-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c37d0-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c37d0-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c37d0-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
```

## <a name="request-headers"></a><span data-ttu-id="c37d0-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c37d0-120">Request headers</span></span>
|<span data-ttu-id="c37d0-121">标头</span><span class="sxs-lookup"><span data-stu-id="c37d0-121">Header</span></span>|<span data-ttu-id="c37d0-122">值</span><span class="sxs-lookup"><span data-stu-id="c37d0-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="c37d0-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c37d0-123">Authorization</span></span>|<span data-ttu-id="c37d0-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="c37d0-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="c37d0-125">Accept</span><span class="sxs-lookup"><span data-stu-id="c37d0-125">Accept</span></span>|<span data-ttu-id="c37d0-126">application/json</span><span class="sxs-lookup"><span data-stu-id="c37d0-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="c37d0-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c37d0-127">Request body</span></span>
<span data-ttu-id="c37d0-128">在请求正文中，提供[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c37d0-128">In the request body, supply a JSON representation for the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object.</span></span>

<span data-ttu-id="c37d0-129">下表显示时创建[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c37d0-129">The following table shows the properties that are required when you create the [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md).</span></span>

|<span data-ttu-id="c37d0-130">属性</span><span class="sxs-lookup"><span data-stu-id="c37d0-130">Property</span></span>|<span data-ttu-id="c37d0-131">类型</span><span class="sxs-lookup"><span data-stu-id="c37d0-131">Type</span></span>|<span data-ttu-id="c37d0-132">说明</span><span class="sxs-lookup"><span data-stu-id="c37d0-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c37d0-133">id</span><span class="sxs-lookup"><span data-stu-id="c37d0-133">id</span></span>|<span data-ttu-id="c37d0-134">String</span><span class="sxs-lookup"><span data-stu-id="c37d0-134">String</span></span>|<span data-ttu-id="c37d0-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="c37d0-135">Key of the entity.</span></span>|
|<span data-ttu-id="c37d0-136">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c37d0-136">createdDateTime</span></span>|<span data-ttu-id="c37d0-137">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c37d0-137">DateTimeOffset</span></span>|<span data-ttu-id="c37d0-138">创建对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c37d0-138">DateTime the object was created.</span></span>|
|<span data-ttu-id="c37d0-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c37d0-139">lastModifiedDateTime</span></span>|<span data-ttu-id="c37d0-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c37d0-140">DateTimeOffset</span></span>|<span data-ttu-id="c37d0-141">上次修改对象的日期/时间。</span><span class="sxs-lookup"><span data-stu-id="c37d0-141">DateTime the object was last modified.</span></span>|
|<span data-ttu-id="c37d0-142">version</span><span class="sxs-lookup"><span data-stu-id="c37d0-142">version</span></span>|<span data-ttu-id="c37d0-143">Int32</span><span class="sxs-lookup"><span data-stu-id="c37d0-143">Int32</span></span>|<span data-ttu-id="c37d0-144">CartToClassAssociation 版本。</span><span class="sxs-lookup"><span data-stu-id="c37d0-144">Version of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="c37d0-145">displayName</span><span class="sxs-lookup"><span data-stu-id="c37d0-145">displayName</span></span>|<span data-ttu-id="c37d0-146">String</span><span class="sxs-lookup"><span data-stu-id="c37d0-146">String</span></span>|<span data-ttu-id="c37d0-147">管理员提供的设备配置的名称。</span><span class="sxs-lookup"><span data-stu-id="c37d0-147">Admin provided name of the device configuration.</span></span>|
|<span data-ttu-id="c37d0-148">说明</span><span class="sxs-lookup"><span data-stu-id="c37d0-148">description</span></span>|<span data-ttu-id="c37d0-149">字符串</span><span class="sxs-lookup"><span data-stu-id="c37d0-149">String</span></span>|<span data-ttu-id="c37d0-150">管理员提供 CartToClassAssociation 的说明。</span><span class="sxs-lookup"><span data-stu-id="c37d0-150">Admin provided description of the CartToClassAssociation.</span></span>|
|<span data-ttu-id="c37d0-151">deviceCartIds</span><span class="sxs-lookup"><span data-stu-id="c37d0-151">deviceCartIds</span></span>|<span data-ttu-id="c37d0-152">String 集合</span><span class="sxs-lookup"><span data-stu-id="c37d0-152">String collection</span></span>|<span data-ttu-id="c37d0-153">设备车与类相关联的标识符。</span><span class="sxs-lookup"><span data-stu-id="c37d0-153">Identifiers of device carts to be associated with classes.</span></span>|
|<span data-ttu-id="c37d0-154">classroomIds</span><span class="sxs-lookup"><span data-stu-id="c37d0-154">classroomIds</span></span>|<span data-ttu-id="c37d0-155">String 集合</span><span class="sxs-lookup"><span data-stu-id="c37d0-155">String collection</span></span>|<span data-ttu-id="c37d0-156">教室与设备车相关联的标识符。</span><span class="sxs-lookup"><span data-stu-id="c37d0-156">Identifiers of classrooms to be associated with device carts.</span></span>|



## <a name="response"></a><span data-ttu-id="c37d0-157">响应</span><span class="sxs-lookup"><span data-stu-id="c37d0-157">Response</span></span>
<span data-ttu-id="c37d0-158">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c37d0-158">If successful, this method returns a `200 OK` response code and an updated [cartToClassAssociation](../resources/intune-deviceconfig-carttoclassassociation.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c37d0-159">示例</span><span class="sxs-lookup"><span data-stu-id="c37d0-159">Example</span></span>
### <a name="request"></a><span data-ttu-id="c37d0-160">请求</span><span class="sxs-lookup"><span data-stu-id="c37d0-160">Request</span></span>
<span data-ttu-id="c37d0-161">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c37d0-161">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/cartToClassAssociations/{cartToClassAssociationId}
Content-type: application/json
Content-length: 274

{
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

### <a name="response"></a><span data-ttu-id="c37d0-162">响应</span><span class="sxs-lookup"><span data-stu-id="c37d0-162">Response</span></span>
<span data-ttu-id="c37d0-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c37d0-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





