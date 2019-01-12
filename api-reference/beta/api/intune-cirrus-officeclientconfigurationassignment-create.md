---
title: 创建 officeClientConfigurationAssignment
description: 将目标组添加到现有的策略。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 20ce558795abcf35cdcaad8386d1b875a2bf3f81
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27954272"
---
# <a name="create-officeclientconfigurationassignment"></a><span data-ttu-id="ca293-103">创建 officeClientConfigurationAssignment</span><span class="sxs-lookup"><span data-stu-id="ca293-103">Create officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="ca293-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ca293-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca293-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ca293-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ca293-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="ca293-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="ca293-107">将目标组添加到现有的策略。</span><span class="sxs-lookup"><span data-stu-id="ca293-107">Add a target group to an existing policy.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="ca293-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="ca293-108">Prerequisites</span></span>
<span data-ttu-id="ca293-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="ca293-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ca293-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ca293-111">Permission type</span></span>|<span data-ttu-id="ca293-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="ca293-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ca293-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ca293-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ca293-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ca293-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="ca293-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ca293-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ca293-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca293-116">Not supported.</span></span>|
|<span data-ttu-id="ca293-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ca293-117">Application</span></span>|<span data-ttu-id="ca293-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ca293-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ca293-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ca293-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /officeConfiguration/clientConfigurations/{key}/assignments
```

## <a name="request-headers"></a><span data-ttu-id="ca293-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ca293-120">Request headers</span></span>
|<span data-ttu-id="ca293-121">标头</span><span class="sxs-lookup"><span data-stu-id="ca293-121">Header</span></span>|<span data-ttu-id="ca293-122">值</span><span class="sxs-lookup"><span data-stu-id="ca293-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ca293-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ca293-123">Authorization</span></span>|<span data-ttu-id="ca293-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="ca293-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ca293-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ca293-125">Accept</span></span>|<span data-ttu-id="ca293-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ca293-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ca293-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="ca293-127">Request body</span></span>
<span data-ttu-id="ca293-128">在请求正文中，提供 officeClientConfigurationAssignment 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca293-128">In the request body, supply a JSON representation for the officeClientConfigurationAssignment object.</span></span>

<span data-ttu-id="ca293-129">下表显示时创建 officeClientConfigurationAssignment 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="ca293-129">The following table shows the properties that are required when you create the officeClientConfigurationAssignment.</span></span>

|<span data-ttu-id="ca293-130">属性</span><span class="sxs-lookup"><span data-stu-id="ca293-130">Property</span></span>|<span data-ttu-id="ca293-131">类型</span><span class="sxs-lookup"><span data-stu-id="ca293-131">Type</span></span>|<span data-ttu-id="ca293-132">说明</span><span class="sxs-lookup"><span data-stu-id="ca293-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ca293-133">id</span><span class="sxs-lookup"><span data-stu-id="ca293-133">id</span></span>|<span data-ttu-id="ca293-134">字符串</span><span class="sxs-lookup"><span data-stu-id="ca293-134">String</span></span>|<span data-ttu-id="ca293-135">OfficeConfigurationAssignment 的 id。</span><span class="sxs-lookup"><span data-stu-id="ca293-135">Id of the OfficeConfigurationAssignment.</span></span>|
|<span data-ttu-id="ca293-136">target</span><span class="sxs-lookup"><span data-stu-id="ca293-136">target</span></span>|[<span data-ttu-id="ca293-137">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="ca293-137">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="ca293-138">目标工作分配定义的管理员。</span><span class="sxs-lookup"><span data-stu-id="ca293-138">The target assignment defined by the admin.</span></span>|



## <a name="response"></a><span data-ttu-id="ca293-139">响应</span><span class="sxs-lookup"><span data-stu-id="ca293-139">Response</span></span>
<span data-ttu-id="ca293-140">如果成功，此方法返回`200 Created`响应代码和响应正文中的[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ca293-140">If successful, this method returns a `200 Created` response code and a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ca293-141">示例</span><span class="sxs-lookup"><span data-stu-id="ca293-141">Example</span></span>
### <a name="request"></a><span data-ttu-id="ca293-142">请求</span><span class="sxs-lookup"><span data-stu-id="ca293-142">Request</span></span>
<span data-ttu-id="ca293-143">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ca293-143">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}/assignments
Content-type: application/json
Content-length: 172

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="ca293-144">响应</span><span class="sxs-lookup"><span data-stu-id="ca293-144">Response</span></span>
<span data-ttu-id="ca293-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ca293-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
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



