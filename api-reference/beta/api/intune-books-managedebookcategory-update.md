---
title: 更新 managedEBookCategory
description: 更新 managedEBookCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: bbc5436c7f4140d1c2cd517b42468b67109c6fd5
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43414093"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="3c0de-103">更新 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="3c0de-103">Update managedEBookCategory</span></span>

<span data-ttu-id="3c0de-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3c0de-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="3c0de-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="3c0de-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="3c0de-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="3c0de-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3c0de-107">更新[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="3c0de-107">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="3c0de-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="3c0de-108">Prerequisites</span></span>
<span data-ttu-id="3c0de-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3c0de-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3c0de-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="3c0de-111">Permission type</span></span>|<span data-ttu-id="3c0de-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="3c0de-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3c0de-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3c0de-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3c0de-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c0de-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3c0de-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3c0de-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3c0de-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3c0de-116">Not supported.</span></span>|
|<span data-ttu-id="3c0de-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="3c0de-117">Application</span></span>|<span data-ttu-id="3c0de-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3c0de-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="3c0de-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3c0de-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="3c0de-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="3c0de-120">Request headers</span></span>
|<span data-ttu-id="3c0de-121">标头</span><span class="sxs-lookup"><span data-stu-id="3c0de-121">Header</span></span>|<span data-ttu-id="3c0de-122">值</span><span class="sxs-lookup"><span data-stu-id="3c0de-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3c0de-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3c0de-123">Authorization</span></span>|<span data-ttu-id="3c0de-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="3c0de-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3c0de-125">接受</span><span class="sxs-lookup"><span data-stu-id="3c0de-125">Accept</span></span>|<span data-ttu-id="3c0de-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3c0de-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3c0de-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3c0de-127">Request body</span></span>
<span data-ttu-id="3c0de-128">在请求正文中，提供[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3c0de-128">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="3c0de-129">下表显示创建[managedEBookCategory](../resources/intune-books-managedebookcategory.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3c0de-129">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="3c0de-130">属性</span><span class="sxs-lookup"><span data-stu-id="3c0de-130">Property</span></span>|<span data-ttu-id="3c0de-131">类型</span><span class="sxs-lookup"><span data-stu-id="3c0de-131">Type</span></span>|<span data-ttu-id="3c0de-132">说明</span><span class="sxs-lookup"><span data-stu-id="3c0de-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3c0de-133">id</span><span class="sxs-lookup"><span data-stu-id="3c0de-133">id</span></span>|<span data-ttu-id="3c0de-134">String</span><span class="sxs-lookup"><span data-stu-id="3c0de-134">String</span></span>|<span data-ttu-id="3c0de-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="3c0de-135">The key of the entity.</span></span>|
|<span data-ttu-id="3c0de-136">displayName</span><span class="sxs-lookup"><span data-stu-id="3c0de-136">displayName</span></span>|<span data-ttu-id="3c0de-137">String</span><span class="sxs-lookup"><span data-stu-id="3c0de-137">String</span></span>|<span data-ttu-id="3c0de-138">电子书类别的名称。</span><span class="sxs-lookup"><span data-stu-id="3c0de-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="3c0de-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="3c0de-139">lastModifiedDateTime</span></span>|<span data-ttu-id="3c0de-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3c0de-140">DateTimeOffset</span></span>|<span data-ttu-id="3c0de-141">上次修改 ManagedEBookCategory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3c0de-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="3c0de-142">响应</span><span class="sxs-lookup"><span data-stu-id="3c0de-142">Response</span></span>
<span data-ttu-id="3c0de-143">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="3c0de-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3c0de-144">示例</span><span class="sxs-lookup"><span data-stu-id="3c0de-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="3c0de-145">请求</span><span class="sxs-lookup"><span data-stu-id="3c0de-145">Request</span></span>
<span data-ttu-id="3c0de-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="3c0de-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="3c0de-147">响应</span><span class="sxs-lookup"><span data-stu-id="3c0de-147">Response</span></span>
<span data-ttu-id="3c0de-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3c0de-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 215

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "id": "3c71fb14-fb14-3c71-14fb-713c14fb713c",
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```



