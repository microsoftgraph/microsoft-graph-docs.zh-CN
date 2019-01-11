---
title: 更新 managementConditionStatement
description: 更新 managementConditionStatement 对象的属性。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 33bee3fe6e386d9d426eb0763ccb608cbc6242e3
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27829447"
---
# <a name="update-managementconditionstatement"></a><span data-ttu-id="800bf-103">更新 managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="800bf-103">Update managementConditionStatement</span></span>

> <span data-ttu-id="800bf-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="800bf-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="800bf-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="800bf-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="800bf-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="800bf-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="800bf-107">更新[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的属性。</span><span class="sxs-lookup"><span data-stu-id="800bf-107">Update the properties of a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="800bf-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="800bf-108">Prerequisites</span></span>
<span data-ttu-id="800bf-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="800bf-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="800bf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="800bf-111">Permission type</span></span>|<span data-ttu-id="800bf-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="800bf-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="800bf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="800bf-113">Delegated (work or school account)</span></span>|<span data-ttu-id="800bf-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="800bf-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="800bf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="800bf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="800bf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="800bf-116">Not supported.</span></span>|
|<span data-ttu-id="800bf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="800bf-117">Application</span></span>|<span data-ttu-id="800bf-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="800bf-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="800bf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="800bf-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditionStatements/{managementConditionStatementId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}
```

## <a name="request-headers"></a><span data-ttu-id="800bf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="800bf-120">Request headers</span></span>
|<span data-ttu-id="800bf-121">标头</span><span class="sxs-lookup"><span data-stu-id="800bf-121">Header</span></span>|<span data-ttu-id="800bf-122">值</span><span class="sxs-lookup"><span data-stu-id="800bf-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="800bf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="800bf-123">Authorization</span></span>|<span data-ttu-id="800bf-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="800bf-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="800bf-125">Accept</span><span class="sxs-lookup"><span data-stu-id="800bf-125">Accept</span></span>|<span data-ttu-id="800bf-126">application/json</span><span class="sxs-lookup"><span data-stu-id="800bf-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="800bf-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="800bf-127">Request body</span></span>
<span data-ttu-id="800bf-128">在请求正文中，提供[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="800bf-128">In the request body, supply a JSON representation for the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>

<span data-ttu-id="800bf-129">下表显示时创建[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)所需的属性。</span><span class="sxs-lookup"><span data-stu-id="800bf-129">The following table shows the properties that are required when you create the [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md).</span></span>

|<span data-ttu-id="800bf-130">属性</span><span class="sxs-lookup"><span data-stu-id="800bf-130">Property</span></span>|<span data-ttu-id="800bf-131">类型</span><span class="sxs-lookup"><span data-stu-id="800bf-131">Type</span></span>|<span data-ttu-id="800bf-132">说明</span><span class="sxs-lookup"><span data-stu-id="800bf-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="800bf-133">id</span><span class="sxs-lookup"><span data-stu-id="800bf-133">id</span></span>|<span data-ttu-id="800bf-134">字符串</span><span class="sxs-lookup"><span data-stu-id="800bf-134">String</span></span>|<span data-ttu-id="800bf-135">管理条件语句的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="800bf-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="800bf-136">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="800bf-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="800bf-137">displayName</span><span class="sxs-lookup"><span data-stu-id="800bf-137">displayName</span></span>|<span data-ttu-id="800bf-138">字符串</span><span class="sxs-lookup"><span data-stu-id="800bf-138">String</span></span>|<span data-ttu-id="800bf-139">管理员定义管理条件语句的名称。</span><span class="sxs-lookup"><span data-stu-id="800bf-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="800bf-140">说明</span><span class="sxs-lookup"><span data-stu-id="800bf-140">description</span></span>|<span data-ttu-id="800bf-141">字符串</span><span class="sxs-lookup"><span data-stu-id="800bf-141">String</span></span>|<span data-ttu-id="800bf-142">管理员定义管理条件语句的说明。</span><span class="sxs-lookup"><span data-stu-id="800bf-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="800bf-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="800bf-143">createdDateTime</span></span>|<span data-ttu-id="800bf-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="800bf-144">DateTimeOffset</span></span>|<span data-ttu-id="800bf-145">创建管理条件语句的时间。</span><span class="sxs-lookup"><span data-stu-id="800bf-145">The time the management condition statement was created.</span></span> <span data-ttu-id="800bf-146">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="800bf-146">Generated service side.</span></span>|
|<span data-ttu-id="800bf-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="800bf-147">modifiedDateTime</span></span>|<span data-ttu-id="800bf-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="800bf-148">DateTimeOffset</span></span>|<span data-ttu-id="800bf-149">管理条件语句上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="800bf-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="800bf-150">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="800bf-150">Updated service side.</span></span>|
|<span data-ttu-id="800bf-151">表达式</span><span class="sxs-lookup"><span data-stu-id="800bf-151">expression</span></span>|[<span data-ttu-id="800bf-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="800bf-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="800bf-153">用来评估如果管理条件语句的管理条件语句表达式已激活/停用。</span><span class="sxs-lookup"><span data-stu-id="800bf-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="800bf-154">eTag</span><span class="sxs-lookup"><span data-stu-id="800bf-154">eTag</span></span>|<span data-ttu-id="800bf-155">String</span><span class="sxs-lookup"><span data-stu-id="800bf-155">String</span></span>|<span data-ttu-id="800bf-156">管理条件语句的 ETag。</span><span class="sxs-lookup"><span data-stu-id="800bf-156">ETag of the management condition statement.</span></span> <span data-ttu-id="800bf-157">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="800bf-157">Updated service side.</span></span>|
|<span data-ttu-id="800bf-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="800bf-158">applicablePlatforms</span></span>|<span data-ttu-id="800bf-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="800bf-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="800bf-160">此管理条件语句适用的平台。</span><span class="sxs-lookup"><span data-stu-id="800bf-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="800bf-161">这从查找管理相关的管理条件计算条件语句并查找适用平台的交点。</span><span class="sxs-lookup"><span data-stu-id="800bf-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="800bf-162">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="800bf-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="800bf-163">响应</span><span class="sxs-lookup"><span data-stu-id="800bf-163">Response</span></span>
<span data-ttu-id="800bf-164">如果成功，此方法返回`200 OK`响应代码和响应正文中的更新的[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="800bf-164">If successful, this method returns a `200 OK` response code and an updated [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="800bf-165">示例</span><span class="sxs-lookup"><span data-stu-id="800bf-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="800bf-166">请求</span><span class="sxs-lookup"><span data-stu-id="800bf-166">Request</span></span>
<span data-ttu-id="800bf-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="800bf-167">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditionStatements/{managementConditionStatementId}
Content-type: application/json
Content-length: 256

{
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

### <a name="response"></a><span data-ttu-id="800bf-168">响应</span><span class="sxs-lookup"><span data-stu-id="800bf-168">Response</span></span>
<span data-ttu-id="800bf-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="800bf-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





