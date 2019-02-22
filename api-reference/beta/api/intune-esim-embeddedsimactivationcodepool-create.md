---
title: 创建 embeddedSIMActivationCodePool
description: 创建新的 embeddedSIMActivationCodePool 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9c0cf5f48f10d01fbaf5e15d74d8fb2421e203f7
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174599"
---
# <a name="create-embeddedsimactivationcodepool"></a><span data-ttu-id="3c16e-103">创建 embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="3c16e-103">Create embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="3c16e-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3c16e-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c16e-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c16e-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c16e-106">创建新的[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3c16e-106">Create a new [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c16e-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="3c16e-107">Prerequisites</span></span>
<span data-ttu-id="3c16e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="3c16e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="3c16e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c16e-110">Permission type</span></span>|<span data-ttu-id="3c16e-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3c16e-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c16e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c16e-112">Delegated (work or school account)</span></span>|<span data-ttu-id="3c16e-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c16e-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="3c16e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c16e-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c16e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c16e-115">Not supported.</span></span>|
|<span data-ttu-id="3c16e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c16e-116">Application</span></span>|<span data-ttu-id="3c16e-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c16e-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c16e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c16e-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools
```

## <a name="request-headers"></a><span data-ttu-id="3c16e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c16e-119">Request headers</span></span>
|<span data-ttu-id="3c16e-120">标头</span><span class="sxs-lookup"><span data-stu-id="3c16e-120">Header</span></span>|<span data-ttu-id="3c16e-121">值</span><span class="sxs-lookup"><span data-stu-id="3c16e-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c16e-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c16e-122">Authorization</span></span>|<span data-ttu-id="3c16e-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3c16e-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c16e-124">Accept</span><span class="sxs-lookup"><span data-stu-id="3c16e-124">Accept</span></span>|<span data-ttu-id="3c16e-125">application/json</span><span class="sxs-lookup"><span data-stu-id="3c16e-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c16e-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c16e-126">Request body</span></span>
<span data-ttu-id="3c16e-127">在请求正文中, 提供 embeddedSIMActivationCodePool 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c16e-127">In the request body, supply a JSON representation for the embeddedSIMActivationCodePool object.</span></span>

<span data-ttu-id="3c16e-128">下表显示创建 embeddedSIMActivationCodePool 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3c16e-128">The following table shows the properties that are required when you create the embeddedSIMActivationCodePool.</span></span>

|<span data-ttu-id="3c16e-129">属性</span><span class="sxs-lookup"><span data-stu-id="3c16e-129">Property</span></span>|<span data-ttu-id="3c16e-130">类型</span><span class="sxs-lookup"><span data-stu-id="3c16e-130">Type</span></span>|<span data-ttu-id="3c16e-131">说明</span><span class="sxs-lookup"><span data-stu-id="3c16e-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c16e-132">id</span><span class="sxs-lookup"><span data-stu-id="3c16e-132">id</span></span>|<span data-ttu-id="3c16e-133">字符串</span><span class="sxs-lookup"><span data-stu-id="3c16e-133">String</span></span>|<span data-ttu-id="3c16e-134">嵌入的 SIM 激活代码池的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3c16e-134">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="3c16e-135">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="3c16e-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="3c16e-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3c16e-136">displayName</span></span>|<span data-ttu-id="3c16e-137">String</span><span class="sxs-lookup"><span data-stu-id="3c16e-137">String</span></span>|<span data-ttu-id="3c16e-138">管理员定义的嵌入式 SIM 激活代码池的名称。</span><span class="sxs-lookup"><span data-stu-id="3c16e-138">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="3c16e-139">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c16e-139">createdDateTime</span></span>|<span data-ttu-id="3c16e-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c16e-140">DateTimeOffset</span></span>|<span data-ttu-id="3c16e-141">创建嵌入的 SIM 激活代码池的时间。</span><span class="sxs-lookup"><span data-stu-id="3c16e-141">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="3c16e-142">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="3c16e-142">Generated service side.</span></span>|
|<span data-ttu-id="3c16e-143">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c16e-143">modifiedDateTime</span></span>|<span data-ttu-id="3c16e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c16e-144">DateTimeOffset</span></span>|<span data-ttu-id="3c16e-145">上次修改嵌入的 SIM 激活代码池的时间。</span><span class="sxs-lookup"><span data-stu-id="3c16e-145">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="3c16e-146">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="3c16e-146">Updated service side.</span></span>|
|<span data-ttu-id="3c16e-147">activationCodes</span><span class="sxs-lookup"><span data-stu-id="3c16e-147">activationCodes</span></span>|<span data-ttu-id="3c16e-148">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)集合</span><span class="sxs-lookup"><span data-stu-id="3c16e-148">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="3c16e-149">属于此池的激活代码。</span><span class="sxs-lookup"><span data-stu-id="3c16e-149">The activation codes which belong to this pool.</span></span> <span data-ttu-id="3c16e-150">此导航属性用于将激活代码发布到 intune, 但不能用于从 Intune 读取激活代码。</span><span class="sxs-lookup"><span data-stu-id="3c16e-150">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="3c16e-151">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="3c16e-151">activationCodeCount</span></span>|<span data-ttu-id="3c16e-152">Int32</span><span class="sxs-lookup"><span data-stu-id="3c16e-152">Int32</span></span>|<span data-ttu-id="3c16e-153">属于此池的激活代码的总计数。</span><span class="sxs-lookup"><span data-stu-id="3c16e-153">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="3c16e-154">响应</span><span class="sxs-lookup"><span data-stu-id="3c16e-154">Response</span></span>
<span data-ttu-id="3c16e-155">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3c16e-155">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c16e-156">示例</span><span class="sxs-lookup"><span data-stu-id="3c16e-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c16e-157">请求</span><span class="sxs-lookup"><span data-stu-id="3c16e-157">Request</span></span>
<span data-ttu-id="3c16e-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c16e-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools
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

### <a name="response"></a><span data-ttu-id="3c16e-159">响应</span><span class="sxs-lookup"><span data-stu-id="3c16e-159">Response</span></span>
<span data-ttu-id="3c16e-p106">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3c16e-p106">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




