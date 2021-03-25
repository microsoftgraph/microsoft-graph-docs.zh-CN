---
title: 更新 windowsQualityUpdateCatalogItem
description: 更新 windowsQualityUpdateCatalogItem 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 1263a65399dea4bbae5d326ca01dd0bf17c3facd
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51156259"
---
# <a name="update-windowsqualityupdatecatalogitem"></a><span data-ttu-id="99c63-103">更新 windowsQualityUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="99c63-103">Update windowsQualityUpdateCatalogItem</span></span>

<span data-ttu-id="99c63-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="99c63-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="99c63-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="99c63-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="99c63-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="99c63-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="99c63-107">更新 [windowsQualityUpdateCatalogItem 对象](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="99c63-107">Update the properties of a [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="99c63-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="99c63-108">Prerequisites</span></span>
<span data-ttu-id="99c63-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="99c63-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="99c63-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="99c63-111">Permission type</span></span>|<span data-ttu-id="99c63-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="99c63-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="99c63-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="99c63-113">Delegated (work or school account)</span></span>|<span data-ttu-id="99c63-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99c63-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="99c63-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="99c63-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="99c63-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="99c63-116">Not supported.</span></span>|
|<span data-ttu-id="99c63-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="99c63-117">Application</span></span>|<span data-ttu-id="99c63-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="99c63-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="99c63-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="99c63-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
```

## <a name="request-headers"></a><span data-ttu-id="99c63-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="99c63-120">Request headers</span></span>
|<span data-ttu-id="99c63-121">标头</span><span class="sxs-lookup"><span data-stu-id="99c63-121">Header</span></span>|<span data-ttu-id="99c63-122">值</span><span class="sxs-lookup"><span data-stu-id="99c63-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="99c63-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="99c63-123">Authorization</span></span>|<span data-ttu-id="99c63-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="99c63-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="99c63-125">接受</span><span class="sxs-lookup"><span data-stu-id="99c63-125">Accept</span></span>|<span data-ttu-id="99c63-126">application/json</span><span class="sxs-lookup"><span data-stu-id="99c63-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="99c63-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="99c63-127">Request body</span></span>
<span data-ttu-id="99c63-128">在请求正文中，提供 [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="99c63-128">In the request body, supply a JSON representation for the [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object.</span></span>

<span data-ttu-id="99c63-129">下表显示创建 [windowsQualityUpdateCatalogItem 时所需的属性](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md)。</span><span class="sxs-lookup"><span data-stu-id="99c63-129">The following table shows the properties that are required when you create the [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md).</span></span>

|<span data-ttu-id="99c63-130">属性</span><span class="sxs-lookup"><span data-stu-id="99c63-130">Property</span></span>|<span data-ttu-id="99c63-131">类型</span><span class="sxs-lookup"><span data-stu-id="99c63-131">Type</span></span>|<span data-ttu-id="99c63-132">说明</span><span class="sxs-lookup"><span data-stu-id="99c63-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="99c63-133">id</span><span class="sxs-lookup"><span data-stu-id="99c63-133">id</span></span>|<span data-ttu-id="99c63-134">String</span><span class="sxs-lookup"><span data-stu-id="99c63-134">String</span></span>|<span data-ttu-id="99c63-135">目录项 ID。继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="99c63-135">The catalog item id. Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="99c63-136">displayName</span><span class="sxs-lookup"><span data-stu-id="99c63-136">displayName</span></span>|<span data-ttu-id="99c63-137">String</span><span class="sxs-lookup"><span data-stu-id="99c63-137">String</span></span>|<span data-ttu-id="99c63-138">目录显示名称列表。</span><span class="sxs-lookup"><span data-stu-id="99c63-138">The display name for the catalog item.</span></span> <span data-ttu-id="99c63-139">继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="99c63-139">Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="99c63-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="99c63-140">releaseDateTime</span></span>|<span data-ttu-id="99c63-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="99c63-141">DateTimeOffset</span></span>|<span data-ttu-id="99c63-142">目录项的发布日期 继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="99c63-142">The date the catalog item was released Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="99c63-143">kbArticleId</span><span class="sxs-lookup"><span data-stu-id="99c63-143">kbArticleId</span></span>|<span data-ttu-id="99c63-144">String</span><span class="sxs-lookup"><span data-stu-id="99c63-144">String</span></span>|<span data-ttu-id="99c63-145">知识库文章 ID</span><span class="sxs-lookup"><span data-stu-id="99c63-145">Knowledge base article id</span></span>|
|<span data-ttu-id="99c63-146">classification</span><span class="sxs-lookup"><span data-stu-id="99c63-146">classification</span></span>|[<span data-ttu-id="99c63-147">windowsQualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="99c63-147">windowsQualityUpdateClassification</span></span>](../resources/intune-softwareupdate-windowsqualityupdateclassification.md)|<span data-ttu-id="99c63-148">质量更新的分类。</span><span class="sxs-lookup"><span data-stu-id="99c63-148">Classification of the quality update.</span></span> <span data-ttu-id="99c63-149">可取值为：`all`、`security`、`nonSecurity`。</span><span class="sxs-lookup"><span data-stu-id="99c63-149">Possible values are: `all`, `security`, `nonSecurity`.</span></span>|
|<span data-ttu-id="99c63-150">isExpeditable</span><span class="sxs-lookup"><span data-stu-id="99c63-150">isExpeditable</span></span>|<span data-ttu-id="99c63-151">Boolean</span><span class="sxs-lookup"><span data-stu-id="99c63-151">Boolean</span></span>|<span data-ttu-id="99c63-152">指示更新是否符合加速条件的标志</span><span class="sxs-lookup"><span data-stu-id="99c63-152">Flag indicating if update qualifies for expedite</span></span>|



## <a name="response"></a><span data-ttu-id="99c63-153">响应</span><span class="sxs-lookup"><span data-stu-id="99c63-153">Response</span></span>
<span data-ttu-id="99c63-154">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="99c63-154">If successful, this method returns a `200 OK` response code and an updated [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="99c63-155">示例</span><span class="sxs-lookup"><span data-stu-id="99c63-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="99c63-156">请求</span><span class="sxs-lookup"><span data-stu-id="99c63-156">Request</span></span>
<span data-ttu-id="99c63-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="99c63-157">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems/{windowsUpdateCatalogItemId}
Content-type: application/json
Content-length: 272

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "kbArticleId": "Kb Article Id value",
  "classification": "security",
  "isExpeditable": true
}
```

### <a name="response"></a><span data-ttu-id="99c63-158">响应</span><span class="sxs-lookup"><span data-stu-id="99c63-158">Response</span></span>
<span data-ttu-id="99c63-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="99c63-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 321

{
  "@odata.type": "#microsoft.graph.windowsQualityUpdateCatalogItem",
  "id": "8eb831ba-31ba-8eb8-ba31-b88eba31b88e",
  "displayName": "Display Name value",
  "releaseDateTime": "2017-01-01T00:01:34.7470482-08:00",
  "kbArticleId": "Kb Article Id value",
  "classification": "security",
  "isExpeditable": true
}
```




