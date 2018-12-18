---
title: 创建 networkIPv4ConfigurationManagementCondition
description: 创建新的 networkIPv4ConfigurationManagementCondition 对象。
author: tfitzmac
ms.openlocfilehash: 60d79584af38ca709d597b4919a7e6dc4171ff73
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27356362"
---
# <a name="create-networkipv4configurationmanagementcondition"></a><span data-ttu-id="fcf01-103">创建 networkIPv4ConfigurationManagementCondition</span><span class="sxs-lookup"><span data-stu-id="fcf01-103">Create networkIPv4ConfigurationManagementCondition</span></span>

> <span data-ttu-id="fcf01-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fcf01-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fcf01-105">在生产应用程序中不支持使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fcf01-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="fcf01-106">**注意：** 使用 Microsoft Graph API 配置 Intune 控件和策略仍需要客户[正确许可](https://go.microsoft.com/fwlink/?linkid=839381) Intune 服务。</span><span class="sxs-lookup"><span data-stu-id="fcf01-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="fcf01-107">创建新的[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fcf01-107">Create a new [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="fcf01-108">先决条件</span><span class="sxs-lookup"><span data-stu-id="fcf01-108">Prerequisites</span></span>
<span data-ttu-id="fcf01-p102">需要以下权限之一才能调用此 API。要了解包括如何选择权限的详细信息，请参阅[权限](/graph/permissions-reference)。
</span><span class="sxs-lookup"><span data-stu-id="fcf01-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fcf01-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="fcf01-111">Permission type</span></span>|<span data-ttu-id="fcf01-112">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fcf01-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fcf01-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fcf01-113">Delegated (work or school account)</span></span>|<span data-ttu-id="fcf01-114">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fcf01-114">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="fcf01-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fcf01-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fcf01-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="fcf01-116">Not supported.</span></span>|
|<span data-ttu-id="fcf01-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="fcf01-117">Application</span></span>|<span data-ttu-id="fcf01-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="fcf01-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fcf01-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fcf01-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/managementConditions
POST /deviceManagement/managementConditions/{managementConditionId}/managementConditionStatements/{managementConditionStatementId}/managementConditions
```

## <a name="request-headers"></a><span data-ttu-id="fcf01-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="fcf01-120">Request headers</span></span>
|<span data-ttu-id="fcf01-121">标头</span><span class="sxs-lookup"><span data-stu-id="fcf01-121">Header</span></span>|<span data-ttu-id="fcf01-122">值</span><span class="sxs-lookup"><span data-stu-id="fcf01-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="fcf01-123">授权</span><span class="sxs-lookup"><span data-stu-id="fcf01-123">Authorization</span></span>|<span data-ttu-id="fcf01-124">Bearer &lt;token&gt;。必需。</span><span class="sxs-lookup"><span data-stu-id="fcf01-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="fcf01-125">Accept</span><span class="sxs-lookup"><span data-stu-id="fcf01-125">Accept</span></span>|<span data-ttu-id="fcf01-126">application/json</span><span class="sxs-lookup"><span data-stu-id="fcf01-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="fcf01-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fcf01-127">Request body</span></span>
<span data-ttu-id="fcf01-128">在请求正文中，提供 networkIPv4ConfigurationManagementCondition 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fcf01-128">In the request body, supply a JSON representation for the networkIPv4ConfigurationManagementCondition object.</span></span>

<span data-ttu-id="fcf01-129">下表显示时创建 networkIPv4ConfigurationManagementCondition 所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fcf01-129">The following table shows the properties that are required when you create the networkIPv4ConfigurationManagementCondition.</span></span>

|<span data-ttu-id="fcf01-130">属性</span><span class="sxs-lookup"><span data-stu-id="fcf01-130">Property</span></span>|<span data-ttu-id="fcf01-131">类型</span><span class="sxs-lookup"><span data-stu-id="fcf01-131">Type</span></span>|<span data-ttu-id="fcf01-132">说明</span><span class="sxs-lookup"><span data-stu-id="fcf01-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fcf01-133">id</span><span class="sxs-lookup"><span data-stu-id="fcf01-133">id</span></span>|<span data-ttu-id="fcf01-134">字符串</span><span class="sxs-lookup"><span data-stu-id="fcf01-134">String</span></span>|<span data-ttu-id="fcf01-135">管理条件的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="fcf01-135">Unique identifier for the management condition.</span></span> <span data-ttu-id="fcf01-136">系统生成时创建分配值。</span><span class="sxs-lookup"><span data-stu-id="fcf01-136">System generated value assigned when created.</span></span> <span data-ttu-id="fcf01-137">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="fcf01-137">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="fcf01-138">唯一名称</span><span class="sxs-lookup"><span data-stu-id="fcf01-138">uniqueName</span></span>|<span data-ttu-id="fcf01-139">字符串</span><span class="sxs-lookup"><span data-stu-id="fcf01-139">String</span></span>|<span data-ttu-id="fcf01-140">管理条件的唯一名称。</span><span class="sxs-lookup"><span data-stu-id="fcf01-140">Unique name for the management condition.</span></span> <span data-ttu-id="fcf01-141">在管理条件表达式中使用。</span><span class="sxs-lookup"><span data-stu-id="fcf01-141">Used in management condition expressions.</span></span> <span data-ttu-id="fcf01-142">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="fcf01-142">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="fcf01-143">displayName</span><span class="sxs-lookup"><span data-stu-id="fcf01-143">displayName</span></span>|<span data-ttu-id="fcf01-144">字符串</span><span class="sxs-lookup"><span data-stu-id="fcf01-144">String</span></span>|<span data-ttu-id="fcf01-145">管理员定义管理条件的名称。</span><span class="sxs-lookup"><span data-stu-id="fcf01-145">The admin defined name of the management condition.</span></span> <span data-ttu-id="fcf01-146">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="fcf01-146">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="fcf01-147">说明</span><span class="sxs-lookup"><span data-stu-id="fcf01-147">description</span></span>|<span data-ttu-id="fcf01-148">字符串</span><span class="sxs-lookup"><span data-stu-id="fcf01-148">String</span></span>|<span data-ttu-id="fcf01-149">管理员定义的管理条件说明。</span><span class="sxs-lookup"><span data-stu-id="fcf01-149">The admin defined description of the management condition.</span></span> <span data-ttu-id="fcf01-150">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="fcf01-150">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="fcf01-151">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="fcf01-151">createdDateTime</span></span>|<span data-ttu-id="fcf01-152">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcf01-152">DateTimeOffset</span></span>|<span data-ttu-id="fcf01-153">创建管理条件的时间。</span><span class="sxs-lookup"><span data-stu-id="fcf01-153">The time the management condition was created.</span></span> <span data-ttu-id="fcf01-154">生成的服务方。</span><span class="sxs-lookup"><span data-stu-id="fcf01-154">Generated service side.</span></span> <span data-ttu-id="fcf01-155">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="fcf01-155">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="fcf01-156">modifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="fcf01-156">modifiedDateTime</span></span>|<span data-ttu-id="fcf01-157">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="fcf01-157">DateTimeOffset</span></span>|<span data-ttu-id="fcf01-158">管理条件上次修改时间。</span><span class="sxs-lookup"><span data-stu-id="fcf01-158">The time the management condition was last modified.</span></span> <span data-ttu-id="fcf01-159">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="fcf01-159">Updated service side.</span></span> <span data-ttu-id="fcf01-160">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="fcf01-160">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="fcf01-161">eTag</span><span class="sxs-lookup"><span data-stu-id="fcf01-161">eTag</span></span>|<span data-ttu-id="fcf01-162">String</span><span class="sxs-lookup"><span data-stu-id="fcf01-162">String</span></span>|<span data-ttu-id="fcf01-163">管理条件的 ETag。</span><span class="sxs-lookup"><span data-stu-id="fcf01-163">ETag of the management condition.</span></span> <span data-ttu-id="fcf01-164">更新服务端。</span><span class="sxs-lookup"><span data-stu-id="fcf01-164">Updated service side.</span></span> <span data-ttu-id="fcf01-165">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)</span><span class="sxs-lookup"><span data-stu-id="fcf01-165">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md)</span></span>|
|<span data-ttu-id="fcf01-166">applicablePlatforms</span><span class="sxs-lookup"><span data-stu-id="fcf01-166">applicablePlatforms</span></span>|<span data-ttu-id="fcf01-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md)集合</span><span class="sxs-lookup"><span data-stu-id="fcf01-167">[devicePlatformType](../resources/intune-shared-deviceplatformtype.md) collection</span></span>|<span data-ttu-id="fcf01-168">此管理条件适用的平台。</span><span class="sxs-lookup"><span data-stu-id="fcf01-168">The applicable platforms for this management condition.</span></span> <span data-ttu-id="fcf01-169">继承自[managementCondition](../resources/intune-fencing-managementcondition.md)。</span><span class="sxs-lookup"><span data-stu-id="fcf01-169">Inherited from [managementCondition](../resources/intune-fencing-managementcondition.md).</span></span> <span data-ttu-id="fcf01-170">可取值为：`android`、`androidForWork`、`iOS`、`macOS`、`windowsPhone81`、`windows81AndLater`、`windows10AndLater`、`androidWorkProfile`。</span><span class="sxs-lookup"><span data-stu-id="fcf01-170">Possible values are: `android`, `androidForWork`, `iOS`, `macOS`, `windowsPhone81`, `windows81AndLater`, `windows10AndLater`, `androidWorkProfile`.</span></span>|
|<span data-ttu-id="fcf01-171">ipV4Prefix</span><span class="sxs-lookup"><span data-stu-id="fcf01-171">ipV4Prefix</span></span>|<span data-ttu-id="fcf01-172">字符串</span><span class="sxs-lookup"><span data-stu-id="fcf01-172">String</span></span>|<span data-ttu-id="fcf01-173">要连接到的 IPv4 子网。</span><span class="sxs-lookup"><span data-stu-id="fcf01-173">The IPv4 subnet to be connected to.</span></span> <span data-ttu-id="fcf01-174">例如 10.0.0.0/8</span><span class="sxs-lookup"><span data-stu-id="fcf01-174">e.g. 10.0.0.0/8</span></span>|
|<span data-ttu-id="fcf01-175">ipV4Gateway</span><span class="sxs-lookup"><span data-stu-id="fcf01-175">ipV4Gateway</span></span>|<span data-ttu-id="fcf01-176">字符串</span><span class="sxs-lookup"><span data-stu-id="fcf01-176">String</span></span>|<span data-ttu-id="fcf01-177">IPv4 网关地址。</span><span class="sxs-lookup"><span data-stu-id="fcf01-177">The IPv4 gateway address.</span></span> <span data-ttu-id="fcf01-178">例如 10.0.0.0</span><span class="sxs-lookup"><span data-stu-id="fcf01-178">e.g. 10.0.0.0</span></span>|
|<span data-ttu-id="fcf01-179">ipV4DHCPServer</span><span class="sxs-lookup"><span data-stu-id="fcf01-179">ipV4DHCPServer</span></span>|<span data-ttu-id="fcf01-180">字符串</span><span class="sxs-lookup"><span data-stu-id="fcf01-180">String</span></span>|<span data-ttu-id="fcf01-181">为此适配器 DHCP 服务器的 IPv4 地址。</span><span class="sxs-lookup"><span data-stu-id="fcf01-181">The IPv4 address of the DHCP server for the adapter.</span></span>|
|<span data-ttu-id="fcf01-182">ipV4DNSServerList</span><span class="sxs-lookup"><span data-stu-id="fcf01-182">ipV4DNSServerList</span></span>|<span data-ttu-id="fcf01-183">String 集合</span><span class="sxs-lookup"><span data-stu-id="fcf01-183">String collection</span></span>|<span data-ttu-id="fcf01-184">配置为此适配器 IPv4 DNS 服务器。</span><span class="sxs-lookup"><span data-stu-id="fcf01-184">The IPv4 DNS servers configured for the adapter.</span></span>|
|<span data-ttu-id="fcf01-185">dnsSuffixList</span><span class="sxs-lookup"><span data-stu-id="fcf01-185">dnsSuffixList</span></span>|<span data-ttu-id="fcf01-186">String 集合</span><span class="sxs-lookup"><span data-stu-id="fcf01-186">String collection</span></span>|<span data-ttu-id="fcf01-187">当前网络的有效 DNS 后缀。</span><span class="sxs-lookup"><span data-stu-id="fcf01-187">Valid DNS suffixes for the current network.</span></span> <span data-ttu-id="fcf01-188">例如 seattle.contoso.com</span><span class="sxs-lookup"><span data-stu-id="fcf01-188">e.g. seattle.contoso.com</span></span>|



## <a name="response"></a><span data-ttu-id="fcf01-189">响应</span><span class="sxs-lookup"><span data-stu-id="fcf01-189">Response</span></span>
<span data-ttu-id="fcf01-190">如果成功，此方法返回`201 Created`响应代码和响应正文中的[networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md)对象。</span><span class="sxs-lookup"><span data-stu-id="fcf01-190">If successful, this method returns a `201 Created` response code and a [networkIPv4ConfigurationManagementCondition](../resources/intune-fencing-networkipv4configurationmanagementcondition.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fcf01-191">示例</span><span class="sxs-lookup"><span data-stu-id="fcf01-191">Example</span></span>
### <a name="request"></a><span data-ttu-id="fcf01-192">请求</span><span class="sxs-lookup"><span data-stu-id="fcf01-192">Request</span></span>
<span data-ttu-id="fcf01-193">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fcf01-193">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/managementConditions
Content-type: application/json
Content-length: 529

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```

### <a name="response"></a><span data-ttu-id="fcf01-194">响应</span><span class="sxs-lookup"><span data-stu-id="fcf01-194">Response</span></span>
<span data-ttu-id="fcf01-p114">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="fcf01-p114">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 697

{
  "@odata.type": "#microsoft.graph.networkIPv4ConfigurationManagementCondition",
  "id": "5e4a8284-8284-5e4a-8482-4a5e84824a5e",
  "uniqueName": "Unique Name value",
  "displayName": "Display Name value",
  "description": "Description value",
  "createdDateTime": "2017-01-01T00:02:43.5775965-08:00",
  "modifiedDateTime": "2017-01-01T00:00:22.8983556-08:00",
  "eTag": "ETag value",
  "applicablePlatforms": [
    "androidForWork"
  ],
  "ipV4Prefix": "Ip V4Prefix value",
  "ipV4Gateway": "Ip V4Gateway value",
  "ipV4DHCPServer": "Ip V4DHCPServer value",
  "ipV4DNSServerList": [
    "Ip V4DNSServer List value"
  ],
  "dnsSuffixList": [
    "Dns Suffix List value"
  ]
}
```





