---
title: 创建 managedEBookCategory
description: 创建新的 managedEBookCategory 对象。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b3d59e4b8e31a894c30237b96ddb524478a420f4
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43392223"
---
# <a name="create-managedebookcategory"></a><span data-ttu-id="bd8a1-103">创建 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="bd8a1-103">Create managedEBookCategory</span></span>

<span data-ttu-id="bd8a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bd8a1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="bd8a1-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="bd8a1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="bd8a1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="bd8a1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="bd8a1-107">创建新的[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bd8a1-107">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="bd8a1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="bd8a1-108">Prerequisites</span></span>
<span data-ttu-id="bd8a1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="bd8a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="bd8a1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="bd8a1-111">Permission type</span></span>|<span data-ttu-id="bd8a1-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="bd8a1-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="bd8a1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="bd8a1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="bd8a1-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd8a1-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="bd8a1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="bd8a1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="bd8a1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="bd8a1-116">Not supported.</span></span>|
|<span data-ttu-id="bd8a1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="bd8a1-117">Application</span></span>|<span data-ttu-id="bd8a1-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="bd8a1-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="bd8a1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="bd8a1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBookCategories
POST /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="bd8a1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="bd8a1-120">Request headers</span></span>
|<span data-ttu-id="bd8a1-121">标头</span><span class="sxs-lookup"><span data-stu-id="bd8a1-121">Header</span></span>|<span data-ttu-id="bd8a1-122">值</span><span class="sxs-lookup"><span data-stu-id="bd8a1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="bd8a1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="bd8a1-123">Authorization</span></span>|<span data-ttu-id="bd8a1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="bd8a1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="bd8a1-125">接受</span><span class="sxs-lookup"><span data-stu-id="bd8a1-125">Accept</span></span>|<span data-ttu-id="bd8a1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="bd8a1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="bd8a1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="bd8a1-127">Request body</span></span>
<span data-ttu-id="bd8a1-128">在请求正文中，提供 managedEBookCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bd8a1-128">In the request body, supply a JSON representation for the managedEBookCategory object.</span></span>

<span data-ttu-id="bd8a1-129">下表显示创建 managedEBookCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="bd8a1-129">The following table shows the properties that are required when you create the managedEBookCategory.</span></span>

|<span data-ttu-id="bd8a1-130">属性</span><span class="sxs-lookup"><span data-stu-id="bd8a1-130">Property</span></span>|<span data-ttu-id="bd8a1-131">类型</span><span class="sxs-lookup"><span data-stu-id="bd8a1-131">Type</span></span>|<span data-ttu-id="bd8a1-132">说明</span><span class="sxs-lookup"><span data-stu-id="bd8a1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="bd8a1-133">id</span><span class="sxs-lookup"><span data-stu-id="bd8a1-133">id</span></span>|<span data-ttu-id="bd8a1-134">字符串</span><span class="sxs-lookup"><span data-stu-id="bd8a1-134">String</span></span>|<span data-ttu-id="bd8a1-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="bd8a1-135">The key of the entity.</span></span>|
|<span data-ttu-id="bd8a1-136">displayName</span><span class="sxs-lookup"><span data-stu-id="bd8a1-136">displayName</span></span>|<span data-ttu-id="bd8a1-137">String</span><span class="sxs-lookup"><span data-stu-id="bd8a1-137">String</span></span>|<span data-ttu-id="bd8a1-138">电子书类别的名称。</span><span class="sxs-lookup"><span data-stu-id="bd8a1-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="bd8a1-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="bd8a1-139">lastModifiedDateTime</span></span>|<span data-ttu-id="bd8a1-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bd8a1-140">DateTimeOffset</span></span>|<span data-ttu-id="bd8a1-141">上次修改 ManagedEBookCategory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bd8a1-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="bd8a1-142">响应</span><span class="sxs-lookup"><span data-stu-id="bd8a1-142">Response</span></span>
<span data-ttu-id="bd8a1-143">如果成功，此方法在响应`201 Created`正文中返回响应代码和[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="bd8a1-143">If successful, this method returns a `201 Created` response code and a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="bd8a1-144">示例</span><span class="sxs-lookup"><span data-stu-id="bd8a1-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="bd8a1-145">请求</span><span class="sxs-lookup"><span data-stu-id="bd8a1-145">Request</span></span>
<span data-ttu-id="bd8a1-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="bd8a1-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="bd8a1-147">响应</span><span class="sxs-lookup"><span data-stu-id="bd8a1-147">Response</span></span>
<span data-ttu-id="bd8a1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="bd8a1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



