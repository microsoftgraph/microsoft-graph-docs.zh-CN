---
title: 创建 macOSSoftwareUpdateStateSummary
description: 创建新的 macOSSoftwareUpdateStateSummary 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a31fdb8581146969d8647a10f429999aeb6d2d0a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132637"
---
# <a name="create-macossoftwareupdatestatesummary"></a><span data-ttu-id="a9651-103">创建 macOSSoftwareUpdateStateSummary</span><span class="sxs-lookup"><span data-stu-id="a9651-103">Create macOSSoftwareUpdateStateSummary</span></span>

<span data-ttu-id="a9651-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a9651-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="a9651-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="a9651-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="a9651-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="a9651-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a9651-107">创建新的 [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a9651-107">Create a new [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a9651-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a9651-108">Prerequisites</span></span>
<span data-ttu-id="a9651-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a9651-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a9651-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a9651-111">Permission type</span></span>|<span data-ttu-id="a9651-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a9651-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a9651-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a9651-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a9651-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9651-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="a9651-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a9651-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a9651-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a9651-116">Not supported.</span></span>|
|<span data-ttu-id="a9651-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a9651-117">Application</span></span>|<span data-ttu-id="a9651-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a9651-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="a9651-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a9651-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries
```

## <a name="request-headers"></a><span data-ttu-id="a9651-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a9651-120">Request headers</span></span>
|<span data-ttu-id="a9651-121">标头</span><span class="sxs-lookup"><span data-stu-id="a9651-121">Header</span></span>|<span data-ttu-id="a9651-122">值</span><span class="sxs-lookup"><span data-stu-id="a9651-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a9651-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a9651-123">Authorization</span></span>|<span data-ttu-id="a9651-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a9651-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a9651-125">接受</span><span class="sxs-lookup"><span data-stu-id="a9651-125">Accept</span></span>|<span data-ttu-id="a9651-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a9651-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a9651-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a9651-127">Request body</span></span>
<span data-ttu-id="a9651-128">在请求正文中，提供 macOSSoftwareUpdateStateSummary 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a9651-128">In the request body, supply a JSON representation for the macOSSoftwareUpdateStateSummary object.</span></span>

<span data-ttu-id="a9651-129">下表显示创建 macOSSoftwareUpdateStateSummary 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a9651-129">The following table shows the properties that are required when you create the macOSSoftwareUpdateStateSummary.</span></span>

|<span data-ttu-id="a9651-130">属性</span><span class="sxs-lookup"><span data-stu-id="a9651-130">Property</span></span>|<span data-ttu-id="a9651-131">类型</span><span class="sxs-lookup"><span data-stu-id="a9651-131">Type</span></span>|<span data-ttu-id="a9651-132">说明</span><span class="sxs-lookup"><span data-stu-id="a9651-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a9651-133">id</span><span class="sxs-lookup"><span data-stu-id="a9651-133">id</span></span>|<span data-ttu-id="a9651-134">String</span><span class="sxs-lookup"><span data-stu-id="a9651-134">String</span></span>|<span data-ttu-id="a9651-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a9651-135">Key of the entity.</span></span>|
|<span data-ttu-id="a9651-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a9651-136">displayName</span></span>|<span data-ttu-id="a9651-137">String</span><span class="sxs-lookup"><span data-stu-id="a9651-137">String</span></span>|<span data-ttu-id="a9651-138">软件更新的可读名称</span><span class="sxs-lookup"><span data-stu-id="a9651-138">Human readable name of the software update</span></span>|
|<span data-ttu-id="a9651-139">productKey</span><span class="sxs-lookup"><span data-stu-id="a9651-139">productKey</span></span>|<span data-ttu-id="a9651-140">String</span><span class="sxs-lookup"><span data-stu-id="a9651-140">String</span></span>|<span data-ttu-id="a9651-141">软件更新的产品密钥。</span><span class="sxs-lookup"><span data-stu-id="a9651-141">Product key of the software update.</span></span>|
|<span data-ttu-id="a9651-142">updateCategory</span><span class="sxs-lookup"><span data-stu-id="a9651-142">updateCategory</span></span>|[<span data-ttu-id="a9651-143">macOSSoftwareUpdateCategory</span><span class="sxs-lookup"><span data-stu-id="a9651-143">macOSSoftwareUpdateCategory</span></span>](../resources/intune-deviceconfig-macossoftwareupdatecategory.md)|<span data-ttu-id="a9651-144">软件更新类别。</span><span class="sxs-lookup"><span data-stu-id="a9651-144">Software update category.</span></span> <span data-ttu-id="a9651-145">可取值为：`critical`、`configurationDataFile`、`firmware`、`other`。</span><span class="sxs-lookup"><span data-stu-id="a9651-145">Possible values are: `critical`, `configurationDataFile`, `firmware`, `other`.</span></span>|
|<span data-ttu-id="a9651-146">updateVersion</span><span class="sxs-lookup"><span data-stu-id="a9651-146">updateVersion</span></span>|<span data-ttu-id="a9651-147">String</span><span class="sxs-lookup"><span data-stu-id="a9651-147">String</span></span>|<span data-ttu-id="a9651-148">软件更新的版本</span><span class="sxs-lookup"><span data-stu-id="a9651-148">Version of the software update</span></span>|
|<span data-ttu-id="a9651-149">state</span><span class="sxs-lookup"><span data-stu-id="a9651-149">state</span></span>|[<span data-ttu-id="a9651-150">macOSSoftwareUpdateState</span><span class="sxs-lookup"><span data-stu-id="a9651-150">macOSSoftwareUpdateState</span></span>](../resources/intune-deviceconfig-macossoftwareupdatestate.md)|<span data-ttu-id="a9651-151">软件更新的状态。</span><span class="sxs-lookup"><span data-stu-id="a9651-151">State of the software update.</span></span> <span data-ttu-id="a9651-152">可能的值是 `success` `downloading` `downloaded` ：、、、、、、、、、、 `installing` `idle` `available` `scheduled` `downloadFailed` `downloadInsufficientSpace` `downloadInsufficientPower` `downloadInsufficientNetwork` `installInsufficientSpace` `installInsufficientPower` `installFailed` `commandFailed` 。</span><span class="sxs-lookup"><span data-stu-id="a9651-152">Possible values are: `success`, `downloading`, `downloaded`, `installing`, `idle`, `available`, `scheduled`, `downloadFailed`, `downloadInsufficientSpace`, `downloadInsufficientPower`, `downloadInsufficientNetwork`, `installInsufficientSpace`, `installInsufficientPower`, `installFailed`, `commandFailed`.</span></span>|
|<span data-ttu-id="a9651-153">lastUpdatedDateTime</span><span class="sxs-lookup"><span data-stu-id="a9651-153">lastUpdatedDateTime</span></span>|<span data-ttu-id="a9651-154">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a9651-154">DateTimeOffset</span></span>|<span data-ttu-id="a9651-155">上次更新此设备和产品密钥报告的日期时间。</span><span class="sxs-lookup"><span data-stu-id="a9651-155">Last date time the report for this device and product key was updated.</span></span>|



## <a name="response"></a><span data-ttu-id="a9651-156">响应</span><span class="sxs-lookup"><span data-stu-id="a9651-156">Response</span></span>
<span data-ttu-id="a9651-157">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a9651-157">If successful, this method returns a `201 Created` response code and a [macOSSoftwareUpdateStateSummary](../resources/intune-deviceconfig-macossoftwareupdatestatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a9651-158">示例</span><span class="sxs-lookup"><span data-stu-id="a9651-158">Example</span></span>

### <a name="request"></a><span data-ttu-id="a9651-159">请求</span><span class="sxs-lookup"><span data-stu-id="a9651-159">Request</span></span>
<span data-ttu-id="a9651-160">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a9651-160">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/macOSSoftwareUpdateAccountSummaries/{macOSSoftwareUpdateAccountSummaryId}/categorySummaries/{macOSSoftwareUpdateCategorySummaryId}/updateStateSummaries
Content-type: application/json
Content-length: 331

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateStateSummary",
  "displayName": "Display Name value",
  "productKey": "Product Key value",
  "updateCategory": "configurationDataFile",
  "updateVersion": "Update Version value",
  "state": "downloading",
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```

### <a name="response"></a><span data-ttu-id="a9651-161">响应</span><span class="sxs-lookup"><span data-stu-id="a9651-161">Response</span></span>
<span data-ttu-id="a9651-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a9651-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 380

{
  "@odata.type": "#microsoft.graph.macOSSoftwareUpdateStateSummary",
  "id": "9527a1df-a1df-9527-dfa1-2795dfa12795",
  "displayName": "Display Name value",
  "productKey": "Product Key value",
  "updateCategory": "configurationDataFile",
  "updateVersion": "Update Version value",
  "state": "downloading",
  "lastUpdatedDateTime": "2017-01-01T00:00:56.8321556-08:00"
}
```




