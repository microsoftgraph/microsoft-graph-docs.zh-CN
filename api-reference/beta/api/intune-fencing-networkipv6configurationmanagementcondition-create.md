---
title: 创建 networkIPv6ConfigurationManagementCondition
description: 创建新的 networkIPv6ConfigurationManagementCondition 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 37ae2f489f41648b0873a45c850603821c09d9b3
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42465637"
---
# <a name="create-networkipv6configurationmanagementcondition"></a><span data-ttu-id="6a7b5-103">创建 networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="6a7b5-103">Create networkIPv6ConfigurationManagementCondition</span></span>

<span data-ttu-id="6a7b5-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="6a7b5-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="6a7b5-105">**重要说明：**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="6a7b5-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="6a7b5-107">创建新的[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-107">Create a new [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="6a7b5-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="6a7b5-108">Prerequisites</span></span>
<span data-ttu-id="6a7b5-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="6a7b5-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="6a7b5-111">Permission type</span></span>|<span data-ttu-id="6a7b5-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="6a7b5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="6a7b5-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6a7b5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="6a7b5-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a7b5-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="6a7b5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6a7b5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="6a7b5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-116">Not supported.</span></span>|
|<span data-ttu-id="6a7b5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="6a7b5-117">Application</span></span>|<span data-ttu-id="6a7b5-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="6a7b5-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="6a7b5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6a7b5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="6a7b5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="6a7b5-120">Request headers</span></span>
|<span data-ttu-id="6a7b5-121">标头</span><span class="sxs-lookup"><span data-stu-id="6a7b5-121">Header</span></span>|<span data-ttu-id="6a7b5-122">值</span><span class="sxs-lookup"><span data-stu-id="6a7b5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="6a7b5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="6a7b5-123">Authorization</span></span>|<span data-ttu-id="6a7b5-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="6a7b5-125">接受</span><span class="sxs-lookup"><span data-stu-id="6a7b5-125">Accept</span></span>|<span data-ttu-id="6a7b5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="6a7b5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="6a7b5-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="6a7b5-127">Request body</span></span>
<span data-ttu-id="6a7b5-128">在请求正文中，提供 networkIPv6ConfigurationManagementCondition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-128">In the request body, supply a JSON representation for the networkIPv6ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="6a7b5-129">下表显示创建 networkIPv6ConfigurationManagementCondition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-129">The following table shows the properties that are required when you create the networkIPv6ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="6a7b5-130">属性</span><span class="sxs-lookup"><span data-stu-id="6a7b5-130">Property</span></span>|<span data-ttu-id="6a7b5-131">类型</span><span class="sxs-lookup"><span data-stu-id="6a7b5-131">Type</span></span>|<span data-ttu-id="6a7b5-132">说明</span><span class="sxs-lookup"><span data-stu-id="6a7b5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6a7b5-133">id</span><span class="sxs-lookup"><span data-stu-id="6a7b5-133">id</span></span>|<span data-ttu-id="6a7b5-134">字符串</span><span class="sxs-lookup"><span data-stu-id="6a7b5-134">String</span></span>|<span data-ttu-id="6a7b5-135">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="6a7b5-136">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-136">System generated value assigned when created.</span></span> <span data-ttu-id="6a7b5-137">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="6a7b5-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6a7b5-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="6a7b5-138">uniqueName</span></span>|<span data-ttu-id="6a7b5-139">String</span><span class="sxs-lookup"><span data-stu-id="6a7b5-139">String</span></span>|<span data-ttu-id="6a7b5-140">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-140">Unique name for the management condition.</span></span> <span data-ttu-id="6a7b5-141">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-141">Used in management condition expressions.</span></span> <span data-ttu-id="6a7b5-142">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="6a7b5-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6a7b5-143">displayName</span><span class="sxs-lookup"><span data-stu-id="6a7b5-143">displayName</span></span>|<span data-ttu-id="6a7b5-144">String</span><span class="sxs-lookup"><span data-stu-id="6a7b5-144">String</span></span>|<span data-ttu-id="6a7b5-145">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="6a7b5-146">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="6a7b5-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6a7b5-147">说明</span><span class="sxs-lookup"><span data-stu-id="6a7b5-147">description</span></span>|<span data-ttu-id="6a7b5-148">字符串</span><span class="sxs-lookup"><span data-stu-id="6a7b5-148">String</span></span>|<span data-ttu-id="6a7b5-149">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="6a7b5-150">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="6a7b5-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6a7b5-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6a7b5-151">createdDateTime</span></span>|<span data-ttu-id="6a7b5-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a7b5-152">DateTimeOffset</span></span>|<span data-ttu-id="6a7b5-153">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-153">The time the management condition was created.</span></span> <span data-ttu-id="6a7b5-154">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-154">Generated service side.</span></span> <span data-ttu-id="6a7b5-155">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="6a7b5-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6a7b5-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6a7b5-156">modifiedDateTime</span></span>|<span data-ttu-id="6a7b5-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6a7b5-157">DateTimeOffset</span></span>|<span data-ttu-id="6a7b5-158">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-158">The time the management condition was last modified.</span></span> <span data-ttu-id="6a7b5-159">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-159">Updated service side.</span></span> <span data-ttu-id="6a7b5-160">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="6a7b5-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6a7b5-161">eTag</span><span class="sxs-lookup"><span data-stu-id="6a7b5-161">eTag</span></span>|<span data-ttu-id="6a7b5-162">String</span><span class="sxs-lookup"><span data-stu-id="6a7b5-162">String</span></span>|<span data-ttu-id="6a7b5-163">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-163">ETag of the management condition.</span></span> <span data-ttu-id="6a7b5-164">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-164">Updated service side.</span></span> <span data-ttu-id="6a7b5-165">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="6a7b5-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="6a7b5-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="6a7b5-166">applicablePlatforms</span></span>|<span data-ttu-id="6a7b5-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="6a7b5-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="6a7b5-168">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="6a7b5-169">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="6a7b5-170">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="6a7b5-171">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="6a7b5-171">ipV6Prefix</span></span>|<span data-ttu-id="6a7b5-172">String</span><span class="sxs-lookup"><span data-stu-id="6a7b5-172">String</span></span>|<span data-ttu-id="6a7b5-173">要连接到的 IPv6 子网。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-173">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="6a7b5-174">例如2001： db8：：/32</span><span class="sxs-lookup"><span data-stu-id="6a7b5-174">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="6a7b5-175">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="6a7b5-175">ipV6Gateway</span></span>|<span data-ttu-id="6a7b5-176">String</span><span class="sxs-lookup"><span data-stu-id="6a7b5-176">String</span></span>|<span data-ttu-id="6a7b5-177">IPv6 网关地址。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-177">The IPv6 gateway address to.</span></span> <span data-ttu-id="6a7b5-178">例如2001： db8：：1</span><span class="sxs-lookup"><span data-stu-id="6a7b5-178">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="6a7b5-179">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="6a7b5-179">ipV6DNSServerList</span></span>|<span data-ttu-id="6a7b5-180">String 集合</span><span class="sxs-lookup"><span data-stu-id="6a7b5-180">String collection</span></span>|<span data-ttu-id="6a7b5-181">为适配器配置的 IPv6 DNS 服务器。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-181">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="6a7b5-182">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="6a7b5-182">dnsSuffixList</span></span>|<span data-ttu-id="6a7b5-183">String 集合</span><span class="sxs-lookup"><span data-stu-id="6a7b5-183">String collection</span></span>|<span data-ttu-id="6a7b5-184">当前网络的有效 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-184">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="6a7b5-185">例如 seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="6a7b5-185">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="6a7b5-186">响应</span><span class="sxs-lookup"><span data-stu-id="6a7b5-186">Response</span></span>
<span data-ttu-id="6a7b5-187">如果成功，此方法在响应`201 Created`正文中返回响应代码和[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-187">If successful, this method returns a `201 Created` response code and a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6a7b5-188">示例</span><span class="sxs-lookup"><span data-stu-id="6a7b5-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="6a7b5-189">请求</span><span class="sxs-lookup"><span data-stu-id="6a7b5-189">Request</span></span>
<span data-ttu-id="6a7b5-190">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-190">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 483

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="6a7b5-191">响应</span><span class="sxs-lookup"><span data-stu-id="6a7b5-191">Response</span></span>
<span data-ttu-id="6a7b5-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="6a7b5-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 651

{
  "@odata.type": "#microsoft.graph.networkIPv6ConfigurationManagementCondition",
  "id": "25811206-1206-2581-0612-812506128125",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV6Prefix": "Ip V6Prefix value",
  "ipV6Gateway": "Ip V6Gateway value",
  "ipV6DNSServerList": [
    "Ip V6DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```





