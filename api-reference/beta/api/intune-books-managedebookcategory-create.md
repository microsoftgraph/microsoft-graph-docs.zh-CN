---
title: 创建 managedEBookCategory
description: 创建新的 managedEBookCategory 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: ae2fd38c576d2d85f4d07137a17e3a20be78ccff
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51133029"
---
# <a name="create-managedebookcategory"></a><span data-ttu-id="760cc-103">创建 managedEBookCategory</span><span class="sxs-lookup"><span data-stu-id="760cc-103">Create managedEBookCategory</span></span>

<span data-ttu-id="760cc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="760cc-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="760cc-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="760cc-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="760cc-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="760cc-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="760cc-107">创建新的 [managedEBookCategory](../resources/intune-books-managedebookcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="760cc-107">Create a new [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="760cc-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="760cc-108">Prerequisites</span></span>
<span data-ttu-id="760cc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="760cc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="760cc-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="760cc-111">Permission type</span></span>|<span data-ttu-id="760cc-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="760cc-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="760cc-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="760cc-113">Delegated (work or school account)</span></span>|<span data-ttu-id="760cc-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="760cc-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="760cc-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="760cc-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="760cc-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="760cc-116">Not supported.</span></span>|
|<span data-ttu-id="760cc-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="760cc-117">Application</span></span>|<span data-ttu-id="760cc-118">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="760cc-118">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="760cc-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="760cc-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBookCategories
POST /deviceAppManagement/managedEBooks/{managedEBookId}/categories
```

## <a name="request-headers"></a><span data-ttu-id="760cc-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="760cc-120">Request headers</span></span>
|<span data-ttu-id="760cc-121">标头</span><span class="sxs-lookup"><span data-stu-id="760cc-121">Header</span></span>|<span data-ttu-id="760cc-122">值</span><span class="sxs-lookup"><span data-stu-id="760cc-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="760cc-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="760cc-123">Authorization</span></span>|<span data-ttu-id="760cc-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="760cc-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="760cc-125">接受</span><span class="sxs-lookup"><span data-stu-id="760cc-125">Accept</span></span>|<span data-ttu-id="760cc-126">application/json</span><span class="sxs-lookup"><span data-stu-id="760cc-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="760cc-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="760cc-127">Request body</span></span>
<span data-ttu-id="760cc-128">在请求正文中，提供 managedEBookCategory 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="760cc-128">In the request body, supply a JSON representation for the managedEBookCategory object.</span></span>

<span data-ttu-id="760cc-129">下表显示创建 managedEBookCategory 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="760cc-129">The following table shows the properties that are required when you create the managedEBookCategory.</span></span>

|<span data-ttu-id="760cc-130">属性</span><span class="sxs-lookup"><span data-stu-id="760cc-130">Property</span></span>|<span data-ttu-id="760cc-131">类型</span><span class="sxs-lookup"><span data-stu-id="760cc-131">Type</span></span>|<span data-ttu-id="760cc-132">说明</span><span class="sxs-lookup"><span data-stu-id="760cc-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="760cc-133">id</span><span class="sxs-lookup"><span data-stu-id="760cc-133">id</span></span>|<span data-ttu-id="760cc-134">String</span><span class="sxs-lookup"><span data-stu-id="760cc-134">String</span></span>|<span data-ttu-id="760cc-135">实体的键。</span><span class="sxs-lookup"><span data-stu-id="760cc-135">The key of the entity.</span></span>|
|<span data-ttu-id="760cc-136">displayName</span><span class="sxs-lookup"><span data-stu-id="760cc-136">displayName</span></span>|<span data-ttu-id="760cc-137">String</span><span class="sxs-lookup"><span data-stu-id="760cc-137">String</span></span>|<span data-ttu-id="760cc-138">电子图书类别的名称。</span><span class="sxs-lookup"><span data-stu-id="760cc-138">The name of the eBook category.</span></span>|
|<span data-ttu-id="760cc-139">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="760cc-139">lastModifiedDateTime</span></span>|<span data-ttu-id="760cc-140">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="760cc-140">DateTimeOffset</span></span>|<span data-ttu-id="760cc-141">ManagedEBookCategory 上次修改的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="760cc-141">The date and time the ManagedEBookCategory was last modified.</span></span>|



## <a name="response"></a><span data-ttu-id="760cc-142">响应</span><span class="sxs-lookup"><span data-stu-id="760cc-142">Response</span></span>
<span data-ttu-id="760cc-143">如果成功，此方法在响应 `201 Created` 正文中返回 [响应代码和 managedEBookCategory](../resources/intune-books-managedebookcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="760cc-143">If successful, this method returns a `201 Created` response code and a [managedEBookCategory](../resources/intune-books-managedebookcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="760cc-144">示例</span><span class="sxs-lookup"><span data-stu-id="760cc-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="760cc-145">请求</span><span class="sxs-lookup"><span data-stu-id="760cc-145">Request</span></span>
<span data-ttu-id="760cc-146">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="760cc-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBookCategories
Content-type: application/json
Content-length: 102

{
  "@odata.type": "#microsoft.graph.managedEBookCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="760cc-147">响应</span><span class="sxs-lookup"><span data-stu-id="760cc-147">Response</span></span>
<span data-ttu-id="760cc-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="760cc-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




