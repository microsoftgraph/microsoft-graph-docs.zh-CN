---
title: 更新 embeddedSIMActivationCodePool
description: 更新 embeddedSIMActivationCodePool 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 6af2c40b0fb028b4f057c15922e2489344f80ee6
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48005031"
---
# <a name="update-embeddedsimactivationcodepool"></a><span data-ttu-id="96ddc-103">更新 embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="96ddc-103">Update embeddedSIMActivationCodePool</span></span>

<span data-ttu-id="96ddc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="96ddc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="96ddc-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="96ddc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="96ddc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="96ddc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="96ddc-107">更新 [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="96ddc-107">Update the properties of a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="96ddc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="96ddc-108">Prerequisites</span></span>
<span data-ttu-id="96ddc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="96ddc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="96ddc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="96ddc-111">Permission type</span></span>|<span data-ttu-id="96ddc-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="96ddc-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="96ddc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="96ddc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="96ddc-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96ddc-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="96ddc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="96ddc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="96ddc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="96ddc-116">Not supported.</span></span>|
|<span data-ttu-id="96ddc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="96ddc-117">Application</span></span>|<span data-ttu-id="96ddc-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="96ddc-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="96ddc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="96ddc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="request-headers"></a><span data-ttu-id="96ddc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="96ddc-120">Request headers</span></span>
|<span data-ttu-id="96ddc-121">标头</span><span class="sxs-lookup"><span data-stu-id="96ddc-121">Header</span></span>|<span data-ttu-id="96ddc-122">值</span><span class="sxs-lookup"><span data-stu-id="96ddc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="96ddc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="96ddc-123">Authorization</span></span>|<span data-ttu-id="96ddc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="96ddc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="96ddc-125">接受</span><span class="sxs-lookup"><span data-stu-id="96ddc-125">Accept</span></span>|<span data-ttu-id="96ddc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="96ddc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="96ddc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="96ddc-127">Request body</span></span>
<span data-ttu-id="96ddc-128">在请求正文中，提供 [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="96ddc-128">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

<span data-ttu-id="96ddc-129">下表显示创建 [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="96ddc-129">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span></span>

|<span data-ttu-id="96ddc-130">属性</span><span class="sxs-lookup"><span data-stu-id="96ddc-130">Property</span></span>|<span data-ttu-id="96ddc-131">类型</span><span class="sxs-lookup"><span data-stu-id="96ddc-131">Type</span></span>|<span data-ttu-id="96ddc-132">说明</span><span class="sxs-lookup"><span data-stu-id="96ddc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="96ddc-133">id</span><span class="sxs-lookup"><span data-stu-id="96ddc-133">id</span></span>|<span data-ttu-id="96ddc-134">String</span><span class="sxs-lookup"><span data-stu-id="96ddc-134">String</span></span>|<span data-ttu-id="96ddc-135">嵌入的 SIM 激活代码池的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="96ddc-135">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="96ddc-136">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="96ddc-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="96ddc-137">displayName</span><span class="sxs-lookup"><span data-stu-id="96ddc-137">displayName</span></span>|<span data-ttu-id="96ddc-138">String</span><span class="sxs-lookup"><span data-stu-id="96ddc-138">String</span></span>|<span data-ttu-id="96ddc-139">管理员定义的嵌入式 SIM 激活代码池的名称。</span><span class="sxs-lookup"><span data-stu-id="96ddc-139">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="96ddc-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="96ddc-140">createdDateTime</span></span>|<span data-ttu-id="96ddc-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96ddc-141">DateTimeOffset</span></span>|<span data-ttu-id="96ddc-142">创建嵌入的 SIM 激活代码池的时间。</span><span class="sxs-lookup"><span data-stu-id="96ddc-142">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="96ddc-143">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="96ddc-143">Generated service side.</span></span>|
|<span data-ttu-id="96ddc-144">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="96ddc-144">modifiedDateTime</span></span>|<span data-ttu-id="96ddc-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="96ddc-145">DateTimeOffset</span></span>|<span data-ttu-id="96ddc-146">上次修改嵌入的 SIM 激活代码池的时间。</span><span class="sxs-lookup"><span data-stu-id="96ddc-146">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="96ddc-147">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="96ddc-147">Updated service side.</span></span>|
|<span data-ttu-id="96ddc-148">activationCodes</span><span class="sxs-lookup"><span data-stu-id="96ddc-148">activationCodes</span></span>|<span data-ttu-id="96ddc-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) 集合</span><span class="sxs-lookup"><span data-stu-id="96ddc-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="96ddc-150">属于此池的激活代码。</span><span class="sxs-lookup"><span data-stu-id="96ddc-150">The activation codes which belong to this pool.</span></span> <span data-ttu-id="96ddc-151">此导航属性用于将激活代码发布到 Intune，但不能用于从 Intune 读取激活代码。</span><span class="sxs-lookup"><span data-stu-id="96ddc-151">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="96ddc-152">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="96ddc-152">activationCodeCount</span></span>|<span data-ttu-id="96ddc-153">Int32</span><span class="sxs-lookup"><span data-stu-id="96ddc-153">Int32</span></span>|<span data-ttu-id="96ddc-154">属于此池的激活代码的总计数。</span><span class="sxs-lookup"><span data-stu-id="96ddc-154">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="96ddc-155">响应</span><span class="sxs-lookup"><span data-stu-id="96ddc-155">Response</span></span>
<span data-ttu-id="96ddc-156">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="96ddc-156">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="96ddc-157">示例</span><span class="sxs-lookup"><span data-stu-id="96ddc-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="96ddc-158">请求</span><span class="sxs-lookup"><span data-stu-id="96ddc-158">Request</span></span>
<span data-ttu-id="96ddc-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="96ddc-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="96ddc-160">响应</span><span class="sxs-lookup"><span data-stu-id="96ddc-160">Response</span></span>
<span data-ttu-id="96ddc-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="96ddc-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






