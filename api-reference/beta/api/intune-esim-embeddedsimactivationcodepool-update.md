---
title: 更新 embeddedSIMActivationCodePool
description: 更新嵌入式SIMActivationCodePool 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: be9d88f6f75d677cf3b8133e8e094da2f1c09dda
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51126127"
---
# <a name="update-embeddedsimactivationcodepool"></a><span data-ttu-id="a3588-103">更新 embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="a3588-103">Update embeddedSIMActivationCodePool</span></span>

<span data-ttu-id="a3588-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a3588-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a3588-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a3588-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a3588-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a3588-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a3588-107">更新嵌入式 [SIMActivationCodePool 对象](../resources/intune-esim-embeddedsimactivationcodepool.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="a3588-107">Update the properties of a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a3588-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a3588-108">Prerequisites</span></span>
<span data-ttu-id="a3588-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a3588-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a3588-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a3588-111">Permission type</span></span>|<span data-ttu-id="a3588-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a3588-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a3588-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a3588-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a3588-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3588-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a3588-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a3588-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a3588-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a3588-116">Not supported.</span></span>|
|<span data-ttu-id="a3588-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a3588-117">Application</span></span>|<span data-ttu-id="a3588-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a3588-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a3588-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a3588-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}
```

## <a name="request-headers"></a><span data-ttu-id="a3588-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a3588-120">Request headers</span></span>
|<span data-ttu-id="a3588-121">标头</span><span class="sxs-lookup"><span data-stu-id="a3588-121">Header</span></span>|<span data-ttu-id="a3588-122">值</span><span class="sxs-lookup"><span data-stu-id="a3588-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a3588-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a3588-123">Authorization</span></span>|<span data-ttu-id="a3588-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a3588-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a3588-125">接受</span><span class="sxs-lookup"><span data-stu-id="a3588-125">Accept</span></span>|<span data-ttu-id="a3588-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a3588-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a3588-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a3588-127">Request body</span></span>
<span data-ttu-id="a3588-128">在请求正文中，提供 [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a3588-128">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

<span data-ttu-id="a3588-129">下表显示创建 [embeddedSIMActivationCodePool 时所需的属性](../resources/intune-esim-embeddedsimactivationcodepool.md)。</span><span class="sxs-lookup"><span data-stu-id="a3588-129">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md).</span></span>

|<span data-ttu-id="a3588-130">属性</span><span class="sxs-lookup"><span data-stu-id="a3588-130">Property</span></span>|<span data-ttu-id="a3588-131">类型</span><span class="sxs-lookup"><span data-stu-id="a3588-131">Type</span></span>|<span data-ttu-id="a3588-132">说明</span><span class="sxs-lookup"><span data-stu-id="a3588-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a3588-133">id</span><span class="sxs-lookup"><span data-stu-id="a3588-133">id</span></span>|<span data-ttu-id="a3588-134">String</span><span class="sxs-lookup"><span data-stu-id="a3588-134">String</span></span>|<span data-ttu-id="a3588-135">嵌入式 SIM 卡激活代码池的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="a3588-135">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="a3588-136">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="a3588-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="a3588-137">displayName</span><span class="sxs-lookup"><span data-stu-id="a3588-137">displayName</span></span>|<span data-ttu-id="a3588-138">String</span><span class="sxs-lookup"><span data-stu-id="a3588-138">String</span></span>|<span data-ttu-id="a3588-139">管理员定义的嵌入式 SIM 卡激活代码池的名称。</span><span class="sxs-lookup"><span data-stu-id="a3588-139">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="a3588-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="a3588-140">createdDateTime</span></span>|<span data-ttu-id="a3588-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3588-141">DateTimeOffset</span></span>|<span data-ttu-id="a3588-142">嵌入式 SIM 卡激活代码池的创建时间。</span><span class="sxs-lookup"><span data-stu-id="a3588-142">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="a3588-143">生成的服务器端。</span><span class="sxs-lookup"><span data-stu-id="a3588-143">Generated service side.</span></span>|
|<span data-ttu-id="a3588-144">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a3588-144">modifiedDateTime</span></span>|<span data-ttu-id="a3588-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a3588-145">DateTimeOffset</span></span>|<span data-ttu-id="a3588-146">上次修改嵌入式 SIM 卡激活代码池的时间。</span><span class="sxs-lookup"><span data-stu-id="a3588-146">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="a3588-147">更新的服务器端。</span><span class="sxs-lookup"><span data-stu-id="a3588-147">Updated service side.</span></span>|
|<span data-ttu-id="a3588-148">activationCodes</span><span class="sxs-lookup"><span data-stu-id="a3588-148">activationCodes</span></span>|<span data-ttu-id="a3588-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) 集合</span><span class="sxs-lookup"><span data-stu-id="a3588-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="a3588-150">属于此池的激活代码。</span><span class="sxs-lookup"><span data-stu-id="a3588-150">The activation codes which belong to this pool.</span></span> <span data-ttu-id="a3588-151">此导航属性用于将激活代码张贴到 Intune，但不能用于从 Intune 读取激活代码。</span><span class="sxs-lookup"><span data-stu-id="a3588-151">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="a3588-152">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="a3588-152">activationCodeCount</span></span>|<span data-ttu-id="a3588-153">Int32</span><span class="sxs-lookup"><span data-stu-id="a3588-153">Int32</span></span>|<span data-ttu-id="a3588-154">属于此池的激活代码总数。</span><span class="sxs-lookup"><span data-stu-id="a3588-154">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="a3588-155">响应</span><span class="sxs-lookup"><span data-stu-id="a3588-155">Response</span></span>
<span data-ttu-id="a3588-156">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a3588-156">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a3588-157">示例</span><span class="sxs-lookup"><span data-stu-id="a3588-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="a3588-158">请求</span><span class="sxs-lookup"><span data-stu-id="a3588-158">Request</span></span>
<span data-ttu-id="a3588-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a3588-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="a3588-160">响应</span><span class="sxs-lookup"><span data-stu-id="a3588-160">Response</span></span>
<span data-ttu-id="a3588-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a3588-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




