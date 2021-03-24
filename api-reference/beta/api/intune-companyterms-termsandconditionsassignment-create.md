---
title: 创建 termsAndConditionsAssignment
description: 创建新的 termsAndConditionsAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: a75ba59e8e528b758c81b9472311569a6bb3e74d
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51131874"
---
# <a name="create-termsandconditionsassignment"></a><span data-ttu-id="655c1-103">创建 termsAndConditionsAssignment</span><span class="sxs-lookup"><span data-stu-id="655c1-103">Create termsAndConditionsAssignment</span></span>

<span data-ttu-id="655c1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="655c1-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="655c1-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="655c1-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="655c1-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="655c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="655c1-107">创建新的 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="655c1-107">Create a new [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="655c1-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="655c1-108">Prerequisites</span></span>
<span data-ttu-id="655c1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="655c1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="655c1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="655c1-111">Permission type</span></span>|<span data-ttu-id="655c1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="655c1-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="655c1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="655c1-113">Delegated (work or school account)</span></span>|<span data-ttu-id="655c1-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="655c1-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="655c1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="655c1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="655c1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="655c1-116">Not supported.</span></span>|
|<span data-ttu-id="655c1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="655c1-117">Application</span></span>|<span data-ttu-id="655c1-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="655c1-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="655c1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="655c1-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="655c1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="655c1-120">Request headers</span></span>
|<span data-ttu-id="655c1-121">标头</span><span class="sxs-lookup"><span data-stu-id="655c1-121">Header</span></span>|<span data-ttu-id="655c1-122">值</span><span class="sxs-lookup"><span data-stu-id="655c1-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="655c1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="655c1-123">Authorization</span></span>|<span data-ttu-id="655c1-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="655c1-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="655c1-125">接受</span><span class="sxs-lookup"><span data-stu-id="655c1-125">Accept</span></span>|<span data-ttu-id="655c1-126">application/json</span><span class="sxs-lookup"><span data-stu-id="655c1-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="655c1-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="655c1-127">Request body</span></span>
<span data-ttu-id="655c1-128">在请求正文中，提供 termsAndConditionsAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="655c1-128">In the request body, supply a JSON representation for the termsAndConditionsAssignment object.</span></span>

<span data-ttu-id="655c1-129">下表显示创建 termsAndConditionsAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="655c1-129">The following table shows the properties that are required when you create the termsAndConditionsAssignment.</span></span>

|<span data-ttu-id="655c1-130">属性</span><span class="sxs-lookup"><span data-stu-id="655c1-130">Property</span></span>|<span data-ttu-id="655c1-131">类型</span><span class="sxs-lookup"><span data-stu-id="655c1-131">Type</span></span>|<span data-ttu-id="655c1-132">说明</span><span class="sxs-lookup"><span data-stu-id="655c1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="655c1-133">id</span><span class="sxs-lookup"><span data-stu-id="655c1-133">id</span></span>|<span data-ttu-id="655c1-134">String</span><span class="sxs-lookup"><span data-stu-id="655c1-134">String</span></span>|<span data-ttu-id="655c1-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="655c1-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="655c1-136">target</span><span class="sxs-lookup"><span data-stu-id="655c1-136">target</span></span>|[<span data-ttu-id="655c1-137">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="655c1-137">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="655c1-138">将 T&C 策略分配到的分配目标。</span><span class="sxs-lookup"><span data-stu-id="655c1-138">Assignment target that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="655c1-139">响应</span><span class="sxs-lookup"><span data-stu-id="655c1-139">Response</span></span>
<span data-ttu-id="655c1-140">如果成功，此方法将在响应正文中返回 `201 Created` 响应代码和 [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="655c1-140">If successful, this method returns a `201 Created` response code and a [termsAndConditionsAssignment](../resources/intune-companyterms-termsandconditionsassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="655c1-141">示例</span><span class="sxs-lookup"><span data-stu-id="655c1-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="655c1-142">请求</span><span class="sxs-lookup"><span data-stu-id="655c1-142">Request</span></span>
<span data-ttu-id="655c1-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="655c1-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/assignments
Content-type: application/json
Content-length: 387

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```

### <a name="response"></a><span data-ttu-id="655c1-144">响应</span><span class="sxs-lookup"><span data-stu-id="655c1-144">Response</span></span>
<span data-ttu-id="655c1-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="655c1-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 436

{
  "@odata.type": "#microsoft.graph.termsAndConditionsAssignment",
  "id": "64c1a196-a196-64c1-96a1-c16496a1c164",
  "target": {
    "@odata.type": "microsoft.graph.configurationManagerCollectionAssignmentTarget",
    "deviceAndAppManagementAssignmentFilterId": "Device And App Management Assignment Filter Id value",
    "deviceAndAppManagementAssignmentFilterType": "include",
    "collectionId": "Collection Id value"
  }
}
```




