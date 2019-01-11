---
title: 更新 sideLoadingKey
description: 更新 sideLoadingKey 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 6f4a6348df539924bdccbf3cacf8411442f877eb
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27885629"
---
# <a name="update-sideloadingkey"></a><span data-ttu-id="de802-103">更新 sideLoadingKey</span><span class="sxs-lookup"><span data-stu-id="de802-103">Update sideLoadingKey</span></span>

> <span data-ttu-id="de802-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="de802-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="de802-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="de802-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="de802-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="de802-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="de802-107">更新[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="de802-107">Update the properties of a [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="de802-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="de802-108">Prerequisites</span></span>
<span data-ttu-id="de802-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="de802-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="de802-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="de802-111">Permission type</span></span>|<span data-ttu-id="de802-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="de802-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="de802-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="de802-113">Delegated (work or school account)</span></span>|<span data-ttu-id="de802-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="de802-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="de802-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="de802-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="de802-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="de802-116">Not supported.</span></span>|
|<span data-ttu-id="de802-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="de802-117">Application</span></span>|<span data-ttu-id="de802-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="de802-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="de802-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="de802-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
```

## <a name="request-headers"></a><span data-ttu-id="de802-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="de802-120">Request headers</span></span>
|<span data-ttu-id="de802-121">标头</span><span class="sxs-lookup"><span data-stu-id="de802-121">Header</span></span>|<span data-ttu-id="de802-122">值</span><span class="sxs-lookup"><span data-stu-id="de802-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="de802-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="de802-123">Authorization</span></span>|<span data-ttu-id="de802-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="de802-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="de802-125">Accept</span><span class="sxs-lookup"><span data-stu-id="de802-125">Accept</span></span>|<span data-ttu-id="de802-126">application/json</span><span class="sxs-lookup"><span data-stu-id="de802-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="de802-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="de802-127">Request body</span></span>
<span data-ttu-id="de802-128">在请求正文中，提供[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="de802-128">In the request body, supply a JSON representation for the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object.</span></span>

<span data-ttu-id="de802-129">下表显示时创建[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="de802-129">The following table shows the properties that are required when you create the [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md).</span></span>

|<span data-ttu-id="de802-130">属性</span><span class="sxs-lookup"><span data-stu-id="de802-130">Property</span></span>|<span data-ttu-id="de802-131">类型</span><span class="sxs-lookup"><span data-stu-id="de802-131">Type</span></span>|<span data-ttu-id="de802-132">说明</span><span class="sxs-lookup"><span data-stu-id="de802-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="de802-133">id</span><span class="sxs-lookup"><span data-stu-id="de802-133">id</span></span>|<span data-ttu-id="de802-134">字符串</span><span class="sxs-lookup"><span data-stu-id="de802-134">String</span></span>|<span data-ttu-id="de802-135">端加载关键的唯一 id。</span><span class="sxs-lookup"><span data-stu-id="de802-135">Side Loading Key Unique Id.</span></span>|
|<span data-ttu-id="de802-136">值</span><span class="sxs-lookup"><span data-stu-id="de802-136">value</span></span>|<span data-ttu-id="de802-137">字符串</span><span class="sxs-lookup"><span data-stu-id="de802-137">String</span></span>|<span data-ttu-id="de802-138">端加载密钥值是 5x5 的值，通过 hiphens 分隔。</span><span class="sxs-lookup"><span data-stu-id="de802-138">Side Loading Key Value, it is 5x5 value, seperated by hiphens.</span></span>|
|<span data-ttu-id="de802-139">displayName</span><span class="sxs-lookup"><span data-stu-id="de802-139">displayName</span></span>|<span data-ttu-id="de802-140">字符串</span><span class="sxs-lookup"><span data-stu-id="de802-140">String</span></span>|<span data-ttu-id="de802-141">端加载项显示名称为 it 专业人员管理员。</span><span class="sxs-lookup"><span data-stu-id="de802-141">Side Loading Key Name displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="de802-142">说明</span><span class="sxs-lookup"><span data-stu-id="de802-142">description</span></span>|<span data-ttu-id="de802-143">字符串</span><span class="sxs-lookup"><span data-stu-id="de802-143">String</span></span>|<span data-ttu-id="de802-144">显示为 it 专业人员 Admins 端加载项说明正在</span><span class="sxs-lookup"><span data-stu-id="de802-144">Side Loading Key description displayed to the ITPro Admins..</span></span>|
|<span data-ttu-id="de802-145">totalActivation</span><span class="sxs-lookup"><span data-stu-id="de802-145">totalActivation</span></span>|<span data-ttu-id="de802-146">Int32</span><span class="sxs-lookup"><span data-stu-id="de802-146">Int32</span></span>|<span data-ttu-id="de802-147">端加载项总激活向 it 专业人员 Admins 显示。</span><span class="sxs-lookup"><span data-stu-id="de802-147">Side Loading Key Total Activation displayed to the ITPro Admins.</span></span>|
|<span data-ttu-id="de802-148">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="de802-148">lastUpdatedDateTime</span></span>|<span data-ttu-id="de802-149">字符串</span><span class="sxs-lookup"><span data-stu-id="de802-149">String</span></span>|<span data-ttu-id="de802-150">端加载项上次更新日期向 it 专业人员 Admins 显示。</span><span class="sxs-lookup"><span data-stu-id="de802-150">Side Loading Key Last Updated Date displayed to the ITPro Admins.</span></span>|



## <a name="response"></a><span data-ttu-id="de802-151">响应</span><span class="sxs-lookup"><span data-stu-id="de802-151">Response</span></span>
<span data-ttu-id="de802-152">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md)对象。</span><span class="sxs-lookup"><span data-stu-id="de802-152">If successful, this method returns a `200 OK` response code and an updated [sideLoadingKey](../resources/intune-onboarding-sideloadingkey.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="de802-153">示例</span><span class="sxs-lookup"><span data-stu-id="de802-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="de802-154">请求</span><span class="sxs-lookup"><span data-stu-id="de802-154">Request</span></span>
<span data-ttu-id="de802-155">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="de802-155">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/sideLoadingKeys/{sideLoadingKeyId}
Content-type: application/json
Content-length: 193

{
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```

### <a name="response"></a><span data-ttu-id="de802-156">响应</span><span class="sxs-lookup"><span data-stu-id="de802-156">Response</span></span>
<span data-ttu-id="de802-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="de802-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 295

{
  "@odata.type": "#microsoft.graph.sideLoadingKey",
  "id": "21c4a3ff-a3ff-21c4-ffa3-c421ffa3c421",
  "value": "Value value",
  "displayName": "Display Name value",
  "description": "Description value",
  "totalActivation": 15,
  "lastUpdatedDateTime": "Last Updated Date Time value"
}
```





