---
title: 创建 embeddedSIMActivationCodePoolAssignment
description: 创建新的 embeddedSIMActivationCodePoolAssignment 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 61a541d9b95f7a8e9f3057856c11fb873dd00fc3
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27953467"
---
# <a name="create-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="e8dad-103">创建 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="e8dad-103">Create embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="e8dad-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="e8dad-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e8dad-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="e8dad-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e8dad-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="e8dad-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e8dad-107">创建新的[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e8dad-107">Create a new [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="e8dad-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="e8dad-108">Prerequisites</span></span>
<span data-ttu-id="e8dad-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="e8dad-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e8dad-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e8dad-111">Permission type</span></span>|<span data-ttu-id="e8dad-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="e8dad-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e8dad-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e8dad-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e8dad-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e8dad-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="e8dad-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e8dad-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e8dad-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8dad-116">Not supported.</span></span>|
|<span data-ttu-id="e8dad-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e8dad-117">Application</span></span>|<span data-ttu-id="e8dad-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e8dad-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e8dad-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e8dad-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="e8dad-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e8dad-120">Request headers</span></span>
|<span data-ttu-id="e8dad-121">标头</span><span class="sxs-lookup"><span data-stu-id="e8dad-121">Header</span></span>|<span data-ttu-id="e8dad-122">值</span><span class="sxs-lookup"><span data-stu-id="e8dad-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e8dad-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e8dad-123">Authorization</span></span>|<span data-ttu-id="e8dad-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="e8dad-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e8dad-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e8dad-125">Accept</span></span>|<span data-ttu-id="e8dad-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e8dad-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e8dad-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="e8dad-127">Request body</span></span>
<span data-ttu-id="e8dad-128">在请求正文中，提供 embeddedSIMActivationCodePoolAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e8dad-128">In the request body, supply a JSON representation for the embeddedSIMActivationCodePoolAssignment object.</span></span>

<span data-ttu-id="e8dad-129">下表显示时创建 embeddedSIMActivationCodePoolAssignment 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="e8dad-129">The following table shows the properties that are required when you create the embeddedSIMActivationCodePoolAssignment.</span></span>

|<span data-ttu-id="e8dad-130">属性</span><span class="sxs-lookup"><span data-stu-id="e8dad-130">Property</span></span>|<span data-ttu-id="e8dad-131">类型</span><span class="sxs-lookup"><span data-stu-id="e8dad-131">Type</span></span>|<span data-ttu-id="e8dad-132">说明</span><span class="sxs-lookup"><span data-stu-id="e8dad-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e8dad-133">id</span><span class="sxs-lookup"><span data-stu-id="e8dad-133">id</span></span>|<span data-ttu-id="e8dad-134">字符串</span><span class="sxs-lookup"><span data-stu-id="e8dad-134">String</span></span>|<span data-ttu-id="e8dad-135">嵌入 SIM 激活代码池分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="e8dad-135">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="e8dad-136">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="e8dad-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="e8dad-137">target</span><span class="sxs-lookup"><span data-stu-id="e8dad-137">target</span></span>|[<span data-ttu-id="e8dad-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e8dad-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="e8dad-139">目标嵌入 SIM 激活代码池的组的类型。</span><span class="sxs-lookup"><span data-stu-id="e8dad-139">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="e8dad-140">响应</span><span class="sxs-lookup"><span data-stu-id="e8dad-140">Response</span></span>
<span data-ttu-id="e8dad-141">如果成功，此方法返回`201 Created`响应代码和响应正文中的[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e8dad-141">If successful, this method returns a `201 Created` response code and a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e8dad-142">示例</span><span class="sxs-lookup"><span data-stu-id="e8dad-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="e8dad-143">请求</span><span class="sxs-lookup"><span data-stu-id="e8dad-143">Request</span></span>
<span data-ttu-id="e8dad-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="e8dad-144">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="e8dad-145">响应</span><span class="sxs-lookup"><span data-stu-id="e8dad-145">Response</span></span>
<span data-ttu-id="e8dad-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="e8dad-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





