---
title: 更新 managementConditionStatement
description: 更新 managementConditionStatement 对象的属性。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 02d5301ca81bf5b1479454f65a6c9e9630a8f284
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29417040"
---
# <a name="update-managementconditionstatement"></a><span data-ttu-id="f8836-103">更新 managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="f8836-103">Update managementConditionStatement</span></span>

> <span data-ttu-id="f8836-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="f8836-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="f8836-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f8836-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f8836-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="f8836-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f8836-107">更新[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="f8836-107">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f8836-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="f8836-108">Prerequisites</span></span>
<span data-ttu-id="f8836-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="f8836-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="f8836-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="f8836-111">Permission type</span></span>|<span data-ttu-id="f8836-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f8836-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f8836-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f8836-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f8836-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f8836-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="f8836-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f8836-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f8836-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8836-116">Not supported.</span></span>|
|<span data-ttu-id="f8836-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="f8836-117">Application</span></span>|<span data-ttu-id="f8836-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f8836-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f8836-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f8836-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a><span data-ttu-id="f8836-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="f8836-120">Request headers</span></span>
|<span data-ttu-id="f8836-121">标头</span><span class="sxs-lookup"><span data-stu-id="f8836-121">Header</span></span>|<span data-ttu-id="f8836-122">值</span><span class="sxs-lookup"><span data-stu-id="f8836-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f8836-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f8836-123">Authorization</span></span>|<span data-ttu-id="f8836-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="f8836-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f8836-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f8836-125">Accept</span></span>|<span data-ttu-id="f8836-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f8836-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f8836-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f8836-127">Request body</span></span>
<span data-ttu-id="f8836-128">在请求正文中，提供[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f8836-128">In the request body, supply a JSON representation for the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

<span data-ttu-id="f8836-129">下表显示时创建[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f8836-129">The following table shows the properties that are required when you create the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>

|<span data-ttu-id="f8836-130">属性</span><span class="sxs-lookup"><span data-stu-id="f8836-130">Property</span></span>|<span data-ttu-id="f8836-131">类型</span><span class="sxs-lookup"><span data-stu-id="f8836-131">Type</span></span>|<span data-ttu-id="f8836-132">说明</span><span class="sxs-lookup"><span data-stu-id="f8836-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f8836-133">id</span><span class="sxs-lookup"><span data-stu-id="f8836-133">id</span></span>|<span data-ttu-id="f8836-134">String</span><span class="sxs-lookup"><span data-stu-id="f8836-134">String</span></span>|<span data-ttu-id="f8836-135">管理条件语句的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="f8836-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="f8836-136">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="f8836-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="f8836-137">displayName</span><span class="sxs-lookup"><span data-stu-id="f8836-137">displayName</span></span>|<span data-ttu-id="f8836-138">String</span><span class="sxs-lookup"><span data-stu-id="f8836-138">String</span></span>|<span data-ttu-id="f8836-139">管理员定义管理条件语句的名称。</span><span class="sxs-lookup"><span data-stu-id="f8836-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="f8836-140">说明</span><span class="sxs-lookup"><span data-stu-id="f8836-140">description</span></span>|<span data-ttu-id="f8836-141">String</span><span class="sxs-lookup"><span data-stu-id="f8836-141">String</span></span>|<span data-ttu-id="f8836-142">管理员定义管理条件语句的说明。</span><span class="sxs-lookup"><span data-stu-id="f8836-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="f8836-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f8836-143">createdDateTime</span></span>|<span data-ttu-id="f8836-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8836-144">DateTimeOffset</span></span>|<span data-ttu-id="f8836-145">创建管理条件语句的时间。</span><span class="sxs-lookup"><span data-stu-id="f8836-145">The time the management condition statement was created.</span></span> <span data-ttu-id="f8836-146">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="f8836-146">Generated service side.</span></span>|
|<span data-ttu-id="f8836-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f8836-147">modifiedDateTime</span></span>|<span data-ttu-id="f8836-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f8836-148">DateTimeOffset</span></span>|<span data-ttu-id="f8836-149">管理条件语句上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="f8836-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="f8836-150">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="f8836-150">Updated service side.</span></span>|
|<span data-ttu-id="f8836-151">表达式</span><span class="sxs-lookup"><span data-stu-id="f8836-151">expression</span></span>|[<span data-ttu-id="f8836-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="f8836-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="f8836-153">用来评估如果管理条件语句的管理条件语句表达式已激活/停用。</span><span class="sxs-lookup"><span data-stu-id="f8836-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="f8836-154">eTag</span><span class="sxs-lookup"><span data-stu-id="f8836-154">eTag</span></span>|<span data-ttu-id="f8836-155">String</span><span class="sxs-lookup"><span data-stu-id="f8836-155">String</span></span>|<span data-ttu-id="f8836-156">管理条件语句的 ETag。</span><span class="sxs-lookup"><span data-stu-id="f8836-156">ETag of the management condition statement.</span></span> <span data-ttu-id="f8836-157">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="f8836-157">Updated service side.</span></span>|
|<span data-ttu-id="f8836-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="f8836-158">applicablePlatforms</span></span>|<span data-ttu-id="f8836-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="f8836-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="f8836-160">此管理条件语句适用的平台。</span><span class="sxs-lookup"><span data-stu-id="f8836-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="f8836-161">这从查找管理相关的管理条件计算条件语句并查找适用平台的交点。</span><span class="sxs-lookup"><span data-stu-id="f8836-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="f8836-162">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="f8836-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="f8836-163">响应</span><span class="sxs-lookup"><span data-stu-id="f8836-163">Response</span></span>
<span data-ttu-id="f8836-164">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="f8836-164">If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f8836-165">示例</span><span class="sxs-lookup"><span data-stu-id="f8836-165">Example</span></span>

### <a name="request"></a><span data-ttu-id="f8836-166">请求</span><span class="sxs-lookup"><span data-stu-id="f8836-166">Request</span></span>
<span data-ttu-id="f8836-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="f8836-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f8836-168">响应</span><span class="sxs-lookup"><span data-stu-id="f8836-168">Response</span></span>
<span data-ttu-id="f8836-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f8836-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




