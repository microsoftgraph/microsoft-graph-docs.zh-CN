---
title: 创建 termsAndConditionsGroupAssignment
description: 创建新的 termsAndConditionsGroupAssignment 对象。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 92f24d359791507485f73ef4f7198cdc5f98572a
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51132910"
---
# <a name="create-termsandconditionsgroupassignment"></a><span data-ttu-id="08945-103">创建 termsAndConditionsGroupAssignment</span><span class="sxs-lookup"><span data-stu-id="08945-103">Create termsAndConditionsGroupAssignment</span></span>

<span data-ttu-id="08945-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="08945-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="08945-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="08945-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="08945-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="08945-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="08945-107">创建新的 [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08945-107">Create a new [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="08945-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="08945-108">Prerequisites</span></span>
<span data-ttu-id="08945-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="08945-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="08945-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="08945-111">Permission type</span></span>|<span data-ttu-id="08945-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="08945-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="08945-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="08945-113">Delegated (work or school account)</span></span>|<span data-ttu-id="08945-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08945-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="08945-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="08945-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="08945-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="08945-116">Not supported.</span></span>|
|<span data-ttu-id="08945-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="08945-117">Application</span></span>|<span data-ttu-id="08945-118">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="08945-118">DeviceManagementServiceConfig.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="08945-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="08945-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
```

## <a name="request-headers"></a><span data-ttu-id="08945-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="08945-120">Request headers</span></span>
|<span data-ttu-id="08945-121">标头</span><span class="sxs-lookup"><span data-stu-id="08945-121">Header</span></span>|<span data-ttu-id="08945-122">值</span><span class="sxs-lookup"><span data-stu-id="08945-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="08945-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="08945-123">Authorization</span></span>|<span data-ttu-id="08945-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="08945-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="08945-125">接受</span><span class="sxs-lookup"><span data-stu-id="08945-125">Accept</span></span>|<span data-ttu-id="08945-126">application/json</span><span class="sxs-lookup"><span data-stu-id="08945-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="08945-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="08945-127">Request body</span></span>
<span data-ttu-id="08945-128">在请求正文中，提供 termsAndConditionsGroupAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="08945-128">In the request body, supply a JSON representation for the termsAndConditionsGroupAssignment object.</span></span>

<span data-ttu-id="08945-129">下表显示创建 termsAndConditionsGroupAssignment 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="08945-129">The following table shows the properties that are required when you create the termsAndConditionsGroupAssignment.</span></span>

|<span data-ttu-id="08945-130">属性</span><span class="sxs-lookup"><span data-stu-id="08945-130">Property</span></span>|<span data-ttu-id="08945-131">类型</span><span class="sxs-lookup"><span data-stu-id="08945-131">Type</span></span>|<span data-ttu-id="08945-132">说明</span><span class="sxs-lookup"><span data-stu-id="08945-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="08945-133">id</span><span class="sxs-lookup"><span data-stu-id="08945-133">id</span></span>|<span data-ttu-id="08945-134">String</span><span class="sxs-lookup"><span data-stu-id="08945-134">String</span></span>|<span data-ttu-id="08945-135">实体的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="08945-135">Unique identifier of the entity.</span></span>|
|<span data-ttu-id="08945-136">targetGroupId</span><span class="sxs-lookup"><span data-stu-id="08945-136">targetGroupId</span></span>|<span data-ttu-id="08945-137">String</span><span class="sxs-lookup"><span data-stu-id="08945-137">String</span></span>|<span data-ttu-id="08945-138">T 和 C 策略&组的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="08945-138">Unique identifier of a group that the T&C policy is assigned to.</span></span>|



## <a name="response"></a><span data-ttu-id="08945-139">响应</span><span class="sxs-lookup"><span data-stu-id="08945-139">Response</span></span>
<span data-ttu-id="08945-140">如果成功，此方法在响应正文中返回 响应代码和 `201 Created` [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="08945-140">If successful, this method returns a `201 Created` response code and a [termsAndConditionsGroupAssignment](../resources/intune-companyterms-termsandconditionsgroupassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="08945-141">示例</span><span class="sxs-lookup"><span data-stu-id="08945-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="08945-142">请求</span><span class="sxs-lookup"><span data-stu-id="08945-142">Request</span></span>
<span data-ttu-id="08945-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="08945-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/termsAndConditions/{termsAndConditionsId}/groupAssignments
Content-type: application/json
Content-length: 120

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "targetGroupId": "Target Group Id value"
}
```

### <a name="response"></a><span data-ttu-id="08945-144">响应</span><span class="sxs-lookup"><span data-stu-id="08945-144">Response</span></span>
<span data-ttu-id="08945-p102">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="08945-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 169

{
  "@odata.type": "#microsoft.graph.termsAndConditionsGroupAssignment",
  "id": "2eb1aab7-aab7-2eb1-b7aa-b12eb7aab12e",
  "targetGroupId": "Target Group Id value"
}
```




