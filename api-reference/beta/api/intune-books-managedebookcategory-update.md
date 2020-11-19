---
title: 更新 managedEBookCategory
description: 更新 managedEBookCategory 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: d126ab73c26543815d734abf6105c932a64f555f
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49244757"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="b9eff-103">更新 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="b9eff-103">Update managedEBookCategory</span></span>

<span data-ttu-id="b9eff-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b9eff-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="b9eff-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="b9eff-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b9eff-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b9eff-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b9eff-107">更新 [managedEBookCategory](../resources/intune-books-managedebookcategory.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="b9eff-107">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b9eff-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b9eff-108">Prerequisites</span></span>
<span data-ttu-id="b9eff-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b9eff-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b9eff-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b9eff-111">Permission type</span></span>|<span data-ttu-id="b9eff-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b9eff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b9eff-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b9eff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b9eff-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9eff-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="b9eff-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b9eff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b9eff-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b9eff-116">Not supported.</span></span>|
|<span data-ttu-id="b9eff-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b9eff-117">Application</span></span>|<span data-ttu-id="b9eff-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b9eff-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="b9eff-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b9eff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="b9eff-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b9eff-120">Request headers</span></span>
|<span data-ttu-id="b9eff-121">标头</span><span class="sxs-lookup"><span data-stu-id="b9eff-121">Header</span></span>|<span data-ttu-id="b9eff-122">值</span><span class="sxs-lookup"><span data-stu-id="b9eff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b9eff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b9eff-123">Authorization</span></span>|<span data-ttu-id="b9eff-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b9eff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b9eff-125">接受</span><span class="sxs-lookup"><span data-stu-id="b9eff-125">Accept</span></span>|<span data-ttu-id="b9eff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b9eff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b9eff-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b9eff-127">Request body</span></span>
<span data-ttu-id="b9eff-128">在请求正文中，提供 [managedEBookCategory](../resources/intune-books-managedebookcategory.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9eff-128">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="b9eff-129">下表显示创建 [managedEBookCategory](../resources/intune-books-managedebookcategory.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b9eff-129">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="b9eff-130">属性</span><span class="sxs-lookup"><span data-stu-id="b9eff-130">Property</span></span>|<span data-ttu-id="b9eff-131">类型</span><span class="sxs-lookup"><span data-stu-id="b9eff-131">Type</span></span>|<span data-ttu-id="b9eff-132">说明</span><span class="sxs-lookup"><span data-stu-id="b9eff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b9eff-133">id</span><span class="sxs-lookup"><span data-stu-id="b9eff-133">id</span></span>|<span data-ttu-id="b9eff-134">String</span><span class="sxs-lookup"><span data-stu-id="b9eff-134">String</span></span>|<span data-ttu-id="b9eff-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="b9eff-135">The key of the entity.</span></span>|
|<span data-ttu-id="b9eff-136">displayName</span><span class="sxs-lookup"><span data-stu-id="b9eff-136">displayName</span></span>|<span data-ttu-id="b9eff-137">String</span><span class="sxs-lookup"><span data-stu-id="b9eff-137">String</span></span>|<span data-ttu-id="b9eff-138">电子书类别的名称。</span><span class="sxs-lookup"><span data-stu-id="b9eff-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="b9eff-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9eff-139">lastModifiedDateTime</span></span>|<span data-ttu-id="b9eff-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9eff-140">DateTimeOffset</span></span>|<span data-ttu-id="b9eff-141">上次修改 ManagedEBookCategory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b9eff-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="b9eff-142">响应</span><span class="sxs-lookup"><span data-stu-id="b9eff-142">Response</span></span>
<span data-ttu-id="b9eff-143">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [managedEBookCategory](../resources/intune-books-managedebookcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="b9eff-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b9eff-144">示例</span><span class="sxs-lookup"><span data-stu-id="b9eff-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="b9eff-145">请求</span><span class="sxs-lookup"><span data-stu-id="b9eff-145">Request</span></span>
<span data-ttu-id="b9eff-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b9eff-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="b9eff-147">响应</span><span class="sxs-lookup"><span data-stu-id="b9eff-147">Response</span></span>
<span data-ttu-id="b9eff-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b9eff-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




