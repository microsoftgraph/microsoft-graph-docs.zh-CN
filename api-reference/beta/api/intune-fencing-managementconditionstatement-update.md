---
title: 更新 managementConditionStatement
description: 更新 managementConditionStatement 对象的属性。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a18582a826ecf44afc1db137af98294f3637292c
ms.sourcegitcommit: 53dd31d323319fbd2ff7afc51b55a46efb8c5be3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/10/2019
ms.locfileid: "39943401"
---
# <a name="update-managementconditionstatement"></a><span data-ttu-id="95857-103">更新 managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="95857-103">Update managementConditionStatement</span></span>

> <span data-ttu-id="95857-104">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="95857-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="95857-105">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="95857-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="95857-106">更新[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="95857-106">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="95857-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="95857-107">Prerequisites</span></span>
<span data-ttu-id="95857-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="95857-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="95857-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="95857-110">Permission type</span></span>|<span data-ttu-id="95857-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="95857-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="95857-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="95857-112">Delegated (work or school account)</span></span>|<span data-ttu-id="95857-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95857-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="95857-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="95857-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="95857-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="95857-115">Not supported.</span></span>|
|<span data-ttu-id="95857-116">Application</span><span class="sxs-lookup"><span data-stu-id="95857-116">Application</span></span>|<span data-ttu-id="95857-117">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="95857-117">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="95857-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="95857-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a><span data-ttu-id="95857-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="95857-119">Request headers</span></span>
|<span data-ttu-id="95857-120">标头</span><span class="sxs-lookup"><span data-stu-id="95857-120">Header</span></span>|<span data-ttu-id="95857-121">值</span><span class="sxs-lookup"><span data-stu-id="95857-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="95857-122">授权</span><span class="sxs-lookup"><span data-stu-id="95857-122">Authorization</span></span>|<span data-ttu-id="95857-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="95857-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="95857-124">接受</span><span class="sxs-lookup"><span data-stu-id="95857-124">Accept</span></span>|<span data-ttu-id="95857-125">application/json</span><span class="sxs-lookup"><span data-stu-id="95857-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="95857-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="95857-126">Request body</span></span>
<span data-ttu-id="95857-127">在请求正文中，提供[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="95857-127">In the request body, supply a JSON representation for the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

<span data-ttu-id="95857-128">下表显示创建[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="95857-128">The following table shows the properties that are required when you create the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>

|<span data-ttu-id="95857-129">属性</span><span class="sxs-lookup"><span data-stu-id="95857-129">Property</span></span>|<span data-ttu-id="95857-130">类型</span><span class="sxs-lookup"><span data-stu-id="95857-130">Type</span></span>|<span data-ttu-id="95857-131">说明</span><span class="sxs-lookup"><span data-stu-id="95857-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="95857-132">id</span><span class="sxs-lookup"><span data-stu-id="95857-132">id</span></span>|<span data-ttu-id="95857-133">字符串</span><span class="sxs-lookup"><span data-stu-id="95857-133">String</span></span>|<span data-ttu-id="95857-134">管理条件语句的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="95857-134">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="95857-135">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="95857-135">System generated value assigned when created.</span></span>|
|<span data-ttu-id="95857-136">displayName</span><span class="sxs-lookup"><span data-stu-id="95857-136">displayName</span></span>|<span data-ttu-id="95857-137">String</span><span class="sxs-lookup"><span data-stu-id="95857-137">String</span></span>|<span data-ttu-id="95857-138">管理条件语句的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="95857-138">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="95857-139">说明</span><span class="sxs-lookup"><span data-stu-id="95857-139">description</span></span>|<span data-ttu-id="95857-140">字符串</span><span class="sxs-lookup"><span data-stu-id="95857-140">String</span></span>|<span data-ttu-id="95857-141">管理员定义的管理条件语句的说明。</span><span class="sxs-lookup"><span data-stu-id="95857-141">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="95857-142">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="95857-142">createdDateTime</span></span>|<span data-ttu-id="95857-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95857-143">DateTimeOffset</span></span>|<span data-ttu-id="95857-144">管理条件语句的创建时间。</span><span class="sxs-lookup"><span data-stu-id="95857-144">The time the management condition statement was created.</span></span> <span data-ttu-id="95857-145">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="95857-145">Generated service side.</span></span>|
|<span data-ttu-id="95857-146">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="95857-146">modifiedDateTime</span></span>|<span data-ttu-id="95857-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="95857-147">DateTimeOffset</span></span>|<span data-ttu-id="95857-148">上次修改管理条件语句的时间。</span><span class="sxs-lookup"><span data-stu-id="95857-148">The time the management condition statement was last modified.</span></span> <span data-ttu-id="95857-149">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="95857-149">Updated service side.</span></span>|
|<span data-ttu-id="95857-150">表达式</span><span class="sxs-lookup"><span data-stu-id="95857-150">expression</span></span>|[<span data-ttu-id="95857-151">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="95857-151">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="95857-152">用于评估管理条件语句是否已激活/停用的管理条件语句表达式。</span><span class="sxs-lookup"><span data-stu-id="95857-152">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="95857-153">eTag</span><span class="sxs-lookup"><span data-stu-id="95857-153">eTag</span></span>|<span data-ttu-id="95857-154">String</span><span class="sxs-lookup"><span data-stu-id="95857-154">String</span></span>|<span data-ttu-id="95857-155">管理条件语句的 ETag。</span><span class="sxs-lookup"><span data-stu-id="95857-155">ETag of the management condition statement.</span></span> <span data-ttu-id="95857-156">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="95857-156">Updated service side.</span></span>|
|<span data-ttu-id="95857-157">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="95857-157">applicablePlatforms</span></span>|<span data-ttu-id="95857-158">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="95857-158">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="95857-159">适用于此管理条件语句的平台。</span><span class="sxs-lookup"><span data-stu-id="95857-159">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="95857-160">这是通过查看与管理条件语句相关的管理条件和查找适用平台的交集计算得出的。</span><span class="sxs-lookup"><span data-stu-id="95857-160">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="95857-161">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="95857-161">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|



## <a name="response"></a><span data-ttu-id="95857-162">响应</span><span class="sxs-lookup"><span data-stu-id="95857-162">Response</span></span>
<span data-ttu-id="95857-163">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="95857-163">If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="95857-164">示例</span><span class="sxs-lookup"><span data-stu-id="95857-164">Example</span></span>

### <a name="request"></a><span data-ttu-id="95857-165">请求</span><span class="sxs-lookup"><span data-stu-id="95857-165">Request</span></span>
<span data-ttu-id="95857-166">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="95857-166">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}
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

### <a name="response"></a><span data-ttu-id="95857-167">响应</span><span class="sxs-lookup"><span data-stu-id="95857-167">Response</span></span>
<span data-ttu-id="95857-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="95857-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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





