---
title: 更新 managedEBookCategory
description: 更新 managedEBookCategory 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 85cda4854d3bbe6f6b1932b1f6fc546044490a56
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/29/2019
ms.locfileid: "30973122"
---
# <a name="update-managedebookcategory"></a><span data-ttu-id="60ca8-103">更新 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="60ca8-103">Update managedEBookCategory</span></span>

> <span data-ttu-id="60ca8-104">**重要说明:**/beta 版本下的 Microsoft Graph api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="60ca8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="60ca8-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="60ca8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="60ca8-106">更新[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="60ca8-106">Update the properties of a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="60ca8-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="60ca8-107">Prerequisites</span></span>
<span data-ttu-id="60ca8-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="60ca8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="60ca8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="60ca8-110">Permission type</span></span>|<span data-ttu-id="60ca8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="60ca8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="60ca8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="60ca8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="60ca8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="60ca8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="60ca8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="60ca8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="60ca8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="60ca8-115">Not supported.</span></span>|
|<span data-ttu-id="60ca8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="60ca8-116">Application</span></span>|<span data-ttu-id="60ca8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="60ca8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="60ca8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="60ca8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/categories/{managedEBookCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="60ca8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="60ca8-119">Request headers</span></span>
|<span data-ttu-id="60ca8-120">标头</span><span class="sxs-lookup"><span data-stu-id="60ca8-120">Header</span></span>|<span data-ttu-id="60ca8-121">值</span><span class="sxs-lookup"><span data-stu-id="60ca8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="60ca8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="60ca8-122">Authorization</span></span>|<span data-ttu-id="60ca8-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="60ca8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="60ca8-124">接受</span><span class="sxs-lookup"><span data-stu-id="60ca8-124">Accept</span></span>|<span data-ttu-id="60ca8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="60ca8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="60ca8-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="60ca8-126">Request body</span></span>
<span data-ttu-id="60ca8-127">在请求正文中, 提供[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="60ca8-127">In the request body, supply a JSON representation for the [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

<span data-ttu-id="60ca8-128">下表显示创建[managedEBookCategory](../resources/intune-books-managedebookcategory.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="60ca8-128">The following table shows the properties that are required when you create the [managedEBookCategory](../resources/intune-books-managedebookcategory.md).</span></span>

|<span data-ttu-id="60ca8-129">属性</span><span class="sxs-lookup"><span data-stu-id="60ca8-129">Property</span></span>|<span data-ttu-id="60ca8-130">类型</span><span class="sxs-lookup"><span data-stu-id="60ca8-130">Type</span></span>|<span data-ttu-id="60ca8-131">说明</span><span class="sxs-lookup"><span data-stu-id="60ca8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="60ca8-132">id</span><span class="sxs-lookup"><span data-stu-id="60ca8-132">id</span></span>|<span data-ttu-id="60ca8-133">String</span><span class="sxs-lookup"><span data-stu-id="60ca8-133">String</span></span>|<span data-ttu-id="60ca8-134">实体的键。</span><span class="sxs-lookup"><span data-stu-id="60ca8-134">The key of the entity.</span></span>|
|<span data-ttu-id="60ca8-135">displayName</span><span class="sxs-lookup"><span data-stu-id="60ca8-135">displayName</span></span>|<span data-ttu-id="60ca8-136">String</span><span class="sxs-lookup"><span data-stu-id="60ca8-136">String</span></span>|<span data-ttu-id="60ca8-137">电子书类别的名称。</span><span class="sxs-lookup"><span data-stu-id="60ca8-137">The name of the eBook category.</span></span>|
|<span data-ttu-id="60ca8-138">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="60ca8-138">lastModifiedDateTime</span></span>|<span data-ttu-id="60ca8-139">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="60ca8-139">DateTimeOffset</span></span>|<span data-ttu-id="60ca8-140">上次修改 ManagedEBookCategory 的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="60ca8-140">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="60ca8-141">响应</span><span class="sxs-lookup"><span data-stu-id="60ca8-141">Response</span></span>
<span data-ttu-id="60ca8-142">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[managedEBookCategory](../resources/intune-books-managedebookcategory.md)对象。</span><span class="sxs-lookup"><span data-stu-id="60ca8-142">If successful, this method returns a `200 OK` response code and an updated [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="60ca8-143">示例</span><span class="sxs-lookup"><span data-stu-id="60ca8-143">Example</span></span>

### <a name="request"></a><span data-ttu-id="60ca8-144">请求</span><span class="sxs-lookup"><span data-stu-id="60ca8-144">Request</span></span>
<span data-ttu-id="60ca8-145">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="60ca8-145">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories/{managedEBookCategoryId}
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="60ca8-146">响应</span><span class="sxs-lookup"><span data-stu-id="60ca8-146">Response</span></span>
<span data-ttu-id="60ca8-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="60ca8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




