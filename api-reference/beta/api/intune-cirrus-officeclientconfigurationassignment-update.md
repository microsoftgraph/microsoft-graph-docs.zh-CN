---
title: 更新 officeClientConfigurationAssignment
description: 更新 officeClientConfigurationAssignment 对象的属性。
author: tfitzmac
ms.openlocfilehash: 78b0ae28bc61bc0d8d8c083502c6f6ef2cf7d0fb
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27343033"
---
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="ad44e-103">更新 officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="ad44e-103">Update officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="ad44e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ad44e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ad44e-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ad44e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ad44e-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ad44e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ad44e-107">更新[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ad44e-107">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ad44e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ad44e-108">Prerequisites</span></span>
<span data-ttu-id="ad44e-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ad44e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad44e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad44e-111">Permission type</span></span>|<span data-ttu-id="ad44e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ad44e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ad44e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad44e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ad44e-114">\* \* TODO： 确定范围 \* \*</span><span class="sxs-lookup"><span data-stu-id="ad44e-114">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="ad44e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad44e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ad44e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad44e-116">Not supported.</span></span>|
|<span data-ttu-id="ad44e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ad44e-117">Application</span></span>|<span data-ttu-id="ad44e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad44e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ad44e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad44e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="ad44e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ad44e-120">Request headers</span></span>
|<span data-ttu-id="ad44e-121">标头</span><span class="sxs-lookup"><span data-stu-id="ad44e-121">Header</span></span>|<span data-ttu-id="ad44e-122">值</span><span class="sxs-lookup"><span data-stu-id="ad44e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ad44e-123">授权</span><span class="sxs-lookup"><span data-stu-id="ad44e-123">Authorization</span></span>|<span data-ttu-id="ad44e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ad44e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ad44e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ad44e-125">Accept</span></span>|<span data-ttu-id="ad44e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ad44e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad44e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad44e-127">Request body</span></span>
<span data-ttu-id="ad44e-128">在请求正文中，提供[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ad44e-128">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="ad44e-129">下表显示时创建[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ad44e-129">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="ad44e-130">属性</span><span class="sxs-lookup"><span data-stu-id="ad44e-130">Property</span></span>|<span data-ttu-id="ad44e-131">类型</span><span class="sxs-lookup"><span data-stu-id="ad44e-131">Type</span></span>|<span data-ttu-id="ad44e-132">说明</span><span class="sxs-lookup"><span data-stu-id="ad44e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ad44e-133">id</span><span class="sxs-lookup"><span data-stu-id="ad44e-133">id</span></span>|<span data-ttu-id="ad44e-134">字符串</span><span class="sxs-lookup"><span data-stu-id="ad44e-134">String</span></span>|<span data-ttu-id="ad44e-135">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ad44e-135">Not yet documented</span></span>|
|<span data-ttu-id="ad44e-136">target</span><span class="sxs-lookup"><span data-stu-id="ad44e-136">target</span></span>|[<span data-ttu-id="ad44e-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ad44e-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="ad44e-138">尚未记录</span><span class="sxs-lookup"><span data-stu-id="ad44e-138">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="ad44e-139">响应</span><span class="sxs-lookup"><span data-stu-id="ad44e-139">Response</span></span>
<span data-ttu-id="ad44e-140">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ad44e-140">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ad44e-141">示例</span><span class="sxs-lookup"><span data-stu-id="ad44e-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="ad44e-142">请求</span><span class="sxs-lookup"><span data-stu-id="ad44e-142">Request</span></span>
<span data-ttu-id="ad44e-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ad44e-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
Content-type: application/json
Content-length: 98

{
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ad44e-144">响应</span><span class="sxs-lookup"><span data-stu-id="ad44e-144">Response</span></span>
<span data-ttu-id="ad44e-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ad44e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "804730f3-30f3-8047-f330-4780f3304780",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```



