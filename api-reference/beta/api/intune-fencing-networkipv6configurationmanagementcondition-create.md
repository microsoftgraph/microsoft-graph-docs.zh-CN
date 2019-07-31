---
title: 创建 networkIPv6ConfigurationManagementCondition
description: 创建新的 networkIPv6ConfigurationManagementCondition 对象。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 454e80f66aaf1cc4421f719df522312b00df1be3
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "35990216"
---
# <a name="create-networkipv6configurationmanagementcondition"></a><span data-ttu-id="25c7f-103">创建 networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="25c7f-103">Create networkIPv6ConfigurationManagementCondition</span></span>

> <span data-ttu-id="25c7f-104">**重要说明:**/Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="25c7f-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="25c7f-105">**注意:** 适用于 Intune 的 Microsoft Graph API 需要租户的[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="25c7f-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="25c7f-106">创建新的[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="25c7f-106">Create a new [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="25c7f-107">先决条件</span><span class="sxs-lookup"><span data-stu-id="25c7f-107">Prerequisites</span></span>
<span data-ttu-id="25c7f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="25c7f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="25c7f-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="25c7f-110">Permission type</span></span>|<span data-ttu-id="25c7f-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="25c7f-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="25c7f-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="25c7f-112">Delegated (work or school account)</span></span>|<span data-ttu-id="25c7f-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="25c7f-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="25c7f-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="25c7f-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="25c7f-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="25c7f-115">Not supported.</span></span>|
|<span data-ttu-id="25c7f-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="25c7f-116">Application</span></span>|<span data-ttu-id="25c7f-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="25c7f-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="25c7f-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="25c7f-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="25c7f-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="25c7f-119">Request headers</span></span>
|<span data-ttu-id="25c7f-120">标头</span><span class="sxs-lookup"><span data-stu-id="25c7f-120">Header</span></span>|<span data-ttu-id="25c7f-121">值</span><span class="sxs-lookup"><span data-stu-id="25c7f-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="25c7f-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="25c7f-122">Authorization</span></span>|<span data-ttu-id="25c7f-123">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="25c7f-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="25c7f-124">接受</span><span class="sxs-lookup"><span data-stu-id="25c7f-124">Accept</span></span>|<span data-ttu-id="25c7f-125">application/json</span><span class="sxs-lookup"><span data-stu-id="25c7f-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="25c7f-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="25c7f-126">Request body</span></span>
<span data-ttu-id="25c7f-127">在请求正文中, 提供 networkIPv6ConfigurationManagementCondition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="25c7f-127">In the request body, supply a JSON representation for the networkIPv6ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="25c7f-128">下表显示创建 networkIPv6ConfigurationManagementCondition 时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="25c7f-128">The following table shows the properties that are required when you create the networkIPv6ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="25c7f-129">属性</span><span class="sxs-lookup"><span data-stu-id="25c7f-129">Property</span></span>|<span data-ttu-id="25c7f-130">类型</span><span class="sxs-lookup"><span data-stu-id="25c7f-130">Type</span></span>|<span data-ttu-id="25c7f-131">说明</span><span class="sxs-lookup"><span data-stu-id="25c7f-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="25c7f-132">id</span><span class="sxs-lookup"><span data-stu-id="25c7f-132">id</span></span>|<span data-ttu-id="25c7f-133">字符串</span><span class="sxs-lookup"><span data-stu-id="25c7f-133">String</span></span>|<span data-ttu-id="25c7f-134">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="25c7f-134">Unique identifier for the management condition.</span></span> <span data-ttu-id="25c7f-135">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="25c7f-135">System generated value assigned when created.</span></span> <span data-ttu-id="25c7f-136">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="25c7f-136">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="25c7f-137">uniqueName</span><span class="sxs-lookup"><span data-stu-id="25c7f-137">uniqueName</span></span>|<span data-ttu-id="25c7f-138">String</span><span class="sxs-lookup"><span data-stu-id="25c7f-138">String</span></span>|<span data-ttu-id="25c7f-139">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="25c7f-139">Unique name for the management condition.</span></span> <span data-ttu-id="25c7f-140">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="25c7f-140">Used in management condition expressions.</span></span> <span data-ttu-id="25c7f-141">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="25c7f-141">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="25c7f-142">displayName</span><span class="sxs-lookup"><span data-stu-id="25c7f-142">displayName</span></span>|<span data-ttu-id="25c7f-143">String</span><span class="sxs-lookup"><span data-stu-id="25c7f-143">String</span></span>|<span data-ttu-id="25c7f-144">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="25c7f-144">The admin defined name of the management condition.</span></span> <span data-ttu-id="25c7f-145">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="25c7f-145">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="25c7f-146">说明</span><span class="sxs-lookup"><span data-stu-id="25c7f-146">description</span></span>|<span data-ttu-id="25c7f-147">字符串</span><span class="sxs-lookup"><span data-stu-id="25c7f-147">String</span></span>|<span data-ttu-id="25c7f-148">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="25c7f-148">The admin defined description of the management condition.</span></span> <span data-ttu-id="25c7f-149">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="25c7f-149">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="25c7f-150">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="25c7f-150">createdDateTime</span></span>|<span data-ttu-id="25c7f-151">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25c7f-151">DateTimeOffset</span></span>|<span data-ttu-id="25c7f-152">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="25c7f-152">The time the management condition was created.</span></span> <span data-ttu-id="25c7f-153">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="25c7f-153">Generated service side.</span></span> <span data-ttu-id="25c7f-154">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="25c7f-154">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="25c7f-155">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="25c7f-155">modifiedDateTime</span></span>|<span data-ttu-id="25c7f-156">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="25c7f-156">DateTimeOffset</span></span>|<span data-ttu-id="25c7f-157">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="25c7f-157">The time the management condition was last modified.</span></span> <span data-ttu-id="25c7f-158">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="25c7f-158">Updated service side.</span></span> <span data-ttu-id="25c7f-159">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="25c7f-159">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="25c7f-160">eTag</span><span class="sxs-lookup"><span data-stu-id="25c7f-160">eTag</span></span>|<span data-ttu-id="25c7f-161">String</span><span class="sxs-lookup"><span data-stu-id="25c7f-161">String</span></span>|<span data-ttu-id="25c7f-162">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="25c7f-162">ETag of the management condition.</span></span> <span data-ttu-id="25c7f-163">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="25c7f-163">Updated service side.</span></span> <span data-ttu-id="25c7f-164">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="25c7f-164">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="25c7f-165">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="25c7f-165">applicablePlatforms</span></span>|<span data-ttu-id="25c7f-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="25c7f-166">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="25c7f-167">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="25c7f-167">The applicable platforms for this management condition.</span></span> <span data-ttu-id="25c7f-168">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="25c7f-168">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="25c7f-169">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="25c7f-169">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="25c7f-170">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="25c7f-170">ipV6Prefix</span></span>|<span data-ttu-id="25c7f-171">String</span><span class="sxs-lookup"><span data-stu-id="25c7f-171">String</span></span>|<span data-ttu-id="25c7f-172">要连接到的 IPv6 子网。</span><span class="sxs-lookup"><span data-stu-id="25c7f-172">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="25c7f-173">例如 2001: db8::/32</span><span class="sxs-lookup"><span data-stu-id="25c7f-173">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="25c7f-174">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="25c7f-174">ipV6Gateway</span></span>|<span data-ttu-id="25c7f-175">String</span><span class="sxs-lookup"><span data-stu-id="25c7f-175">String</span></span>|<span data-ttu-id="25c7f-176">IPv6 网关地址。</span><span class="sxs-lookup"><span data-stu-id="25c7f-176">The IPv6 gateway address to.</span></span> <span data-ttu-id="25c7f-177">例如 2001: db8:: 1</span><span class="sxs-lookup"><span data-stu-id="25c7f-177">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="25c7f-178">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="25c7f-178">ipV6DNSServerList</span></span>|<span data-ttu-id="25c7f-179">String collection</span><span class="sxs-lookup"><span data-stu-id="25c7f-179">String collection</span></span>|<span data-ttu-id="25c7f-180">为适配器配置的 IPv6 DNS 服务器。</span><span class="sxs-lookup"><span data-stu-id="25c7f-180">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="25c7f-181">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="25c7f-181">dnsSuffixList</span></span>|<span data-ttu-id="25c7f-182">String collection</span><span class="sxs-lookup"><span data-stu-id="25c7f-182">String collection</span></span>|<span data-ttu-id="25c7f-183">当前网络的有效 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="25c7f-183">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="25c7f-184">例如 seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="25c7f-184">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="25c7f-185">响应</span><span class="sxs-lookup"><span data-stu-id="25c7f-185">Response</span></span>
<span data-ttu-id="25c7f-186">如果成功, 此方法在响应`201 Created`正文中返回响应代码和[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="25c7f-186">If successful, this method returns a `201 Created` response code and a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="25c7f-187">示例</span><span class="sxs-lookup"><span data-stu-id="25c7f-187">Example</span></span>

### <a name="request"></a><span data-ttu-id="25c7f-188">请求</span><span class="sxs-lookup"><span data-stu-id="25c7f-188">Request</span></span>
<span data-ttu-id="25c7f-189">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="25c7f-189">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="25c7f-190">响应</span><span class="sxs-lookup"><span data-stu-id="25c7f-190">Response</span></span>
<span data-ttu-id="25c7f-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="25c7f-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





