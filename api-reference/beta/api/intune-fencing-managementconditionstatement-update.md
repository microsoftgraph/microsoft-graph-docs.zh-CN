---
title: 更新 managementConditionStatement
description: 更新 managementConditionStatement 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: 819d17f2884c1581a088646d4f3e107a32af78b0
ms.sourcegitcommit: f592c9ff96ceeb40caa67fcfe90fe6c8525cb7d2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/23/2021
ms.locfileid: "51153606"
---
# <a name="update-managementconditionstatement"></a><span data-ttu-id="d8184-103">更新 managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="d8184-103">Update managementConditionStatement</span></span>

<span data-ttu-id="d8184-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d8184-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="d8184-105">**重要提示：** /beta 版本下的 Microsoft Graph API 可能会更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="d8184-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d8184-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="d8184-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d8184-107">更新 [managementConditionStatement 对象](../resources/intune-fencing-managementconditionstatement.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="d8184-107">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d8184-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="d8184-108">Prerequisites</span></span>
<span data-ttu-id="d8184-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="d8184-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d8184-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="d8184-111">Permission type</span></span>|<span data-ttu-id="d8184-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="d8184-112">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d8184-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="d8184-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d8184-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8184-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="d8184-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="d8184-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d8184-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="d8184-116">Not supported.</span></span>|
|<span data-ttu-id="d8184-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="d8184-117">Application</span></span>|<span data-ttu-id="d8184-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d8184-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="d8184-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="d8184-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a><span data-ttu-id="d8184-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="d8184-120">Request headers</span></span>
|<span data-ttu-id="d8184-121">标头</span><span class="sxs-lookup"><span data-stu-id="d8184-121">Header</span></span>|<span data-ttu-id="d8184-122">值</span><span class="sxs-lookup"><span data-stu-id="d8184-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d8184-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d8184-123">Authorization</span></span>|<span data-ttu-id="d8184-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="d8184-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d8184-125">接受</span><span class="sxs-lookup"><span data-stu-id="d8184-125">Accept</span></span>|<span data-ttu-id="d8184-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d8184-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d8184-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="d8184-127">Request body</span></span>
<span data-ttu-id="d8184-128">在请求正文中，提供 [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d8184-128">In the request body, supply a JSON representation for the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

<span data-ttu-id="d8184-129">下表显示创建 [managementConditionStatement 时所需的属性](../resources/intune-fencing-managementconditionstatement.md)。</span><span class="sxs-lookup"><span data-stu-id="d8184-129">The following table shows the properties that are required when you create the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>

|<span data-ttu-id="d8184-130">属性</span><span class="sxs-lookup"><span data-stu-id="d8184-130">Property</span></span>|<span data-ttu-id="d8184-131">类型</span><span class="sxs-lookup"><span data-stu-id="d8184-131">Type</span></span>|<span data-ttu-id="d8184-132">说明</span><span class="sxs-lookup"><span data-stu-id="d8184-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d8184-133">id</span><span class="sxs-lookup"><span data-stu-id="d8184-133">id</span></span>|<span data-ttu-id="d8184-134">String</span><span class="sxs-lookup"><span data-stu-id="d8184-134">String</span></span>|<span data-ttu-id="d8184-135">管理条件语句的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="d8184-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="d8184-136">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="d8184-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="d8184-137">displayName</span><span class="sxs-lookup"><span data-stu-id="d8184-137">displayName</span></span>|<span data-ttu-id="d8184-138">String</span><span class="sxs-lookup"><span data-stu-id="d8184-138">String</span></span>|<span data-ttu-id="d8184-139">管理员定义的管理条件声明的名称。</span><span class="sxs-lookup"><span data-stu-id="d8184-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="d8184-140">说明</span><span class="sxs-lookup"><span data-stu-id="d8184-140">description</span></span>|<span data-ttu-id="d8184-141">String</span><span class="sxs-lookup"><span data-stu-id="d8184-141">String</span></span>|<span data-ttu-id="d8184-142">管理员定义的管理条件声明的说明。</span><span class="sxs-lookup"><span data-stu-id="d8184-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="d8184-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="d8184-143">createdDateTime</span></span>|<span data-ttu-id="d8184-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8184-144">DateTimeOffset</span></span>|<span data-ttu-id="d8184-145">创建管理条件语句的时间。</span><span class="sxs-lookup"><span data-stu-id="d8184-145">The time the management condition statement was created.</span></span> <span data-ttu-id="d8184-146">生成的服务器端。</span><span class="sxs-lookup"><span data-stu-id="d8184-146">Generated service side.</span></span>|
|<span data-ttu-id="d8184-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="d8184-147">modifiedDateTime</span></span>|<span data-ttu-id="d8184-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d8184-148">DateTimeOffset</span></span>|<span data-ttu-id="d8184-149">上次修改管理条件语句的时间。</span><span class="sxs-lookup"><span data-stu-id="d8184-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="d8184-150">更新的服务器端。</span><span class="sxs-lookup"><span data-stu-id="d8184-150">Updated service side.</span></span>|
|<span data-ttu-id="d8184-151">表达式</span><span class="sxs-lookup"><span data-stu-id="d8184-151">expression</span></span>|[<span data-ttu-id="d8184-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="d8184-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="d8184-153">用于评估管理条件语句是否被激活/停用的管理条件语句表达式。</span><span class="sxs-lookup"><span data-stu-id="d8184-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="d8184-154">eTag</span><span class="sxs-lookup"><span data-stu-id="d8184-154">eTag</span></span>|<span data-ttu-id="d8184-155">String</span><span class="sxs-lookup"><span data-stu-id="d8184-155">String</span></span>|<span data-ttu-id="d8184-156">管理条件声明的 ETag。</span><span class="sxs-lookup"><span data-stu-id="d8184-156">ETag of the management condition statement.</span></span> <span data-ttu-id="d8184-157">更新的服务器端。</span><span class="sxs-lookup"><span data-stu-id="d8184-157">Updated service side.</span></span>|
|<span data-ttu-id="d8184-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="d8184-158">applicablePlatforms</span></span>|<span data-ttu-id="d8184-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="d8184-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="d8184-160">此管理条件声明的适用平台。</span><span class="sxs-lookup"><span data-stu-id="d8184-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="d8184-161">这是通过查看与管理条件声明关联的管理条件并查找适用平台的交集得出的。</span><span class="sxs-lookup"><span data-stu-id="d8184-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="d8184-162">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="d8184-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|



## <a name="response"></a><span data-ttu-id="d8184-163">响应</span><span class="sxs-lookup"><span data-stu-id="d8184-163">Response</span></span>
<span data-ttu-id="d8184-164">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="d8184-164">If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d8184-165">示例</span><span class="sxs-lookup"><span data-stu-id="d8184-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="d8184-166">请求</span><span class="sxs-lookup"><span data-stu-id="d8184-166">Request</span></span>
<span data-ttu-id="d8184-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="d8184-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}
Content-type: application/json
Content-length: 358

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "displayName": "Display Name value",
  "description": "Description value",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpressionString",
    "value": "Value value"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```

### <a name="response"></a><span data-ttu-id="d8184-168">响应</span><span class="sxs-lookup"><span data-stu-id="d8184-168">Response</span></span>
<span data-ttu-id="d8184-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="d8184-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 526

{
  "@odata.type": "#microsoft.graph.managementConditionStatement",
  "id": "bedb0c00-0c00-bedb-000c-dbbe000cdbbe",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "expression": {
    "@odata.type": "microsoft.graph.managementConditionExpressionString",
    "value": "Value value"
  },
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ]
}
```




