---
title: 更新 managedEBookCategory
description: 更新 managedEBookCategory 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: ef8970fb32b94b17b9277c3d30fc72bbc582ea87
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27853191"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="a2ed6-103">更新 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="a2ed6-103">Update managedEBookCategory</span></span>

> <span data-ttu-id="a2ed6-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="a2ed6-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a2ed6-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="a2ed6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a2ed6-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="a2ed6-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="a2ed6-107">更新[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="a2ed6-107">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="a2ed6-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="a2ed6-108">Prerequisites</span></span>
<span data-ttu-id="a2ed6-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="a2ed6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a2ed6-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="a2ed6-111">Permission type</span></span>|<span data-ttu-id="a2ed6-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="a2ed6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a2ed6-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a2ed6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a2ed6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a2ed6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a2ed6-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a2ed6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a2ed6-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2ed6-116">Not supported.</span></span>|
|<span data-ttu-id="a2ed6-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="a2ed6-117">Application</span></span>|<span data-ttu-id="a2ed6-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="a2ed6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a2ed6-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a2ed6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="a2ed6-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="a2ed6-120">Request headers</span></span>
|<span data-ttu-id="a2ed6-121">标头</span><span class="sxs-lookup"><span data-stu-id="a2ed6-121">Header</span></span>|<span data-ttu-id="a2ed6-122">值</span><span class="sxs-lookup"><span data-stu-id="a2ed6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a2ed6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a2ed6-123">Authorization</span></span>|<span data-ttu-id="a2ed6-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="a2ed6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a2ed6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a2ed6-125">Accept</span></span>|<span data-ttu-id="a2ed6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a2ed6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a2ed6-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="a2ed6-127">Request body</span></span>
<span data-ttu-id="a2ed6-128">在请求正文中，提供[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="a2ed6-128">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="a2ed6-129">下表显示时创建[managedEBookCategory](../resources/intune-books-managedebookcategory.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="a2ed6-129">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="a2ed6-130">属性</span><span class="sxs-lookup"><span data-stu-id="a2ed6-130">Property</span></span>|<span data-ttu-id="a2ed6-131">类型</span><span class="sxs-lookup"><span data-stu-id="a2ed6-131">Type</span></span>|<span data-ttu-id="a2ed6-132">说明</span><span class="sxs-lookup"><span data-stu-id="a2ed6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a2ed6-133">id</span><span class="sxs-lookup"><span data-stu-id="a2ed6-133">id</span></span>|<span data-ttu-id="a2ed6-134">String</span><span class="sxs-lookup"><span data-stu-id="a2ed6-134">String</span></span>|<span data-ttu-id="a2ed6-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="a2ed6-135">The key of the entity.</span></span>|
|<span data-ttu-id="a2ed6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="a2ed6-136">displayName</span></span>|<span data-ttu-id="a2ed6-137">字符串</span><span class="sxs-lookup"><span data-stu-id="a2ed6-137">String</span></span>|<span data-ttu-id="a2ed6-138">电子图书类别的名称。</span><span class="sxs-lookup"><span data-stu-id="a2ed6-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="a2ed6-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="a2ed6-139">lastModifiedDateTime</span></span>|<span data-ttu-id="a2ed6-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="a2ed6-140">DateTimeOffset</span></span>|<span data-ttu-id="a2ed6-141">日期和 ManagedEBookCategory 上次修改的时间。</span><span class="sxs-lookup"><span data-stu-id="a2ed6-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="a2ed6-142">响应</span><span class="sxs-lookup"><span data-stu-id="a2ed6-142">Response</span></span>
<span data-ttu-id="a2ed6-143">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a2ed6-143">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a2ed6-144">示例</span><span class="sxs-lookup"><span data-stu-id="a2ed6-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="a2ed6-145">请求</span><span class="sxs-lookup"><span data-stu-id="a2ed6-145">Request</span></span>
<span data-ttu-id="a2ed6-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="a2ed6-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 107

{
  "displayName": "Display Name value",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00"
}
```

### <a name="response"></a><span data-ttu-id="a2ed6-147">响应</span><span class="sxs-lookup"><span data-stu-id="a2ed6-147">Response</span></span>
<span data-ttu-id="a2ed6-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a2ed6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





