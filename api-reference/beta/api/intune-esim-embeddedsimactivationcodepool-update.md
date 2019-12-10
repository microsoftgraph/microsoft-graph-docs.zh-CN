---
title: 更新 embeddedSIMActivationCodePool
description: 更新 embeddedSIMActivationCodePool 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: f35d6d32037b24574a4917160917c1f54ed82a4b
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943591"
---
# <a name="update-embeddedsimactivationcodepool"></a><span data-ttu-id="4f00d-103">更新 embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="4f00d-103">Update embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="4f00d-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="4f00d-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4f00d-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="4f00d-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4f00d-106">更新[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="4f00d-106">Update the properties of a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4f00d-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="4f00d-107">Prerequisites</span></span>
<span data-ttu-id="4f00d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="4f00d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4f00d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="4f00d-110">Permission type</span></span>|<span data-ttu-id="4f00d-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="4f00d-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4f00d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="4f00d-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4f00d-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f00d-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4f00d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="4f00d-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4f00d-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="4f00d-115">Not supported.</span></span>|
|<span data-ttu-id="4f00d-116">Application</span><span class="sxs-lookup"><span data-stu-id="4f00d-116">Application</span></span>|<span data-ttu-id="4f00d-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4f00d-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="4f00d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="4f00d-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="request-headers"></a><span data-ttu-id="4f00d-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="4f00d-119">Request headers</span></span>
|<span data-ttu-id="4f00d-120">标头</span><span class="sxs-lookup"><span data-stu-id="4f00d-120">Header</span></span>|<span data-ttu-id="4f00d-121">值</span><span class="sxs-lookup"><span data-stu-id="4f00d-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4f00d-122">授权</span><span class="sxs-lookup"><span data-stu-id="4f00d-122">Authorization</span></span>|<span data-ttu-id="4f00d-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="4f00d-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4f00d-124">接受</span><span class="sxs-lookup"><span data-stu-id="4f00d-124">Accept</span></span>|<span data-ttu-id="4f00d-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4f00d-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4f00d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="4f00d-126">Request body</span></span>
<span data-ttu-id="4f00d-127">在请求正文中，提供[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="4f00d-127">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

<span data-ttu-id="4f00d-128">下表显示创建[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="4f00d-128">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span></span>

|<span data-ttu-id="4f00d-129">属性</span><span class="sxs-lookup"><span data-stu-id="4f00d-129">Property</span></span>|<span data-ttu-id="4f00d-130">类型</span><span class="sxs-lookup"><span data-stu-id="4f00d-130">Type</span></span>|<span data-ttu-id="4f00d-131">说明</span><span class="sxs-lookup"><span data-stu-id="4f00d-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4f00d-132">id</span><span class="sxs-lookup"><span data-stu-id="4f00d-132">id</span></span>|<span data-ttu-id="4f00d-133">字符串</span><span class="sxs-lookup"><span data-stu-id="4f00d-133">String</span></span>|<span data-ttu-id="4f00d-134">嵌入的 SIM 激活代码池的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="4f00d-134">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="4f00d-135">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="4f00d-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="4f00d-136">displayName</span><span class="sxs-lookup"><span data-stu-id="4f00d-136">displayName</span></span>|<span data-ttu-id="4f00d-137">String</span><span class="sxs-lookup"><span data-stu-id="4f00d-137">String</span></span>|<span data-ttu-id="4f00d-138">管理员定义的嵌入式 SIM 激活代码池的名称。</span><span class="sxs-lookup"><span data-stu-id="4f00d-138">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="4f00d-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="4f00d-139">createdDateTime</span></span>|<span data-ttu-id="4f00d-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f00d-140">DateTimeOffset</span></span>|<span data-ttu-id="4f00d-141">创建嵌入的 SIM 激活代码池的时间。</span><span class="sxs-lookup"><span data-stu-id="4f00d-141">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="4f00d-142">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="4f00d-142">Generated service side.</span></span>|
|<span data-ttu-id="4f00d-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="4f00d-143">modifiedDateTime</span></span>|<span data-ttu-id="4f00d-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="4f00d-144">DateTimeOffset</span></span>|<span data-ttu-id="4f00d-145">上次修改嵌入的 SIM 激活代码池的时间。</span><span class="sxs-lookup"><span data-stu-id="4f00d-145">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="4f00d-146">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="4f00d-146">Updated service side.</span></span>|
|<span data-ttu-id="4f00d-147">activationCodes</span><span class="sxs-lookup"><span data-stu-id="4f00d-147">activationCodes</span></span>|<span data-ttu-id="4f00d-148">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)集合</span><span class="sxs-lookup"><span data-stu-id="4f00d-148">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="4f00d-149">属于此池的激活代码。</span><span class="sxs-lookup"><span data-stu-id="4f00d-149">The activation codes which belong to this pool.</span></span> <span data-ttu-id="4f00d-150">此导航属性用于将激活代码发布到 Intune，但不能用于从 Intune 读取激活代码。</span><span class="sxs-lookup"><span data-stu-id="4f00d-150">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="4f00d-151">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="4f00d-151">activationCodeCount</span></span>|<span data-ttu-id="4f00d-152">Int32</span><span class="sxs-lookup"><span data-stu-id="4f00d-152">Int32</span></span>|<span data-ttu-id="4f00d-153">属于此池的激活代码的总计数。</span><span class="sxs-lookup"><span data-stu-id="4f00d-153">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="4f00d-154">响应</span><span class="sxs-lookup"><span data-stu-id="4f00d-154">Response</span></span>
<span data-ttu-id="4f00d-155">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)对象。</span><span class="sxs-lookup"><span data-stu-id="4f00d-155">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4f00d-156">示例</span><span class="sxs-lookup"><span data-stu-id="4f00d-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="4f00d-157">请求</span><span class="sxs-lookup"><span data-stu-id="4f00d-157">Request</span></span>
<span data-ttu-id="4f00d-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="4f00d-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
Content-type: application/json
Content-length: 460

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "displayName": "Display Name value",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```

### <a name="response"></a><span data-ttu-id="4f00d-159">响应</span><span class="sxs-lookup"><span data-stu-id="4f00d-159">Response</span></span>
<span data-ttu-id="4f00d-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="4f00d-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 628

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePool",
  "id": "ec308741-8741-ec30-4187-30ec418730ec",
  "displayName": "Display Name value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "activationCodes": [
    {
      "@odata.type": "microsoft.graph.embeddedSIMActivationCode",
      "integratedCircuitCardIdentifier": "Integrated Circuit Card Identifier value",
      "matchingIdentifier": "Matching Identifier value",
      "smdpPlusServerAddress": "Smdp Plus Server Address value"
    }
  ],
  "activationCodeCount": 3
}
```





