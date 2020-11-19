---
title: 创建 configManagerCollection
description: 创建新的 configManagerCollection 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a16a878140e233e44960d842687f05f0c2c7a79e
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49301577"
---
# <a name="create-configmanagercollection"></a><span data-ttu-id="3c3af-103">创建 configManagerCollection</span><span class="sxs-lookup"><span data-stu-id="3c3af-103">Create configManagerCollection</span></span>

<span data-ttu-id="3c3af-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c3af-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c3af-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3c3af-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c3af-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c3af-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c3af-107">创建新的 [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3c3af-107">Create a new [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c3af-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3c3af-108">Prerequisites</span></span>
<span data-ttu-id="3c3af-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c3af-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c3af-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c3af-111">Permission type</span></span>|<span data-ttu-id="3c3af-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3c3af-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c3af-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c3af-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c3af-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c3af-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3c3af-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c3af-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c3af-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c3af-116">Not supported.</span></span>|
|<span data-ttu-id="3c3af-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c3af-117">Application</span></span>|<span data-ttu-id="3c3af-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c3af-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c3af-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c3af-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/configManagerCollections
```

## <a name="request-headers"></a><span data-ttu-id="3c3af-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c3af-120">Request headers</span></span>
|<span data-ttu-id="3c3af-121">标头</span><span class="sxs-lookup"><span data-stu-id="3c3af-121">Header</span></span>|<span data-ttu-id="3c3af-122">值</span><span class="sxs-lookup"><span data-stu-id="3c3af-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c3af-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c3af-123">Authorization</span></span>|<span data-ttu-id="3c3af-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3c3af-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c3af-125">接受</span><span class="sxs-lookup"><span data-stu-id="3c3af-125">Accept</span></span>|<span data-ttu-id="3c3af-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c3af-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c3af-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c3af-127">Request body</span></span>
<span data-ttu-id="3c3af-128">在请求正文中，提供 configManagerCollection 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c3af-128">In the request body, supply a JSON representation for the configManagerCollection object.</span></span>

<span data-ttu-id="3c3af-129">下表显示创建 configManagerCollection 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3c3af-129">The following table shows the properties that are required when you create the configManagerCollection.</span></span>

|<span data-ttu-id="3c3af-130">属性</span><span class="sxs-lookup"><span data-stu-id="3c3af-130">Property</span></span>|<span data-ttu-id="3c3af-131">类型</span><span class="sxs-lookup"><span data-stu-id="3c3af-131">Type</span></span>|<span data-ttu-id="3c3af-132">说明</span><span class="sxs-lookup"><span data-stu-id="3c3af-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c3af-133">id</span><span class="sxs-lookup"><span data-stu-id="3c3af-133">id</span></span>|<span data-ttu-id="3c3af-134">字符串</span><span class="sxs-lookup"><span data-stu-id="3c3af-134">String</span></span>|<span data-ttu-id="3c3af-135">ConfigManager 集合的键。</span><span class="sxs-lookup"><span data-stu-id="3c3af-135">The key for the ConfigManager Collection.</span></span>|
|<span data-ttu-id="3c3af-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3c3af-136">displayName</span></span>|<span data-ttu-id="3c3af-137">字符串</span><span class="sxs-lookup"><span data-stu-id="3c3af-137">String</span></span>|<span data-ttu-id="3c3af-138">DisplayName。</span><span class="sxs-lookup"><span data-stu-id="3c3af-138">The DisplayName.</span></span>|
|<span data-ttu-id="3c3af-139">collectionIdentifier</span><span class="sxs-lookup"><span data-stu-id="3c3af-139">collectionIdentifier</span></span>|<span data-ttu-id="3c3af-140">字符串</span><span class="sxs-lookup"><span data-stu-id="3c3af-140">String</span></span>|<span data-ttu-id="3c3af-141">SCCM 中的集合标识符。</span><span class="sxs-lookup"><span data-stu-id="3c3af-141">The collection identifier in SCCM.</span></span>|
|<span data-ttu-id="3c3af-142">hierarchyName</span><span class="sxs-lookup"><span data-stu-id="3c3af-142">hierarchyName</span></span>|<span data-ttu-id="3c3af-143">字符串</span><span class="sxs-lookup"><span data-stu-id="3c3af-143">String</span></span>|<span data-ttu-id="3c3af-144">HierarchyName。</span><span class="sxs-lookup"><span data-stu-id="3c3af-144">The HierarchyName.</span></span>|
|<span data-ttu-id="3c3af-145">hierarchyIdentifier</span><span class="sxs-lookup"><span data-stu-id="3c3af-145">hierarchyIdentifier</span></span>|<span data-ttu-id="3c3af-146">字符串</span><span class="sxs-lookup"><span data-stu-id="3c3af-146">String</span></span>|<span data-ttu-id="3c3af-147">层次结构标识符。</span><span class="sxs-lookup"><span data-stu-id="3c3af-147">The Hierarchy Identifier.</span></span>|
|<span data-ttu-id="3c3af-148">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="3c3af-148">createdDateTime</span></span>|<span data-ttu-id="3c3af-149">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c3af-149">DateTimeOffset</span></span>|<span data-ttu-id="3c3af-150">创建日期。</span><span class="sxs-lookup"><span data-stu-id="3c3af-150">The created date.</span></span>|
|<span data-ttu-id="3c3af-151">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c3af-151">lastModifiedDateTime</span></span>|<span data-ttu-id="3c3af-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c3af-152">DateTimeOffset</span></span>|<span data-ttu-id="3c3af-153">上次修改日期。</span><span class="sxs-lookup"><span data-stu-id="3c3af-153">The last modified date.</span></span>|



## <a name="response"></a><span data-ttu-id="3c3af-154">响应</span><span class="sxs-lookup"><span data-stu-id="3c3af-154">Response</span></span>
<span data-ttu-id="3c3af-155">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3c3af-155">If successful, this method returns a `201 Created` response code and a [configManagerCollection](../resources/intune-partnerintegration-configmanagercollection.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c3af-156">示例</span><span class="sxs-lookup"><span data-stu-id="3c3af-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c3af-157">请求</span><span class="sxs-lookup"><span data-stu-id="3c3af-157">Request</span></span>
<span data-ttu-id="3c3af-158">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c3af-158">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/configManagerCollections
Content-type: application/json
Content-length: 263

{
  "@odata.type": "#microsoft.graph.configManagerCollection",
  "displayName": "Display Name value",
  "collectionIdentifier": "Collection Identifier value",
  "hierarchyName": "Hierarchy Name value",
  "hierarchyIdentifier": "Hierarchy Identifier value"
}
```

### <a name="response"></a><span data-ttu-id="3c3af-159">响应</span><span class="sxs-lookup"><span data-stu-id="3c3af-159">Response</span></span>
<span data-ttu-id="3c3af-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3c3af-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 435

{
  "@odata.type": "#microsoft.graph.configManagerCollection",
  "id": "5f9d1d76-1d76-5f9d-761d-9d5f761d9d5f",
  "displayName": "Display Name value",
  "collectionIdentifier": "Collection Identifier value",
  "hierarchyName": "Hierarchy Name value",
  "hierarchyIdentifier": "Hierarchy Identifier value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```




