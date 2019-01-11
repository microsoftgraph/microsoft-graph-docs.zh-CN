---
title: 创建 embeddedSIMActivationCodePoolAssignment
description: 创建新的 embeddedSIMActivationCodePoolAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: e020dafec47fe1a669251825ba0dff75f41f382c
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27865931"
---
# <a name="create-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="da2f4-103">创建 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="da2f4-103">Create embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="da2f4-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="da2f4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="da2f4-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="da2f4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="da2f4-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="da2f4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="da2f4-107">创建新的[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="da2f4-107">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="da2f4-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="da2f4-108">Prerequisites</span></span>
<span data-ttu-id="da2f4-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="da2f4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="da2f4-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="da2f4-111">Permission type</span></span>|<span data-ttu-id="da2f4-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="da2f4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="da2f4-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="da2f4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="da2f4-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="da2f4-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="da2f4-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="da2f4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="da2f4-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="da2f4-116">Not supported.</span></span>|
|<span data-ttu-id="da2f4-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="da2f4-117">Application</span></span>|<span data-ttu-id="da2f4-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="da2f4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="da2f4-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="da2f4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="da2f4-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="da2f4-120">Request headers</span></span>
|<span data-ttu-id="da2f4-121">标头</span><span class="sxs-lookup"><span data-stu-id="da2f4-121">Header</span></span>|<span data-ttu-id="da2f4-122">值</span><span class="sxs-lookup"><span data-stu-id="da2f4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="da2f4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="da2f4-123">Authorization</span></span>|<span data-ttu-id="da2f4-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="da2f4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="da2f4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="da2f4-125">Accept</span></span>|<span data-ttu-id="da2f4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="da2f4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="da2f4-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="da2f4-127">Request body</span></span>
<span data-ttu-id="da2f4-128">在请求正文中，提供 embeddedSIMActivationCodePoolAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="da2f4-128">In the request body, supply a JSON representation for the embeddedSIMActivationCodePoolAssignment object.</span></span>

<span data-ttu-id="da2f4-129">下表显示时创建 embeddedSIMActivationCodePoolAssignment 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="da2f4-129">The following table shows the properties that are required when you create the embeddedSIMActivationCodePoolAssignment.</span></span>

|<span data-ttu-id="da2f4-130">属性</span><span class="sxs-lookup"><span data-stu-id="da2f4-130">Property</span></span>|<span data-ttu-id="da2f4-131">类型</span><span class="sxs-lookup"><span data-stu-id="da2f4-131">Type</span></span>|<span data-ttu-id="da2f4-132">说明</span><span class="sxs-lookup"><span data-stu-id="da2f4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="da2f4-133">id</span><span class="sxs-lookup"><span data-stu-id="da2f4-133">id</span></span>|<span data-ttu-id="da2f4-134">字符串</span><span class="sxs-lookup"><span data-stu-id="da2f4-134">String</span></span>|<span data-ttu-id="da2f4-135">嵌入 SIM 激活代码池分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="da2f4-135">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="da2f4-136">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="da2f4-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="da2f4-137">target</span><span class="sxs-lookup"><span data-stu-id="da2f4-137">target</span></span>|[<span data-ttu-id="da2f4-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="da2f4-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="da2f4-139">目标嵌入 SIM 激活代码池的组的类型。</span><span class="sxs-lookup"><span data-stu-id="da2f4-139">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="da2f4-140">响应</span><span class="sxs-lookup"><span data-stu-id="da2f4-140">Response</span></span>
<span data-ttu-id="da2f4-141">如果成功，此方法返回`201 Created`响应代码和响应正文中的[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="da2f4-141">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="da2f4-142">示例</span><span class="sxs-lookup"><span data-stu-id="da2f4-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="da2f4-143">请求</span><span class="sxs-lookup"><span data-stu-id="da2f4-143">Request</span></span>
<span data-ttu-id="da2f4-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="da2f4-144">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
Content-type: application/json
Content-length: 179

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="da2f4-145">响应</span><span class="sxs-lookup"><span data-stu-id="da2f4-145">Response</span></span>
<span data-ttu-id="da2f4-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="da2f4-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 228

{
  "@odata.type": "#microsoft.graph.embeddedSIMActivationCodePoolAssignment",
  "id": "e7304dcc-4dcc-e730-cc4d-30e7cc4d30e7",
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```





