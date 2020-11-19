---
title: 更新 networkIPv6ConfigurationManagementCondition
description: 更新 networkIPv6ConfigurationManagementCondition 对象的属性。
author: dougeby
localization_priority: Normal
ms.prod: intune
doc_type: apiPageType
ms.openlocfilehash: e281a917e1193383aa41f29639e0d668939d0f57
ms.sourcegitcommit: eb536655ffd8d49ae258664f35c50a8263238400
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/18/2020
ms.locfileid: "49286155"
---
# <a name="update-networkipv6configurationmanagementcondition"></a><span data-ttu-id="518eb-103">更新 networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="518eb-103">Update networkIPv6ConfigurationManagementCondition</span></span>

<span data-ttu-id="518eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="518eb-104">Namespace: microsoft.graph</span></span>

> <span data-ttu-id="518eb-105">**重要说明：** /Beta 版本下的 Microsoft Graph Api 可能会发生更改;不支持生产使用。</span><span class="sxs-lookup"><span data-stu-id="518eb-105">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="518eb-106">**注意：** 适用于 Intune 的 Microsoft Graph API 需要适用于租户的 [活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="518eb-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="518eb-107">更新 [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="518eb-107">Update the properties of a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="518eb-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="518eb-108">Prerequisites</span></span>
<span data-ttu-id="518eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="518eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="518eb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="518eb-111">Permission type</span></span>|<span data-ttu-id="518eb-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="518eb-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="518eb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="518eb-113">Delegated (work or school account)</span></span>|<span data-ttu-id="518eb-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="518eb-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="518eb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="518eb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="518eb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="518eb-116">Not supported.</span></span>|
|<span data-ttu-id="518eb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="518eb-117">Application</span></span>|<span data-ttu-id="518eb-118">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="518eb-118">DeviceManagementConfiguration.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="518eb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="518eb-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/managementConditions/{managementConditionId}
PATCH /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions/{managementConditionId}
```

## <a name="request-headers"></a><span data-ttu-id="518eb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="518eb-120">Request headers</span></span>
|<span data-ttu-id="518eb-121">标头</span><span class="sxs-lookup"><span data-stu-id="518eb-121">Header</span></span>|<span data-ttu-id="518eb-122">值</span><span class="sxs-lookup"><span data-stu-id="518eb-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="518eb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="518eb-123">Authorization</span></span>|<span data-ttu-id="518eb-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="518eb-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="518eb-125">接受</span><span class="sxs-lookup"><span data-stu-id="518eb-125">Accept</span></span>|<span data-ttu-id="518eb-126">application/json</span><span class="sxs-lookup"><span data-stu-id="518eb-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="518eb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="518eb-127">Request body</span></span>
<span data-ttu-id="518eb-128">在请求正文中，提供 [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="518eb-128">In the request body, supply a JSON representation for the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

<span data-ttu-id="518eb-129">下表显示创建 [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="518eb-129">The following table shows the properties that are required when you create the [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md).</span></span>

|<span data-ttu-id="518eb-130">属性</span><span class="sxs-lookup"><span data-stu-id="518eb-130">Property</span></span>|<span data-ttu-id="518eb-131">类型</span><span class="sxs-lookup"><span data-stu-id="518eb-131">Type</span></span>|<span data-ttu-id="518eb-132">说明</span><span class="sxs-lookup"><span data-stu-id="518eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="518eb-133">id</span><span class="sxs-lookup"><span data-stu-id="518eb-133">id</span></span>|<span data-ttu-id="518eb-134">字符串</span><span class="sxs-lookup"><span data-stu-id="518eb-134">String</span></span>|<span data-ttu-id="518eb-135">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="518eb-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="518eb-136">创建时分配的系统生成值。</span><span class="sxs-lookup"><span data-stu-id="518eb-136">System generated value assigned when created.</span></span> <span data-ttu-id="518eb-137">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="518eb-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="518eb-138">uniqueName</span><span class="sxs-lookup"><span data-stu-id="518eb-138">uniqueName</span></span>|<span data-ttu-id="518eb-139">字符串</span><span class="sxs-lookup"><span data-stu-id="518eb-139">String</span></span>|<span data-ttu-id="518eb-140">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="518eb-140">Unique name for the management condition.</span></span> <span data-ttu-id="518eb-141">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="518eb-141">Used in management condition expressions.</span></span> <span data-ttu-id="518eb-142">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="518eb-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="518eb-143">displayName</span><span class="sxs-lookup"><span data-stu-id="518eb-143">displayName</span></span>|<span data-ttu-id="518eb-144">字符串</span><span class="sxs-lookup"><span data-stu-id="518eb-144">String</span></span>|<span data-ttu-id="518eb-145">管理条件的管理员定义名称。</span><span class="sxs-lookup"><span data-stu-id="518eb-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="518eb-146">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="518eb-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="518eb-147">description</span><span class="sxs-lookup"><span data-stu-id="518eb-147">description</span></span>|<span data-ttu-id="518eb-148">字符串</span><span class="sxs-lookup"><span data-stu-id="518eb-148">String</span></span>|<span data-ttu-id="518eb-149">管理条件的管理员定义的说明。</span><span class="sxs-lookup"><span data-stu-id="518eb-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="518eb-150">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="518eb-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="518eb-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="518eb-151">createdDateTime</span></span>|<span data-ttu-id="518eb-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="518eb-152">DateTimeOffset</span></span>|<span data-ttu-id="518eb-153">管理条件的创建时间。</span><span class="sxs-lookup"><span data-stu-id="518eb-153">The time the management condition was created.</span></span> <span data-ttu-id="518eb-154">生成的服务端。</span><span class="sxs-lookup"><span data-stu-id="518eb-154">Generated service side.</span></span> <span data-ttu-id="518eb-155">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="518eb-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="518eb-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="518eb-156">modifiedDateTime</span></span>|<span data-ttu-id="518eb-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="518eb-157">DateTimeOffset</span></span>|<span data-ttu-id="518eb-158">上次修改管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="518eb-158">The time the management condition was last modified.</span></span> <span data-ttu-id="518eb-159">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="518eb-159">Updated service side.</span></span> <span data-ttu-id="518eb-160">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="518eb-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="518eb-161">eTag</span><span class="sxs-lookup"><span data-stu-id="518eb-161">eTag</span></span>|<span data-ttu-id="518eb-162">String</span><span class="sxs-lookup"><span data-stu-id="518eb-162">String</span></span>|<span data-ttu-id="518eb-163">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="518eb-163">ETag of the management condition.</span></span> <span data-ttu-id="518eb-164">更新了服务端。</span><span class="sxs-lookup"><span data-stu-id="518eb-164">Updated service side.</span></span> <span data-ttu-id="518eb-165">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="518eb-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="518eb-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="518eb-166">applicablePlatforms</span></span>|<span data-ttu-id="518eb-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) 集合</span><span class="sxs-lookup"><span data-stu-id="518eb-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="518eb-168">适用于此管理条件的平台。</span><span class="sxs-lookup"><span data-stu-id="518eb-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="518eb-169">继承自 [managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="518eb-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="518eb-170">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`、`unknown`。</span><span class="sxs-lookup"><span data-stu-id="518eb-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`, `unknown`.</span></span>|
|<span data-ttu-id="518eb-171">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="518eb-171">ipV6Prefix</span></span>|<span data-ttu-id="518eb-172">字符串</span><span class="sxs-lookup"><span data-stu-id="518eb-172">String</span></span>|<span data-ttu-id="518eb-173">要连接到的 IPv6 子网。</span><span class="sxs-lookup"><span data-stu-id="518eb-173">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="518eb-174">例如2001： db8：：/32</span><span class="sxs-lookup"><span data-stu-id="518eb-174">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="518eb-175">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="518eb-175">ipV6Gateway</span></span>|<span data-ttu-id="518eb-176">字符串</span><span class="sxs-lookup"><span data-stu-id="518eb-176">String</span></span>|<span data-ttu-id="518eb-177">IPv6 网关地址。</span><span class="sxs-lookup"><span data-stu-id="518eb-177">The IPv6 gateway address to.</span></span> <span data-ttu-id="518eb-178">例如2001： db8：：1</span><span class="sxs-lookup"><span data-stu-id="518eb-178">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="518eb-179">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="518eb-179">ipV6DNSServerList</span></span>|<span data-ttu-id="518eb-180">String 集合</span><span class="sxs-lookup"><span data-stu-id="518eb-180">String collection</span></span>|<span data-ttu-id="518eb-181">为适配器配置的 IPv6 DNS 服务器。</span><span class="sxs-lookup"><span data-stu-id="518eb-181">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="518eb-182">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="518eb-182">dnsSuffixList</span></span>|<span data-ttu-id="518eb-183">String 集合</span><span class="sxs-lookup"><span data-stu-id="518eb-183">String collection</span></span>|<span data-ttu-id="518eb-184">当前网络的有效 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="518eb-184">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="518eb-185">例如 seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="518eb-185">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="518eb-186">响应</span><span class="sxs-lookup"><span data-stu-id="518eb-186">Response</span></span>
<span data-ttu-id="518eb-187">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="518eb-187">If successful, this method returns a `200 OK` response code and an updated [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="518eb-188">示例</span><span class="sxs-lookup"><span data-stu-id="518eb-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="518eb-189">请求</span><span class="sxs-lookup"><span data-stu-id="518eb-189">Request</span></span>
<span data-ttu-id="518eb-190">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="518eb-190">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/managementConditions/{managementConditionId}
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

### <a name="response"></a><span data-ttu-id="518eb-191">响应</span><span class="sxs-lookup"><span data-stu-id="518eb-191">Response</span></span>
<span data-ttu-id="518eb-p113">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="518eb-p113">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




