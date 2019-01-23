---
title: 创建 embeddedSIMActivationCodePool
description: 创建新的 embeddedSIMActivationCodePool 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3b2d84230049c7b1f96756ac104557c5d8648c6a
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394024"
---
# <a name="create-embeddedsimactivationcodepool"></a><span data-ttu-id="eba30-103">创建 embeddedSIMActivationCodePool</span><span class="sxs-lookup"><span data-stu-id="eba30-103">Create embeddedSIMActivationCodePool</span></span>

> <span data-ttu-id="eba30-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="eba30-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="eba30-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="eba30-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="eba30-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="eba30-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="eba30-107">创建新的[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)对象。</span><span class="sxs-lookup"><span data-stu-id="eba30-107">Create a new [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="eba30-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="eba30-108">Prerequisites</span></span>
<span data-ttu-id="eba30-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="eba30-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="eba30-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="eba30-111">Permission type</span></span>|<span data-ttu-id="eba30-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="eba30-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="eba30-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="eba30-113">Delegated (work or school account)</span></span>|<span data-ttu-id="eba30-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="eba30-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="eba30-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="eba30-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="eba30-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="eba30-116">Not supported.</span></span>|
|<span data-ttu-id="eba30-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="eba30-117">Application</span></span>|<span data-ttu-id="eba30-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="eba30-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="eba30-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="eba30-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools
```

## <a name="request-headers"></a><span data-ttu-id="eba30-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="eba30-120">Request headers</span></span>
|<span data-ttu-id="eba30-121">标头</span><span class="sxs-lookup"><span data-stu-id="eba30-121">Header</span></span>|<span data-ttu-id="eba30-122">值</span><span class="sxs-lookup"><span data-stu-id="eba30-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="eba30-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="eba30-123">Authorization</span></span>|<span data-ttu-id="eba30-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="eba30-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="eba30-125">Accept</span><span class="sxs-lookup"><span data-stu-id="eba30-125">Accept</span></span>|<span data-ttu-id="eba30-126">application/json</span><span class="sxs-lookup"><span data-stu-id="eba30-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="eba30-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="eba30-127">Request body</span></span>
<span data-ttu-id="eba30-128">在请求正文中，提供 embeddedSIMActivationCodePool 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eba30-128">In the request body, supply a JSON representation for the embeddedSIMActivationCodePool object.</span></span>

<span data-ttu-id="eba30-129">下表显示时创建 embeddedSIMActivationCodePool 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="eba30-129">The following table shows the properties that are required when you create the embeddedSIMActivationCodePool.</span></span>

|<span data-ttu-id="eba30-130">属性</span><span class="sxs-lookup"><span data-stu-id="eba30-130">Property</span></span>|<span data-ttu-id="eba30-131">类型</span><span class="sxs-lookup"><span data-stu-id="eba30-131">Type</span></span>|<span data-ttu-id="eba30-132">说明</span><span class="sxs-lookup"><span data-stu-id="eba30-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="eba30-133">id</span><span class="sxs-lookup"><span data-stu-id="eba30-133">id</span></span>|<span data-ttu-id="eba30-134">String</span><span class="sxs-lookup"><span data-stu-id="eba30-134">String</span></span>|<span data-ttu-id="eba30-135">嵌入 SIM 激活代码池的的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="eba30-135">Unique identifier for the embedded SIM activation code pool.</span></span> <span data-ttu-id="eba30-136">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="eba30-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="eba30-137">displayName</span><span class="sxs-lookup"><span data-stu-id="eba30-137">displayName</span></span>|<span data-ttu-id="eba30-138">String</span><span class="sxs-lookup"><span data-stu-id="eba30-138">String</span></span>|<span data-ttu-id="eba30-139">管理员定义的嵌入 SIM 激活代码池的名称。</span><span class="sxs-lookup"><span data-stu-id="eba30-139">The admin defined name of the embedded SIM activation code pool.</span></span>|
|<span data-ttu-id="eba30-140">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="eba30-140">createdDateTime</span></span>|<span data-ttu-id="eba30-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eba30-141">DateTimeOffset</span></span>|<span data-ttu-id="eba30-142">嵌入的 SIM 激活代码池的创建时间。</span><span class="sxs-lookup"><span data-stu-id="eba30-142">The time the embedded SIM activation code pool was created.</span></span> <span data-ttu-id="eba30-143">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="eba30-143">Generated service side.</span></span>|
|<span data-ttu-id="eba30-144">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="eba30-144">modifiedDateTime</span></span>|<span data-ttu-id="eba30-145">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="eba30-145">DateTimeOffset</span></span>|<span data-ttu-id="eba30-146">嵌入的 SIM 激活代码池上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="eba30-146">The time the embedded SIM activation code pool was last modified.</span></span> <span data-ttu-id="eba30-147">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="eba30-147">Updated service side.</span></span>|
|<span data-ttu-id="eba30-148">activationCodes</span><span class="sxs-lookup"><span data-stu-id="eba30-148">activationCodes</span></span>|<span data-ttu-id="eba30-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md)集合</span><span class="sxs-lookup"><span data-stu-id="eba30-149">[embeddedSIMActivationCode](../resources/intune-esim-embeddedsimactivationcode.md) collection</span></span>|<span data-ttu-id="eba30-150">属于此池激活代码。</span><span class="sxs-lookup"><span data-stu-id="eba30-150">The activation codes which belong to this pool.</span></span> <span data-ttu-id="eba30-151">此导航属性用于发布到 Intune 的激活代码，但不能用于读取 Intune 激活代码。</span><span class="sxs-lookup"><span data-stu-id="eba30-151">This navigation property is used to post activation codes to Intune but cannot be used to read activation codes from Intune.</span></span>|
|<span data-ttu-id="eba30-152">activationCodeCount</span><span class="sxs-lookup"><span data-stu-id="eba30-152">activationCodeCount</span></span>|<span data-ttu-id="eba30-153">Int32</span><span class="sxs-lookup"><span data-stu-id="eba30-153">Int32</span></span>|<span data-ttu-id="eba30-154">属于此池的激活代码的总计数。</span><span class="sxs-lookup"><span data-stu-id="eba30-154">The total count of activation codes which belong to this pool.</span></span>|



## <a name="response"></a><span data-ttu-id="eba30-155">响应</span><span class="sxs-lookup"><span data-stu-id="eba30-155">Response</span></span>
<span data-ttu-id="eba30-156">如果成功，此方法返回`201 Created`响应代码和响应正文中的[embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md)对象。</span><span class="sxs-lookup"><span data-stu-id="eba30-156">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePool](../resources/intune-esim-embeddedsimactivationcodepool.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="eba30-157">示例</span><span class="sxs-lookup"><span data-stu-id="eba30-157">Example</span></span>

### <a name="request"></a><span data-ttu-id="eba30-158">请求</span><span class="sxs-lookup"><span data-stu-id="eba30-158">Request</span></span>
<span data-ttu-id="eba30-159">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="eba30-159">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="eba30-160">响应</span><span class="sxs-lookup"><span data-stu-id="eba30-160">Response</span></span>
<span data-ttu-id="eba30-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="eba30-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




