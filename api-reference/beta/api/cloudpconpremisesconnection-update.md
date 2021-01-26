---
title: 更新 cloudPcOnPremisesConnection
description: 更新 cloudPcOnPremisesConnection 对象的属性。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 9c7f71249f47f9027afc8e7495e8d133a9f74885
ms.sourcegitcommit: 479b366f3265b666fdc024b0f90b8d29764bb4b2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/26/2021
ms.locfileid: "49981716"
---
# <a name="update-cloudpconpremisesconnection"></a><span data-ttu-id="1e9e2-103">更新 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="1e9e2-103">Update cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="1e9e2-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="1e9e2-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1e9e2-105">更新 [cloudPcOnPremisesConnection 对象](../resources/cloudpconpremisesconnection.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-105">Update the properties of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>
<span data-ttu-id="1e9e2-106">本地连接通过运行状况检查（由属性指示）后 `healthCheckStatus` ，将无法更新它。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-106">Once the on-premises connection passes health check, which is indicated by the `healthCheckStatus` property, you cannot update it.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="1e9e2-107">Permissions</span><span class="sxs-lookup"><span data-stu-id="1e9e2-107">Permissions</span></span>

<span data-ttu-id="1e9e2-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1e9e2-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1e9e2-110">Permission type</span></span>|<span data-ttu-id="1e9e2-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1e9e2-111">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1e9e2-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1e9e2-112">Delegated (work or school account)</span></span>|<span data-ttu-id="1e9e2-113">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1e9e2-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="1e9e2-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1e9e2-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1e9e2-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-115">Not supported.</span></span>|
|<span data-ttu-id="1e9e2-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="1e9e2-116">Application</span></span>|<span data-ttu-id="1e9e2-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1e9e2-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1e9e2-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="1e9e2-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="1e9e2-119">Request headers</span></span>

| <span data-ttu-id="1e9e2-120">名称</span><span class="sxs-lookup"><span data-stu-id="1e9e2-120">Name</span></span>          | <span data-ttu-id="1e9e2-121">说明</span><span class="sxs-lookup"><span data-stu-id="1e9e2-121">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="1e9e2-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="1e9e2-122">Authorization</span></span> | <span data-ttu-id="1e9e2-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="1e9e2-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="1e9e2-125">Content-Type</span></span>  | <span data-ttu-id="1e9e2-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="1e9e2-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="1e9e2-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1e9e2-128">Request body</span></span>

<span data-ttu-id="1e9e2-129">在请求正文中，提供 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-129">In the request body, supply a JSON representation of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="1e9e2-130">下表显示创建 [cloudPcOnPremisesConnection 时所需的属性](../resources/cloudpconpremisesconnection.md)。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-130">The following table shows the properties that are required when you create the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

|<span data-ttu-id="1e9e2-131">属性</span><span class="sxs-lookup"><span data-stu-id="1e9e2-131">Property</span></span>|<span data-ttu-id="1e9e2-132">类型</span><span class="sxs-lookup"><span data-stu-id="1e9e2-132">Type</span></span>|<span data-ttu-id="1e9e2-133">说明</span><span class="sxs-lookup"><span data-stu-id="1e9e2-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1e9e2-134">displayName</span><span class="sxs-lookup"><span data-stu-id="1e9e2-134">displayName</span></span>|<span data-ttu-id="1e9e2-135">String</span><span class="sxs-lookup"><span data-stu-id="1e9e2-135">String</span></span>|<span data-ttu-id="1e9e2-136">本地显示名称的基础结构。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-136">The display name for the on-premises connection.</span></span>|
|<span data-ttu-id="1e9e2-137">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="1e9e2-137">subscriptionId</span></span>|<span data-ttu-id="1e9e2-138">String</span><span class="sxs-lookup"><span data-stu-id="1e9e2-138">String</span></span>|<span data-ttu-id="1e9e2-139">与租户关联的目标 Azure 订阅的 ID。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-139">The ID of the target Azure subscription that’s associated with your tenant.</span></span>|
|<span data-ttu-id="1e9e2-140">adDomainName</span><span class="sxs-lookup"><span data-stu-id="1e9e2-140">adDomainName</span></span>|<span data-ttu-id="1e9e2-141">String</span><span class="sxs-lookup"><span data-stu-id="1e9e2-141">String</span></span>|<span data-ttu-id="1e9e2-142">要加入的 Active Directory (的 FQDN) 完全限定域名。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-142">The fully qualified domain name (FQDN) of the Active Directory domain you want to join.</span></span>|
|<span data-ttu-id="1e9e2-143">adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="1e9e2-143">adDomainUsername</span></span>|<span data-ttu-id="1e9e2-144">String</span><span class="sxs-lookup"><span data-stu-id="1e9e2-144">String</span></span>|<span data-ttu-id="1e9e2-145">Active Directory 帐户的用户名 (拥有在 Active Directory) 创建计算机对象的权限的用户或服务帐户。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-145">The username of an Active Directory account (user or service account) that has permissions to create computer objects in Active Directory.</span></span> <span data-ttu-id="1e9e2-146">所需格式：username@contoso.com。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-146">Required format: username@contoso.com.</span></span>|
|<span data-ttu-id="1e9e2-147">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="1e9e2-147">adDomainPassword</span></span>|<span data-ttu-id="1e9e2-148">String</span><span class="sxs-lookup"><span data-stu-id="1e9e2-148">String</span></span>|<span data-ttu-id="1e9e2-149">与 adDomainUsername 关联的密码。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-149">The password associated with adDomainUsername.</span></span>|
|<span data-ttu-id="1e9e2-150">resourceGroupId</span><span class="sxs-lookup"><span data-stu-id="1e9e2-150">resourceGroupId</span></span>|<span data-ttu-id="1e9e2-151">String</span><span class="sxs-lookup"><span data-stu-id="1e9e2-151">String</span></span>|<span data-ttu-id="1e9e2-152">目标资源组的 ID。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-152">The ID of the target resource group.</span></span> <span data-ttu-id="1e9e2-153">必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}"。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-153">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span></span>|
|<span data-ttu-id="1e9e2-154">virtualNetworkId</span><span class="sxs-lookup"><span data-stu-id="1e9e2-154">virtualNetworkId</span></span>|<span data-ttu-id="1e9e2-155">String</span><span class="sxs-lookup"><span data-stu-id="1e9e2-155">String</span></span>|<span data-ttu-id="1e9e2-156">目标虚拟网络的 ID。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-156">The ID of the target virtual network.</span></span> <span data-ttu-id="1e9e2-157">必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}"。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-157">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span></span>|
|<span data-ttu-id="1e9e2-158">subnetId</span><span class="sxs-lookup"><span data-stu-id="1e9e2-158">subnetId</span></span>|<span data-ttu-id="1e9e2-159">String</span><span class="sxs-lookup"><span data-stu-id="1e9e2-159">String</span></span>|<span data-ttu-id="1e9e2-160">目标子网的 ID。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-160">The ID of the target subnet.</span></span> <span data-ttu-id="1e9e2-161">必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}"。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-161">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span></span>|

## <a name="response"></a><span data-ttu-id="1e9e2-162">响应</span><span class="sxs-lookup"><span data-stu-id="1e9e2-162">Response</span></span>

<span data-ttu-id="1e9e2-163">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-163">If successful, this method returns a `200 OK` response code and an updated [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="1e9e2-164">示例</span><span class="sxs-lookup"><span data-stu-id="1e9e2-164">Examples</span></span>

### <a name="request"></a><span data-ttu-id="1e9e2-165">请求</span><span class="sxs-lookup"><span data-stu-id="1e9e2-165">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="1e9e2-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="1e9e2-166">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="1e9e2-167">C#</span><span class="sxs-lookup"><span data-stu-id="1e9e2-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisesconnections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="1e9e2-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="1e9e2-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisesconnections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="1e9e2-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="1e9e2-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisesconnections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="1e9e2-170">Java</span><span class="sxs-lookup"><span data-stu-id="1e9e2-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisesconnections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="1e9e2-171">响应</span><span class="sxs-lookup"><span data-stu-id="1e9e2-171">Response</span></span>

<span data-ttu-id="1e9e2-172">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="1e9e2-172">**Note:** The response object shown here might be shortened for readability.</span></span>

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
