---
title: 创建 managementConditionStatement
description: 创建新的 managementConditionStatement 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: eba9d3f96d7d3a8b1f855c94b18aab6a6450651f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417355"
---
# <a name="create-managementconditionstatement"></a><span data-ttu-id="fc35e-103">创建 managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="fc35e-103">Create managementConditionStatement</span></span>

> <span data-ttu-id="fc35e-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="fc35e-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="fc35e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fc35e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fc35e-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="fc35e-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="fc35e-107">创建新的[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fc35e-107">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="fc35e-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fc35e-108">Prerequisites</span></span>
<span data-ttu-id="fc35e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="fc35e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="fc35e-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fc35e-111">Permission type</span></span>|<span data-ttu-id="fc35e-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fc35e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fc35e-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fc35e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fc35e-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fc35e-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fc35e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fc35e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fc35e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc35e-116">Not supported.</span></span>|
|<span data-ttu-id="fc35e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fc35e-117">Application</span></span>|<span data-ttu-id="fc35e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fc35e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fc35e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fc35e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="fc35e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fc35e-120">Request headers</span></span>
|<span data-ttu-id="fc35e-121">标头</span><span class="sxs-lookup"><span data-stu-id="fc35e-121">Header</span></span>|<span data-ttu-id="fc35e-122">值</span><span class="sxs-lookup"><span data-stu-id="fc35e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fc35e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fc35e-123">Authorization</span></span>|<span data-ttu-id="fc35e-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fc35e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fc35e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fc35e-125">Accept</span></span>|<span data-ttu-id="fc35e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fc35e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fc35e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fc35e-127">Request body</span></span>
<span data-ttu-id="fc35e-128">在请求正文中，提供 managementConditionStatement 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fc35e-128">In the request body, supply a JSON representation for the managementConditionStatement object.</span></span>

<span data-ttu-id="fc35e-129">下表显示时创建 managementConditionStatement 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fc35e-129">The following table shows the properties that are required when you create the managementConditionStatement.</span></span>

|<span data-ttu-id="fc35e-130">属性</span><span class="sxs-lookup"><span data-stu-id="fc35e-130">Property</span></span>|<span data-ttu-id="fc35e-131">类型</span><span class="sxs-lookup"><span data-stu-id="fc35e-131">Type</span></span>|<span data-ttu-id="fc35e-132">说明</span><span class="sxs-lookup"><span data-stu-id="fc35e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fc35e-133">id</span><span class="sxs-lookup"><span data-stu-id="fc35e-133">id</span></span>|<span data-ttu-id="fc35e-134">String</span><span class="sxs-lookup"><span data-stu-id="fc35e-134">String</span></span>|<span data-ttu-id="fc35e-135">管理条件语句的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fc35e-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="fc35e-136">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="fc35e-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="fc35e-137">displayName</span><span class="sxs-lookup"><span data-stu-id="fc35e-137">displayName</span></span>|<span data-ttu-id="fc35e-138">String</span><span class="sxs-lookup"><span data-stu-id="fc35e-138">String</span></span>|<span data-ttu-id="fc35e-139">管理员定义管理条件语句的名称。</span><span class="sxs-lookup"><span data-stu-id="fc35e-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="fc35e-140">说明</span><span class="sxs-lookup"><span data-stu-id="fc35e-140">description</span></span>|<span data-ttu-id="fc35e-141">String</span><span class="sxs-lookup"><span data-stu-id="fc35e-141">String</span></span>|<span data-ttu-id="fc35e-142">管理员定义管理条件语句的说明。</span><span class="sxs-lookup"><span data-stu-id="fc35e-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="fc35e-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fc35e-143">createdDateTime</span></span>|<span data-ttu-id="fc35e-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc35e-144">DateTimeOffset</span></span>|<span data-ttu-id="fc35e-145">创建管理条件语句的时间。</span><span class="sxs-lookup"><span data-stu-id="fc35e-145">The time the management condition statement was created.</span></span> <span data-ttu-id="fc35e-146">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="fc35e-146">Generated service side.</span></span>|
|<span data-ttu-id="fc35e-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fc35e-147">modifiedDateTime</span></span>|<span data-ttu-id="fc35e-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fc35e-148">DateTimeOffset</span></span>|<span data-ttu-id="fc35e-149">管理条件语句上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="fc35e-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="fc35e-150">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="fc35e-150">Updated service side.</span></span>|
|<span data-ttu-id="fc35e-151">表达式</span><span class="sxs-lookup"><span data-stu-id="fc35e-151">expression</span></span>|[<span data-ttu-id="fc35e-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="fc35e-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="fc35e-153">用来评估如果管理条件语句的管理条件语句表达式已激活/停用。</span><span class="sxs-lookup"><span data-stu-id="fc35e-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="fc35e-154">eTag</span><span class="sxs-lookup"><span data-stu-id="fc35e-154">eTag</span></span>|<span data-ttu-id="fc35e-155">String</span><span class="sxs-lookup"><span data-stu-id="fc35e-155">String</span></span>|<span data-ttu-id="fc35e-156">管理条件语句的 ETag。</span><span class="sxs-lookup"><span data-stu-id="fc35e-156">ETag of the management condition statement.</span></span> <span data-ttu-id="fc35e-157">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="fc35e-157">Updated service side.</span></span>|
|<span data-ttu-id="fc35e-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="fc35e-158">applicablePlatforms</span></span>|<span data-ttu-id="fc35e-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="fc35e-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="fc35e-160">此管理条件语句适用的平台。</span><span class="sxs-lookup"><span data-stu-id="fc35e-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="fc35e-161">这从查找管理相关的管理条件计算条件语句并查找适用平台的交点。</span><span class="sxs-lookup"><span data-stu-id="fc35e-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="fc35e-162">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="fc35e-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="fc35e-163">响应</span><span class="sxs-lookup"><span data-stu-id="fc35e-163">Response</span></span>
<span data-ttu-id="fc35e-164">如果成功，此方法返回`201 Created`响应代码和响应正文中的[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fc35e-164">If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fc35e-165">示例</span><span class="sxs-lookup"><span data-stu-id="fc35e-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="fc35e-166">请求</span><span class="sxs-lookup"><span data-stu-id="fc35e-166">Request</span></span>
<span data-ttu-id="fc35e-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fc35e-167">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements
Content-type: application/json
Content-length: 323

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "displayName": "Display Name value",
  "description": "Description value",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```

### <a name="response"></a><span data-ttu-id="fc35e-168">响应</span><span class="sxs-lookup"><span data-stu-id="fc35e-168">Response</span></span>
<span data-ttu-id="fc35e-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fc35e-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 491

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpression"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```




