---
title: 创建 windowsFeatureUpdateCatalogItem
description: 创建新的 windowsFeatureUpdateCatalogItem 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: af504a01a4a32e739bdc2faff823fc6192d5c8bd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51134359"
---
# <a name="create-windowsfeatureupdatecatalogitem"></a><span data-ttu-id="474e2-103">创建 windowsFeatureUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="474e2-103">Create windowsFeatureUpdateCatalogItem</span></span>

<span data-ttu-id="474e2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="474e2-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="474e2-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="474e2-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="474e2-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="474e2-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="474e2-107">创建新的 [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="474e2-107">Create a new [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="474e2-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="474e2-108">Prerequisites</span></span>
<span data-ttu-id="474e2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="474e2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="474e2-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="474e2-111">Permission type</span></span>|<span data-ttu-id="474e2-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="474e2-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="474e2-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="474e2-113">Delegated (work or school account)</span></span>|<span data-ttu-id="474e2-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="474e2-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="474e2-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="474e2-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="474e2-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="474e2-116">Not supported.</span></span>|
|<span data-ttu-id="474e2-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="474e2-117">Application</span></span>|<span data-ttu-id="474e2-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="474e2-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="474e2-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="474e2-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsUpdateCatalogItems
```

## <a name="request-headers"></a><span data-ttu-id="474e2-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="474e2-120">Request headers</span></span>
|<span data-ttu-id="474e2-121">标头</span><span class="sxs-lookup"><span data-stu-id="474e2-121">Header</span></span>|<span data-ttu-id="474e2-122">值</span><span class="sxs-lookup"><span data-stu-id="474e2-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="474e2-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="474e2-123">Authorization</span></span>|<span data-ttu-id="474e2-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="474e2-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="474e2-125">接受</span><span class="sxs-lookup"><span data-stu-id="474e2-125">Accept</span></span>|<span data-ttu-id="474e2-126">application/json</span><span class="sxs-lookup"><span data-stu-id="474e2-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="474e2-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="474e2-127">Request body</span></span>
<span data-ttu-id="474e2-128">在请求正文中，提供 windowsFeatureUpdateCatalogItem 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="474e2-128">In the request body, supply a JSON representation for the windowsFeatureUpdateCatalogItem object.</span></span>

<span data-ttu-id="474e2-129">下表显示创建 windowsFeatureUpdateCatalogItem 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="474e2-129">The following table shows the properties that are required when you create the windowsFeatureUpdateCatalogItem.</span></span>

|<span data-ttu-id="474e2-130">属性</span><span class="sxs-lookup"><span data-stu-id="474e2-130">Property</span></span>|<span data-ttu-id="474e2-131">类型</span><span class="sxs-lookup"><span data-stu-id="474e2-131">Type</span></span>|<span data-ttu-id="474e2-132">说明</span><span class="sxs-lookup"><span data-stu-id="474e2-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="474e2-133">id</span><span class="sxs-lookup"><span data-stu-id="474e2-133">id</span></span>|<span data-ttu-id="474e2-134">String</span><span class="sxs-lookup"><span data-stu-id="474e2-134">String</span></span>|<span data-ttu-id="474e2-135">目录项 ID。继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="474e2-135">The catalog item id. Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="474e2-136">displayName</span><span class="sxs-lookup"><span data-stu-id="474e2-136">displayName</span></span>|<span data-ttu-id="474e2-137">String</span><span class="sxs-lookup"><span data-stu-id="474e2-137">String</span></span>|<span data-ttu-id="474e2-138">目录显示名称列表。</span><span class="sxs-lookup"><span data-stu-id="474e2-138">The display name for the catalog item.</span></span> <span data-ttu-id="474e2-139">继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="474e2-139">Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="474e2-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="474e2-140">releaseDateTime</span></span>|<span data-ttu-id="474e2-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="474e2-141">DateTimeOffset</span></span>|<span data-ttu-id="474e2-142">目录项的发布日期 继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="474e2-142">The date the catalog item was released Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="474e2-143">version</span><span class="sxs-lookup"><span data-stu-id="474e2-143">version</span></span>|<span data-ttu-id="474e2-144">String</span><span class="sxs-lookup"><span data-stu-id="474e2-144">String</span></span>|<span data-ttu-id="474e2-145">功能更新版本</span><span class="sxs-lookup"><span data-stu-id="474e2-145">The feature update version</span></span>|



## <a name="response"></a><span data-ttu-id="474e2-146">响应</span><span class="sxs-lookup"><span data-stu-id="474e2-146">Response</span></span>
<span data-ttu-id="474e2-147">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="474e2-147">If successful, this method returns a `201 Created` response code and a [windowsFeatureUpdateCatalogItem](../resources/intune-softwareupdate-windowsfeatureupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="474e2-148">示例</span><span class="sxs-lookup"><span data-stu-id="474e2-148">Example</span></span>

### <a name="request"></a><span data-ttu-id="474e2-149">请求</span><span class="sxs-lookup"><span data-stu-id="474e2-149">Request</span></span>
<span data-ttu-id="474e2-150">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="474e2-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems
Content-type: application/json
Content-length: 203

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "version": "Version value"
}
```

### <a name="response"></a><span data-ttu-id="474e2-151">响应</span><span class="sxs-lookup"><span data-stu-id="474e2-151">Response</span></span>
<span data-ttu-id="474e2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="474e2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 252

{
  "@odata.type": "#microsoft.graph.windowsFeatureUpdateCatalogItem",
  "id": "cbd85729-5729-cbd8-2957-d8cb2957d8cb",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "version": "Version value"
}
```




