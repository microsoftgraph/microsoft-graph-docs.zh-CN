---
title: 创建 windowsQualityUpdateCatalogItem
description: 创建新的 windowsQualityUpdateCatalogItem 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ad143f79bdabc99dadef3009bc10d55263acca1d
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50160212"
---
# <a name="create-windowsqualityupdatecatalogitem"></a><span data-ttu-id="62a0b-103">创建 windowsQualityUpdateCatalogItem</span><span class="sxs-lookup"><span data-stu-id="62a0b-103">Create windowsQualityUpdateCatalogItem</span></span>

<span data-ttu-id="62a0b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="62a0b-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="62a0b-105">**重要提示：** /beta 版本的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="62a0b-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="62a0b-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="62a0b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="62a0b-107">创建新的 [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="62a0b-107">Create a new [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="62a0b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="62a0b-108">Prerequisites</span></span>
<span data-ttu-id="62a0b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="62a0b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="62a0b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="62a0b-111">Permission type</span></span>|<span data-ttu-id="62a0b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="62a0b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="62a0b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="62a0b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="62a0b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62a0b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="62a0b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="62a0b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="62a0b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="62a0b-116">Not supported.</span></span>|
|<span data-ttu-id="62a0b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="62a0b-117">Application</span></span>|<span data-ttu-id="62a0b-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="62a0b-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="62a0b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="62a0b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsUpdateCatalogItems
```

## <a name="request-headers"></a><span data-ttu-id="62a0b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="62a0b-120">Request headers</span></span>
|<span data-ttu-id="62a0b-121">标头</span><span class="sxs-lookup"><span data-stu-id="62a0b-121">Header</span></span>|<span data-ttu-id="62a0b-122">值</span><span class="sxs-lookup"><span data-stu-id="62a0b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="62a0b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="62a0b-123">Authorization</span></span>|<span data-ttu-id="62a0b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="62a0b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="62a0b-125">接受</span><span class="sxs-lookup"><span data-stu-id="62a0b-125">Accept</span></span>|<span data-ttu-id="62a0b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="62a0b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="62a0b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="62a0b-127">Request body</span></span>
<span data-ttu-id="62a0b-128">在请求正文中，提供 windowsQualityUpdateCatalogItem 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="62a0b-128">In the request body, supply a JSON representation for the windowsQualityUpdateCatalogItem object.</span></span>

<span data-ttu-id="62a0b-129">下表显示创建 windowsQualityUpdateCatalogItem 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="62a0b-129">The following table shows the properties that are required when you create the windowsQualityUpdateCatalogItem.</span></span>

|<span data-ttu-id="62a0b-130">属性</span><span class="sxs-lookup"><span data-stu-id="62a0b-130">Property</span></span>|<span data-ttu-id="62a0b-131">类型</span><span class="sxs-lookup"><span data-stu-id="62a0b-131">Type</span></span>|<span data-ttu-id="62a0b-132">说明</span><span class="sxs-lookup"><span data-stu-id="62a0b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="62a0b-133">id</span><span class="sxs-lookup"><span data-stu-id="62a0b-133">id</span></span>|<span data-ttu-id="62a0b-134">String</span><span class="sxs-lookup"><span data-stu-id="62a0b-134">String</span></span>|<span data-ttu-id="62a0b-135">目录项 ID。继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="62a0b-135">The catalog item id. Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="62a0b-136">displayName</span><span class="sxs-lookup"><span data-stu-id="62a0b-136">displayName</span></span>|<span data-ttu-id="62a0b-137">String</span><span class="sxs-lookup"><span data-stu-id="62a0b-137">String</span></span>|<span data-ttu-id="62a0b-138">目录显示名称列表。</span><span class="sxs-lookup"><span data-stu-id="62a0b-138">The display name for the catalog item.</span></span> <span data-ttu-id="62a0b-139">继承自 [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="62a0b-139">Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="62a0b-140">releaseDateTime</span><span class="sxs-lookup"><span data-stu-id="62a0b-140">releaseDateTime</span></span>|<span data-ttu-id="62a0b-141">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="62a0b-141">DateTimeOffset</span></span>|<span data-ttu-id="62a0b-142">目录项的发布日期 继承 [自 windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span><span class="sxs-lookup"><span data-stu-id="62a0b-142">The date the catalog item was released Inherited from [windowsUpdateCatalogItem](../resources/intune-softwareupdate-windowsupdatecatalogitem.md)</span></span>|
|<span data-ttu-id="62a0b-143">kbArticleId</span><span class="sxs-lookup"><span data-stu-id="62a0b-143">kbArticleId</span></span>|<span data-ttu-id="62a0b-144">String</span><span class="sxs-lookup"><span data-stu-id="62a0b-144">String</span></span>|<span data-ttu-id="62a0b-145">知识库文章 ID</span><span class="sxs-lookup"><span data-stu-id="62a0b-145">Knowledge base article id</span></span>|
|<span data-ttu-id="62a0b-146">classification</span><span class="sxs-lookup"><span data-stu-id="62a0b-146">classification</span></span>|[<span data-ttu-id="62a0b-147">windowsQualityUpdateClassification</span><span class="sxs-lookup"><span data-stu-id="62a0b-147">windowsQualityUpdateClassification</span></span>](../resources/intune-softwareupdate-windowsqualityupdateclassification.md)|<span data-ttu-id="62a0b-148">质量更新的分类。</span><span class="sxs-lookup"><span data-stu-id="62a0b-148">Classification of the quality update.</span></span> <span data-ttu-id="62a0b-149">可取值为：`all`、`security`、`nonSecurity`。</span><span class="sxs-lookup"><span data-stu-id="62a0b-149">Possible values are: `all`, `security`, `nonSecurity`.</span></span>|
|<span data-ttu-id="62a0b-150">isExpeditable</span><span class="sxs-lookup"><span data-stu-id="62a0b-150">isExpeditable</span></span>|<span data-ttu-id="62a0b-151">布尔</span><span class="sxs-lookup"><span data-stu-id="62a0b-151">Boolean</span></span>|<span data-ttu-id="62a0b-152">指示更新是否符合加速条件的标志</span><span class="sxs-lookup"><span data-stu-id="62a0b-152">Flag indicating if update qualifies for expedite</span></span>|



## <a name="response"></a><span data-ttu-id="62a0b-153">响应</span><span class="sxs-lookup"><span data-stu-id="62a0b-153">Response</span></span>
<span data-ttu-id="62a0b-154">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="62a0b-154">If successful, this method returns a `201 Created` response code and a [windowsQualityUpdateCatalogItem](../resources/intune-softwareupdate-windowsqualityupdatecatalogitem.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="62a0b-155">示例</span><span class="sxs-lookup"><span data-stu-id="62a0b-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="62a0b-156">请求</span><span class="sxs-lookup"><span data-stu-id="62a0b-156">Request</span></span>
<span data-ttu-id="62a0b-157">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="62a0b-157">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsUpdateCatalogItems
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

### <a name="response"></a><span data-ttu-id="62a0b-158">响应</span><span class="sxs-lookup"><span data-stu-id="62a0b-158">Response</span></span>
<span data-ttu-id="62a0b-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="62a0b-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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




