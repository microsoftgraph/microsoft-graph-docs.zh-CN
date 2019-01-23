---
title: 创建 networkIPv6ConfigurationManagementCondition
description: 创建新的 networkIPv6ConfigurationManagementCondition 对象。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 34db810cfcb62472a125d92487d6235b8f70d7ed
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/23/2019
ms.locfileid: "29411923"
---
# <a name="create-networkipv6configurationmanagementcondition"></a><span data-ttu-id="b0809-103">创建 networkIPv6ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="b0809-103">Create networkIPv6ConfigurationManagementCondition</span></span>

> <span data-ttu-id="b0809-104">**重要：** 在 Microsoft Graph 中的 /beta 版本下的 Api 可随时更改。</span><span class="sxs-lookup"><span data-stu-id="b0809-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="b0809-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b0809-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="b0809-106">**注意：** Intune Microsoft Graph API 要求租户[活动 Intune 许可证](https://go.microsoft.com/fwlink/?linkid=839381)。</span><span class="sxs-lookup"><span data-stu-id="b0809-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0809-107">创建新的[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b0809-107">Create a new [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="b0809-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="b0809-108">Prerequisites</span></span>
<span data-ttu-id="b0809-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/concepts/permissions-reference.md)。</span><span class="sxs-lookup"><span data-stu-id="b0809-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="b0809-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b0809-111">Permission type</span></span>|<span data-ttu-id="b0809-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="b0809-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="b0809-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b0809-113">Delegated (work or school account)</span></span>|<span data-ttu-id="b0809-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b0809-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="b0809-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b0809-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b0809-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0809-116">Not supported.</span></span>|
|<span data-ttu-id="b0809-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b0809-117">Application</span></span>|<span data-ttu-id="b0809-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b0809-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="b0809-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b0809-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="b0809-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b0809-120">Request headers</span></span>
|<span data-ttu-id="b0809-121">标头</span><span class="sxs-lookup"><span data-stu-id="b0809-121">Header</span></span>|<span data-ttu-id="b0809-122">值</span><span class="sxs-lookup"><span data-stu-id="b0809-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="b0809-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b0809-123">Authorization</span></span>|<span data-ttu-id="b0809-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="b0809-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="b0809-125">Accept</span><span class="sxs-lookup"><span data-stu-id="b0809-125">Accept</span></span>|<span data-ttu-id="b0809-126">application/json</span><span class="sxs-lookup"><span data-stu-id="b0809-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="b0809-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="b0809-127">Request body</span></span>
<span data-ttu-id="b0809-128">在请求正文中，提供 networkIPv6ConfigurationManagementCondition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b0809-128">In the request body, supply a JSON representation for the networkIPv6ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="b0809-129">下表显示时创建 networkIPv6ConfigurationManagementCondition 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="b0809-129">The following table shows the properties that are required when you create the networkIPv6ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="b0809-130">属性</span><span class="sxs-lookup"><span data-stu-id="b0809-130">Property</span></span>|<span data-ttu-id="b0809-131">类型</span><span class="sxs-lookup"><span data-stu-id="b0809-131">Type</span></span>|<span data-ttu-id="b0809-132">说明</span><span class="sxs-lookup"><span data-stu-id="b0809-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0809-133">id</span><span class="sxs-lookup"><span data-stu-id="b0809-133">id</span></span>|<span data-ttu-id="b0809-134">String</span><span class="sxs-lookup"><span data-stu-id="b0809-134">String</span></span>|<span data-ttu-id="b0809-135">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="b0809-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="b0809-136">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="b0809-136">System generated value assigned when created.</span></span> <span data-ttu-id="b0809-137">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b0809-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b0809-138">唯一名称</span><span class="sxs-lookup"><span data-stu-id="b0809-138">uniqueName</span></span>|<span data-ttu-id="b0809-139">String</span><span class="sxs-lookup"><span data-stu-id="b0809-139">String</span></span>|<span data-ttu-id="b0809-140">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="b0809-140">Unique name for the management condition.</span></span> <span data-ttu-id="b0809-141">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="b0809-141">Used in management condition expressions.</span></span> <span data-ttu-id="b0809-142">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b0809-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b0809-143">displayName</span><span class="sxs-lookup"><span data-stu-id="b0809-143">displayName</span></span>|<span data-ttu-id="b0809-144">String</span><span class="sxs-lookup"><span data-stu-id="b0809-144">String</span></span>|<span data-ttu-id="b0809-145">管理员定义管理条件的名称。</span><span class="sxs-lookup"><span data-stu-id="b0809-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="b0809-146">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b0809-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b0809-147">说明</span><span class="sxs-lookup"><span data-stu-id="b0809-147">description</span></span>|<span data-ttu-id="b0809-148">String</span><span class="sxs-lookup"><span data-stu-id="b0809-148">String</span></span>|<span data-ttu-id="b0809-149">管理员定义的管理条件说明。</span><span class="sxs-lookup"><span data-stu-id="b0809-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="b0809-150">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b0809-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b0809-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0809-151">createdDateTime</span></span>|<span data-ttu-id="b0809-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0809-152">DateTimeOffset</span></span>|<span data-ttu-id="b0809-153">创建管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="b0809-153">The time the management condition was created.</span></span> <span data-ttu-id="b0809-154">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="b0809-154">Generated service side.</span></span> <span data-ttu-id="b0809-155">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b0809-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b0809-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0809-156">modifiedDateTime</span></span>|<span data-ttu-id="b0809-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0809-157">DateTimeOffset</span></span>|<span data-ttu-id="b0809-158">管理条件上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="b0809-158">The time the management condition was last modified.</span></span> <span data-ttu-id="b0809-159">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="b0809-159">Updated service side.</span></span> <span data-ttu-id="b0809-160">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b0809-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b0809-161">eTag</span><span class="sxs-lookup"><span data-stu-id="b0809-161">eTag</span></span>|<span data-ttu-id="b0809-162">String</span><span class="sxs-lookup"><span data-stu-id="b0809-162">String</span></span>|<span data-ttu-id="b0809-163">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="b0809-163">ETag of the management condition.</span></span> <span data-ttu-id="b0809-164">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="b0809-164">Updated service side.</span></span> <span data-ttu-id="b0809-165">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="b0809-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="b0809-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="b0809-166">applicablePlatforms</span></span>|<span data-ttu-id="b0809-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="b0809-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="b0809-168">此管理条件适用的平台。</span><span class="sxs-lookup"><span data-stu-id="b0809-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="b0809-169">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="b0809-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="b0809-170">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="b0809-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="b0809-171">ipV6Prefix</span><span class="sxs-lookup"><span data-stu-id="b0809-171">ipV6Prefix</span></span>|<span data-ttu-id="b0809-172">String</span><span class="sxs-lookup"><span data-stu-id="b0809-172">String</span></span>|<span data-ttu-id="b0809-173">要连接到的 IPv6 子网。</span><span class="sxs-lookup"><span data-stu-id="b0809-173">The IPv6 subnet to be connected to.</span></span> <span data-ttu-id="b0809-174">例如 2001:db8:: / 32</span><span class="sxs-lookup"><span data-stu-id="b0809-174">e.g. 2001:db8::/32</span></span>|
|<span data-ttu-id="b0809-175">ipV6Gateway</span><span class="sxs-lookup"><span data-stu-id="b0809-175">ipV6Gateway</span></span>|<span data-ttu-id="b0809-176">String</span><span class="sxs-lookup"><span data-stu-id="b0809-176">String</span></span>|<span data-ttu-id="b0809-177">对 IPv6 网关地址。</span><span class="sxs-lookup"><span data-stu-id="b0809-177">The IPv6 gateway address to.</span></span> <span data-ttu-id="b0809-178">例如 2001:db8::1</span><span class="sxs-lookup"><span data-stu-id="b0809-178">e.g 2001:db8::1</span></span>|
|<span data-ttu-id="b0809-179">ipV6DNSServerList</span><span class="sxs-lookup"><span data-stu-id="b0809-179">ipV6DNSServerList</span></span>|<span data-ttu-id="b0809-180">String 集合</span><span class="sxs-lookup"><span data-stu-id="b0809-180">String collection</span></span>|<span data-ttu-id="b0809-181">为此适配器配置 IPv6 DNS 服务器。</span><span class="sxs-lookup"><span data-stu-id="b0809-181">An IPv6 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="b0809-182">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="b0809-182">dnsSuffixList</span></span>|<span data-ttu-id="b0809-183">String 集合</span><span class="sxs-lookup"><span data-stu-id="b0809-183">String collection</span></span>|<span data-ttu-id="b0809-184">当前网络的有效 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="b0809-184">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="b0809-185">例如 seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="b0809-185">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="b0809-186">响应</span><span class="sxs-lookup"><span data-stu-id="b0809-186">Response</span></span>
<span data-ttu-id="b0809-187">如果成功，此方法返回`201 Created`响应代码和响应正文中的[networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b0809-187">If successful, this method returns a `201 Created` response code and a [networkIPv6ConfigurationManagementCondition](../resources/intune-fencing-networkipv6configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b0809-188">示例</span><span class="sxs-lookup"><span data-stu-id="b0809-188">Example</span></span>

### <a name="request"></a><span data-ttu-id="b0809-189">请求</span><span class="sxs-lookup"><span data-stu-id="b0809-189">Request</span></span>
<span data-ttu-id="b0809-190">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="b0809-190">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="b0809-191">响应</span><span class="sxs-lookup"><span data-stu-id="b0809-191">Response</span></span>
<span data-ttu-id="b0809-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="b0809-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




