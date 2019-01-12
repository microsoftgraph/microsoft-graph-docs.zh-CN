---
title: 更新 embeddedSIMActivationCodePoolAssignment
description: 更新 embeddedSIMActivationCodePoolAssignment 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5dca1f71f31cd793a0611165026330863dad29be
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27975362"
---
# <a name="update-embeddedsimactivationcodepoolassignment"></a><span data-ttu-id="148db-103">更新 embeddedSIMActivationCodePoolAssignment</span><span class="sxs-lookup"><span data-stu-id="148db-103">Update embeddedSIMActivationCodePoolAssignment</span></span>

> <span data-ttu-id="148db-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="148db-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="148db-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="148db-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="148db-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="148db-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="148db-107">更新[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="148db-107">Update the properties of a [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="148db-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="148db-108">Prerequisites</span></span>
<span data-ttu-id="148db-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="148db-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="148db-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="148db-111">Permission type</span></span>|<span data-ttu-id="148db-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="148db-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="148db-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="148db-113">Delegated (work or school account)</span></span>|<span data-ttu-id="148db-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="148db-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="148db-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="148db-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="148db-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="148db-116">Not supported.</span></span>|
|<span data-ttu-id="148db-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="148db-117">Application</span></span>|<span data-ttu-id="148db-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="148db-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="148db-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="148db-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="148db-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="148db-120">Request headers</span></span>
|<span data-ttu-id="148db-121">标头</span><span class="sxs-lookup"><span data-stu-id="148db-121">Header</span></span>|<span data-ttu-id="148db-122">值</span><span class="sxs-lookup"><span data-stu-id="148db-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="148db-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="148db-123">Authorization</span></span>|<span data-ttu-id="148db-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="148db-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="148db-125">Accept</span><span class="sxs-lookup"><span data-stu-id="148db-125">Accept</span></span>|<span data-ttu-id="148db-126">application/json</span><span class="sxs-lookup"><span data-stu-id="148db-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="148db-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="148db-127">Request body</span></span>
<span data-ttu-id="148db-128">在请求正文中，提供[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="148db-128">In the request body, supply a JSON representation for the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object.</span></span>

<span data-ttu-id="148db-129">下表显示时创建[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="148db-129">The following table shows the properties that are required when you create the [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md).</span></span>

|<span data-ttu-id="148db-130">属性</span><span class="sxs-lookup"><span data-stu-id="148db-130">Property</span></span>|<span data-ttu-id="148db-131">类型</span><span class="sxs-lookup"><span data-stu-id="148db-131">Type</span></span>|<span data-ttu-id="148db-132">说明</span><span class="sxs-lookup"><span data-stu-id="148db-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="148db-133">id</span><span class="sxs-lookup"><span data-stu-id="148db-133">id</span></span>|<span data-ttu-id="148db-134">字符串</span><span class="sxs-lookup"><span data-stu-id="148db-134">String</span></span>|<span data-ttu-id="148db-135">嵌入 SIM 激活代码池分配的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="148db-135">Unique identifier for the embedded SIM activation code pool assignment.</span></span> <span data-ttu-id="148db-136">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="148db-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="148db-137">target</span><span class="sxs-lookup"><span data-stu-id="148db-137">target</span></span>|[<span data-ttu-id="148db-138">deviceAndAppManagementAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="148db-138">deviceAndAppManagementAssignmentTarget</span></span>](../resources/intune-shared-deviceandappmanagementassignmenttarget.md)|<span data-ttu-id="148db-139">目标嵌入 SIM 激活代码池的组的类型。</span><span class="sxs-lookup"><span data-stu-id="148db-139">The type of groups targeted by the embedded SIM activation code pool.</span></span>|



## <a name="response"></a><span data-ttu-id="148db-140">响应</span><span class="sxs-lookup"><span data-stu-id="148db-140">Response</span></span>
<span data-ttu-id="148db-141">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="148db-141">If successful, this method returns a `200 OK` response code and an updated [embeddedSIMActivationCodePoolAssignment](../resources/intune-esim-embeddedsimactivationcodepoolassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="148db-142">示例</span><span class="sxs-lookup"><span data-stu-id="148db-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="148db-143">请求</span><span class="sxs-lookup"><span data-stu-id="148db-143">Request</span></span>
<span data-ttu-id="148db-144">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="148db-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/embeddedSIMActivationCodePools/{embeddedSIMActivationCodePoolId}/assignments/{embeddedSIMActivationCodePoolAssignmentId}
Content-type: application/json
Content-length: 101

{
  "target": {
    "@odata.type": "microsoft.graph.deviceAndAppManagementAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="148db-145">响应</span><span class="sxs-lookup"><span data-stu-id="148db-145">Response</span></span>
<span data-ttu-id="148db-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="148db-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





