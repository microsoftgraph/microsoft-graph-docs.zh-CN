---
title: 创建 managementConditionStatement
description: 创建新的 managementConditionStatement 对象。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 0c884f1b7239dc2f73438c007202ab783a5bdf1d
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27919153"
---
# <a name="create-managementconditionstatement"></a><span data-ttu-id="80a7b-103">创建 managementConditionStatement</span><span class="sxs-lookup"><span data-stu-id="80a7b-103">Create managementConditionStatement</span></span>

> <span data-ttu-id="80a7b-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="80a7b-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="80a7b-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="80a7b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="80a7b-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="80a7b-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="80a7b-107">创建新的[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="80a7b-107">Create a new [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="80a7b-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="80a7b-108">Prerequisites</span></span>
<span data-ttu-id="80a7b-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="80a7b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="80a7b-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="80a7b-111">Permission type</span></span>|<span data-ttu-id="80a7b-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="80a7b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="80a7b-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="80a7b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="80a7b-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="80a7b-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="80a7b-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="80a7b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="80a7b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="80a7b-116">Not supported.</span></span>|
|<span data-ttu-id="80a7b-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="80a7b-117">Application</span></span>|<span data-ttu-id="80a7b-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="80a7b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="80a7b-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="80a7b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditionStatements
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements
```

## <a name="request-headers"></a><span data-ttu-id="80a7b-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="80a7b-120">Request headers</span></span>
|<span data-ttu-id="80a7b-121">标头</span><span class="sxs-lookup"><span data-stu-id="80a7b-121">Header</span></span>|<span data-ttu-id="80a7b-122">值</span><span class="sxs-lookup"><span data-stu-id="80a7b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="80a7b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="80a7b-123">Authorization</span></span>|<span data-ttu-id="80a7b-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="80a7b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="80a7b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="80a7b-125">Accept</span></span>|<span data-ttu-id="80a7b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="80a7b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="80a7b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="80a7b-127">Request body</span></span>
<span data-ttu-id="80a7b-128">在请求正文中，提供 managementConditionStatement 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="80a7b-128">In the request body, supply a JSON representation for the managementConditionStatement object.</span></span>

<span data-ttu-id="80a7b-129">下表显示时创建 managementConditionStatement 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="80a7b-129">The following table shows the properties that are required when you create the managementConditionStatement.</span></span>

|<span data-ttu-id="80a7b-130">属性</span><span class="sxs-lookup"><span data-stu-id="80a7b-130">Property</span></span>|<span data-ttu-id="80a7b-131">类型</span><span class="sxs-lookup"><span data-stu-id="80a7b-131">Type</span></span>|<span data-ttu-id="80a7b-132">说明</span><span class="sxs-lookup"><span data-stu-id="80a7b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="80a7b-133">id</span><span class="sxs-lookup"><span data-stu-id="80a7b-133">id</span></span>|<span data-ttu-id="80a7b-134">字符串</span><span class="sxs-lookup"><span data-stu-id="80a7b-134">String</span></span>|<span data-ttu-id="80a7b-135">管理条件语句的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="80a7b-135">Unique identifier for the management condition statement.</span></span> <span data-ttu-id="80a7b-136">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="80a7b-136">System generated value assigned when created.</span></span>|
|<span data-ttu-id="80a7b-137">displayName</span><span class="sxs-lookup"><span data-stu-id="80a7b-137">displayName</span></span>|<span data-ttu-id="80a7b-138">字符串</span><span class="sxs-lookup"><span data-stu-id="80a7b-138">String</span></span>|<span data-ttu-id="80a7b-139">管理员定义管理条件语句的名称。</span><span class="sxs-lookup"><span data-stu-id="80a7b-139">The admin defined name of the management condition statement.</span></span>|
|<span data-ttu-id="80a7b-140">说明</span><span class="sxs-lookup"><span data-stu-id="80a7b-140">description</span></span>|<span data-ttu-id="80a7b-141">字符串</span><span class="sxs-lookup"><span data-stu-id="80a7b-141">String</span></span>|<span data-ttu-id="80a7b-142">管理员定义管理条件语句的说明。</span><span class="sxs-lookup"><span data-stu-id="80a7b-142">The admin defined description of the management condition statement.</span></span>|
|<span data-ttu-id="80a7b-143">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="80a7b-143">createdDateTime</span></span>|<span data-ttu-id="80a7b-144">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80a7b-144">DateTimeOffset</span></span>|<span data-ttu-id="80a7b-145">创建管理条件语句的时间。</span><span class="sxs-lookup"><span data-stu-id="80a7b-145">The time the management condition statement was created.</span></span> <span data-ttu-id="80a7b-146">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="80a7b-146">Generated service side.</span></span>|
|<span data-ttu-id="80a7b-147">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="80a7b-147">modifiedDateTime</span></span>|<span data-ttu-id="80a7b-148">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="80a7b-148">DateTimeOffset</span></span>|<span data-ttu-id="80a7b-149">管理条件语句上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="80a7b-149">The time the management condition statement was last modified.</span></span> <span data-ttu-id="80a7b-150">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="80a7b-150">Updated service side.</span></span>|
|<span data-ttu-id="80a7b-151">表达式</span><span class="sxs-lookup"><span data-stu-id="80a7b-151">expression</span></span>|[<span data-ttu-id="80a7b-152">managementConditionExpression</span><span class="sxs-lookup"><span data-stu-id="80a7b-152">managementConditionExpression</span></span>](../resources/intune-fencing-managementconditionexpression.md)|<span data-ttu-id="80a7b-153">用来评估如果管理条件语句的管理条件语句表达式已激活/停用。</span><span class="sxs-lookup"><span data-stu-id="80a7b-153">The management condition statement expression used to evaluate if a management condition statement was activated/deactivated.</span></span>|
|<span data-ttu-id="80a7b-154">eTag</span><span class="sxs-lookup"><span data-stu-id="80a7b-154">eTag</span></span>|<span data-ttu-id="80a7b-155">String</span><span class="sxs-lookup"><span data-stu-id="80a7b-155">String</span></span>|<span data-ttu-id="80a7b-156">管理条件语句的 ETag。</span><span class="sxs-lookup"><span data-stu-id="80a7b-156">ETag of the management condition statement.</span></span> <span data-ttu-id="80a7b-157">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="80a7b-157">Updated service side.</span></span>|
|<span data-ttu-id="80a7b-158">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="80a7b-158">applicablePlatforms</span></span>|<span data-ttu-id="80a7b-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="80a7b-159">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="80a7b-160">此管理条件语句适用的平台。</span><span class="sxs-lookup"><span data-stu-id="80a7b-160">The applicable platforms for this management condition statement.</span></span>
<span data-ttu-id="80a7b-161">这从查找管理相关的管理条件计算条件语句并查找适用平台的交点。</span><span class="sxs-lookup"><span data-stu-id="80a7b-161">This is calculated from looking the management conditions associated to the management condition statement and finding the intersection of applicable platforms.</span></span> <span data-ttu-id="80a7b-162">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="80a7b-162">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|



## <a name="response"></a><span data-ttu-id="80a7b-163">响应</span><span class="sxs-lookup"><span data-stu-id="80a7b-163">Response</span></span>
<span data-ttu-id="80a7b-164">如果成功，此方法返回`201 Created`响应代码和响应正文中的[managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md)对象。</span><span class="sxs-lookup"><span data-stu-id="80a7b-164">If successful, this method returns a `201 Created` response code and a [managementConditionStatement](../resources/intune-fencing-managementconditionstatement.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="80a7b-165">示例</span><span class="sxs-lookup"><span data-stu-id="80a7b-165">Example</span></span>
### <a name="request"></a><span data-ttu-id="80a7b-166">请求</span><span class="sxs-lookup"><span data-stu-id="80a7b-166">Request</span></span>
<span data-ttu-id="80a7b-167">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="80a7b-167">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="80a7b-168">响应</span><span class="sxs-lookup"><span data-stu-id="80a7b-168">Response</span></span>
<span data-ttu-id="80a7b-p108">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="80a7b-p108">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





