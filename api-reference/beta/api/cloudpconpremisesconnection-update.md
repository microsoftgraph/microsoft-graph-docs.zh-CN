---
title: 更新 cloudPcOnPremisesConnection
description: 更新 cloudPcOnPremisesConnection 对象的属性。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: ''
doc_type: apiPageType
ms.openlocfilehash: b4f50441c46cc74dad5da08a3836aa471c158ad7
ms.sourcegitcommit: 3644a6cee51ab2bd19fa94e698d064073323d1dd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/21/2020
ms.locfileid: "49378273"
---
# <a name="update-cloudpconpremisesconnection"></a><span data-ttu-id="cb0a8-103">更新 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="cb0a8-103">Update cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="cb0a8-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="cb0a8-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="cb0a8-105">更新 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-105">Update the properties of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>
<span data-ttu-id="cb0a8-106">一旦本地连接通过属性指示的运行状况检查， `healthCheckStatus` 则无法更新它。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-106">Once the on-premises connection passes health check, which is indicated by the `healthCheckStatus` property, you cannot update it.</span></span>

## <a name="permissions"></a><span data-ttu-id="cb0a8-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="cb0a8-107">Permissions</span></span>

<span data-ttu-id="cb0a8-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="cb0a8-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="cb0a8-110">Permission type</span></span>|<span data-ttu-id="cb0a8-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="cb0a8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="cb0a8-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="cb0a8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="cb0a8-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="cb0a8-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="cb0a8-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="cb0a8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="cb0a8-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-115">Not supported.</span></span>|
|<span data-ttu-id="cb0a8-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="cb0a8-116">Application</span></span>|<span data-ttu-id="cb0a8-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="cb0a8-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="cb0a8-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="cb0a8-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="cb0a8-119">Request headers</span></span>

| <span data-ttu-id="cb0a8-120">名称</span><span class="sxs-lookup"><span data-stu-id="cb0a8-120">Name</span></span>          | <span data-ttu-id="cb0a8-121">说明</span><span class="sxs-lookup"><span data-stu-id="cb0a8-121">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="cb0a8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="cb0a8-122">Authorization</span></span> | <span data-ttu-id="cb0a8-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="cb0a8-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="cb0a8-125">Content-Type</span></span>  | <span data-ttu-id="cb0a8-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="cb0a8-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="cb0a8-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="cb0a8-128">Request body</span></span>

<span data-ttu-id="cb0a8-129">在请求正文中，提供 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-129">In the request body, supply a JSON representation of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="cb0a8-130">下表显示创建 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-130">The following table shows the properties that are required when you create the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

|<span data-ttu-id="cb0a8-131">属性</span><span class="sxs-lookup"><span data-stu-id="cb0a8-131">Property</span></span>|<span data-ttu-id="cb0a8-132">类型</span><span class="sxs-lookup"><span data-stu-id="cb0a8-132">Type</span></span>|<span data-ttu-id="cb0a8-133">说明</span><span class="sxs-lookup"><span data-stu-id="cb0a8-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="cb0a8-134">displayName</span><span class="sxs-lookup"><span data-stu-id="cb0a8-134">displayName</span></span>|<span data-ttu-id="cb0a8-135">字符串</span><span class="sxs-lookup"><span data-stu-id="cb0a8-135">String</span></span>|<span data-ttu-id="cb0a8-136">本地连接的显示名称。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-136">The display name for the on-premises connection.</span></span>|
|<span data-ttu-id="cb0a8-137">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="cb0a8-137">subscriptionId</span></span>|<span data-ttu-id="cb0a8-138">字符串</span><span class="sxs-lookup"><span data-stu-id="cb0a8-138">String</span></span>|<span data-ttu-id="cb0a8-139">与你的租户关联的目标 Azure 订阅的 ID。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-139">The ID of the target Azure subscription that’s associated with your tenant.</span></span>|
|<span data-ttu-id="cb0a8-140">adDomainName</span><span class="sxs-lookup"><span data-stu-id="cb0a8-140">adDomainName</span></span>|<span data-ttu-id="cb0a8-141">字符串</span><span class="sxs-lookup"><span data-stu-id="cb0a8-141">String</span></span>|<span data-ttu-id="cb0a8-142">要加入的 Active Directory 域 (FQDN) 的完全限定的域名称。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-142">The fully qualified domain name (FQDN) of the Active Directory domain you want to join.</span></span>|
|<span data-ttu-id="cb0a8-143">adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="cb0a8-143">adDomainUsername</span></span>|<span data-ttu-id="cb0a8-144">字符串</span><span class="sxs-lookup"><span data-stu-id="cb0a8-144">String</span></span>|<span data-ttu-id="cb0a8-145">Active Directory 帐户的用户名 (用户或服务帐户) 具有在 Active Directory 中创建计算机对象的权限。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-145">The username of an Active Directory account (user or service account) that has permissions to create computer objects in Active Directory.</span></span> <span data-ttu-id="cb0a8-146">必需的格式： contoso@microsoft.com。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-146">Required format: contoso@microsoft.com.</span></span>|
|<span data-ttu-id="cb0a8-147">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="cb0a8-147">adDomainPassword</span></span>|<span data-ttu-id="cb0a8-148">字符串</span><span class="sxs-lookup"><span data-stu-id="cb0a8-148">String</span></span>|<span data-ttu-id="cb0a8-149">与 adDomainUsername 相关联的密码。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-149">The password associated with adDomainUsername.</span></span>|
|<span data-ttu-id="cb0a8-150">resourceGroupId</span><span class="sxs-lookup"><span data-stu-id="cb0a8-150">resourceGroupId</span></span>|<span data-ttu-id="cb0a8-151">字符串</span><span class="sxs-lookup"><span data-stu-id="cb0a8-151">String</span></span>|<span data-ttu-id="cb0a8-152">目标资源组的 ID。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-152">The ID of the target resource group.</span></span> <span data-ttu-id="cb0a8-153">必需的格式： "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}"。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-153">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span></span>|
|<span data-ttu-id="cb0a8-154">virtualNetworkId</span><span class="sxs-lookup"><span data-stu-id="cb0a8-154">virtualNetworkId</span></span>|<span data-ttu-id="cb0a8-155">字符串</span><span class="sxs-lookup"><span data-stu-id="cb0a8-155">String</span></span>|<span data-ttu-id="cb0a8-156">目标虚拟网络的 ID。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-156">The ID of the target virtual network.</span></span> <span data-ttu-id="cb0a8-157">必需的格式： "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}"。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-157">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span></span>|
|<span data-ttu-id="cb0a8-158">subnetId</span><span class="sxs-lookup"><span data-stu-id="cb0a8-158">subnetId</span></span>|<span data-ttu-id="cb0a8-159">字符串</span><span class="sxs-lookup"><span data-stu-id="cb0a8-159">String</span></span>|<span data-ttu-id="cb0a8-160">目标子网的 ID。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-160">The ID of the target subnet.</span></span> <span data-ttu-id="cb0a8-161">必需的格式： "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}"。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-161">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span></span>|

## <a name="response"></a><span data-ttu-id="cb0a8-162">响应</span><span class="sxs-lookup"><span data-stu-id="cb0a8-162">Response</span></span>

<span data-ttu-id="cb0a8-163">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-163">If successful, this method returns a `200 OK` response code and an updated [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="cb0a8-164">示例</span><span class="sxs-lookup"><span data-stu-id="cb0a8-164">Examples</span></span>

### <a name="request"></a><span data-ttu-id="cb0a8-165">请求</span><span class="sxs-lookup"><span data-stu-id="cb0a8-165">Request</span></span>

<!-- {
  "blockType": "request",
  "name": "update_onpremisesconnections"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections/{id}
Content-Type: application/json
Content-length: 800

{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
  "displayName": "Display Name value",
  "subscriptionId": "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
  "subscriptionName": "Subscription Name value",
  "adDomainName": "Active Directory Domain Name value",
  "adDomainUsername": "Active Directory Domain User Name value",
  "organizationalUnit": "Organization Unit value",
  "resourceGroupId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG",
  "virtualNetworkId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet",
  "subnetId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default"
}
```

### <a name="response"></a><span data-ttu-id="cb0a8-166">响应</span><span class="sxs-lookup"><span data-stu-id="cb0a8-166">Response</span></span>

<span data-ttu-id="cb0a8-167">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="cb0a8-167">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnection"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 897

{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
  "id": "9ec90ff8-fd63-4fb9-ab5a-aa4fdcc4ffff",
  "displayName": "Display Name value",
  "subscriptionId": "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
  "subscriptionName": "Subscription Name value",
  "adDomainName": "Active Directory Domain Name value",
  "adDomainUsername": "Active Directory Domain User Name value",
  "organizationalUnit": "Organization Unit value",
  "resourceGroupId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG",
  "virtualNetworkId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet",
  "subnetId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default",
  "healthCheckStatus": "running",
  "inUse": false
}
```
