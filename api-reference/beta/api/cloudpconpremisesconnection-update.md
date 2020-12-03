---
title: 更新 cloudPcOnPremisesConnection
description: 更新 cloudPcOnPremisesConnection 对象的属性。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: ba7034305d6d8dcabea463e0f98f034947334ac8
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563266"
---
# <a name="update-cloudpconpremisesconnection"></a><span data-ttu-id="fb80b-103">更新 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="fb80b-103">Update cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="fb80b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fb80b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="fb80b-105">更新 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="fb80b-105">Update the properties of a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>
<span data-ttu-id="fb80b-106">一旦本地连接通过属性指示的运行状况检查， `healthCheckStatus` 则无法更新它。</span><span class="sxs-lookup"><span data-stu-id="fb80b-106">Once the on-premises connection passes health check, which is indicated by the `healthCheckStatus` property, you cannot update it.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="fb80b-107">权限</span><span class="sxs-lookup"><span data-stu-id="fb80b-107">Permissions</span></span>

<span data-ttu-id="fb80b-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fb80b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fb80b-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fb80b-110">Permission type</span></span>|<span data-ttu-id="fb80b-111">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="fb80b-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="fb80b-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fb80b-112">Delegated (work or school account)</span></span>|<span data-ttu-id="fb80b-113">CloudPC</span><span class="sxs-lookup"><span data-stu-id="fb80b-113">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="fb80b-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fb80b-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="fb80b-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb80b-115">Not supported.</span></span>|
|<span data-ttu-id="fb80b-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fb80b-116">Application</span></span>|<span data-ttu-id="fb80b-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="fb80b-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="fb80b-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fb80b-118">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /deviceManagement/virtualEndpoint/onPremisesConnections/{id}
```

## <a name="request-headers"></a><span data-ttu-id="fb80b-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fb80b-119">Request headers</span></span>

| <span data-ttu-id="fb80b-120">名称</span><span class="sxs-lookup"><span data-stu-id="fb80b-120">Name</span></span>          | <span data-ttu-id="fb80b-121">说明</span><span class="sxs-lookup"><span data-stu-id="fb80b-121">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="fb80b-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="fb80b-122">Authorization</span></span> | <span data-ttu-id="fb80b-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fb80b-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="fb80b-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="fb80b-125">Content-Type</span></span>  | <span data-ttu-id="fb80b-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="fb80b-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="fb80b-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="fb80b-128">Request body</span></span>

<span data-ttu-id="fb80b-129">在请求正文中，提供 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="fb80b-129">In the request body, supply a JSON representation of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="fb80b-130">下表显示创建 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="fb80b-130">The following table shows the properties that are required when you create the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

|<span data-ttu-id="fb80b-131">属性</span><span class="sxs-lookup"><span data-stu-id="fb80b-131">Property</span></span>|<span data-ttu-id="fb80b-132">类型</span><span class="sxs-lookup"><span data-stu-id="fb80b-132">Type</span></span>|<span data-ttu-id="fb80b-133">说明</span><span class="sxs-lookup"><span data-stu-id="fb80b-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="fb80b-134">displayName</span><span class="sxs-lookup"><span data-stu-id="fb80b-134">displayName</span></span>|<span data-ttu-id="fb80b-135">String</span><span class="sxs-lookup"><span data-stu-id="fb80b-135">String</span></span>|<span data-ttu-id="fb80b-136">本地连接的显示名称。</span><span class="sxs-lookup"><span data-stu-id="fb80b-136">The display name for the on-premises connection.</span></span>|
|<span data-ttu-id="fb80b-137">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="fb80b-137">subscriptionId</span></span>|<span data-ttu-id="fb80b-138">String</span><span class="sxs-lookup"><span data-stu-id="fb80b-138">String</span></span>|<span data-ttu-id="fb80b-139">与你的租户关联的目标 Azure 订阅的 ID。</span><span class="sxs-lookup"><span data-stu-id="fb80b-139">The ID of the target Azure subscription that’s associated with your tenant.</span></span>|
|<span data-ttu-id="fb80b-140">adDomainName</span><span class="sxs-lookup"><span data-stu-id="fb80b-140">adDomainName</span></span>|<span data-ttu-id="fb80b-141">String</span><span class="sxs-lookup"><span data-stu-id="fb80b-141">String</span></span>|<span data-ttu-id="fb80b-142">要加入的 Active Directory 域 (FQDN) 的完全限定的域名称。</span><span class="sxs-lookup"><span data-stu-id="fb80b-142">The fully qualified domain name (FQDN) of the Active Directory domain you want to join.</span></span>|
|<span data-ttu-id="fb80b-143">adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="fb80b-143">adDomainUsername</span></span>|<span data-ttu-id="fb80b-144">String</span><span class="sxs-lookup"><span data-stu-id="fb80b-144">String</span></span>|<span data-ttu-id="fb80b-145">Active Directory 帐户的用户名 (用户或服务帐户) 具有在 Active Directory 中创建计算机对象的权限。</span><span class="sxs-lookup"><span data-stu-id="fb80b-145">The username of an Active Directory account (user or service account) that has permissions to create computer objects in Active Directory.</span></span> <span data-ttu-id="fb80b-146">必需的格式： contoso@microsoft.com。</span><span class="sxs-lookup"><span data-stu-id="fb80b-146">Required format: contoso@microsoft.com.</span></span>|
|<span data-ttu-id="fb80b-147">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="fb80b-147">adDomainPassword</span></span>|<span data-ttu-id="fb80b-148">String</span><span class="sxs-lookup"><span data-stu-id="fb80b-148">String</span></span>|<span data-ttu-id="fb80b-149">与 adDomainUsername 相关联的密码。</span><span class="sxs-lookup"><span data-stu-id="fb80b-149">The password associated with adDomainUsername.</span></span>|
|<span data-ttu-id="fb80b-150">resourceGroupId</span><span class="sxs-lookup"><span data-stu-id="fb80b-150">resourceGroupId</span></span>|<span data-ttu-id="fb80b-151">String</span><span class="sxs-lookup"><span data-stu-id="fb80b-151">String</span></span>|<span data-ttu-id="fb80b-152">目标资源组的 ID。</span><span class="sxs-lookup"><span data-stu-id="fb80b-152">The ID of the target resource group.</span></span> <span data-ttu-id="fb80b-153">必需的格式： "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}"。</span><span class="sxs-lookup"><span data-stu-id="fb80b-153">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span></span>|
|<span data-ttu-id="fb80b-154">virtualNetworkId</span><span class="sxs-lookup"><span data-stu-id="fb80b-154">virtualNetworkId</span></span>|<span data-ttu-id="fb80b-155">String</span><span class="sxs-lookup"><span data-stu-id="fb80b-155">String</span></span>|<span data-ttu-id="fb80b-156">目标虚拟网络的 ID。</span><span class="sxs-lookup"><span data-stu-id="fb80b-156">The ID of the target virtual network.</span></span> <span data-ttu-id="fb80b-157">必需的格式： "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}"。</span><span class="sxs-lookup"><span data-stu-id="fb80b-157">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span></span>|
|<span data-ttu-id="fb80b-158">subnetId</span><span class="sxs-lookup"><span data-stu-id="fb80b-158">subnetId</span></span>|<span data-ttu-id="fb80b-159">String</span><span class="sxs-lookup"><span data-stu-id="fb80b-159">String</span></span>|<span data-ttu-id="fb80b-160">目标子网的 ID。</span><span class="sxs-lookup"><span data-stu-id="fb80b-160">The ID of the target subnet.</span></span> <span data-ttu-id="fb80b-161">必需的格式： "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}"。</span><span class="sxs-lookup"><span data-stu-id="fb80b-161">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span></span>|

## <a name="response"></a><span data-ttu-id="fb80b-162">响应</span><span class="sxs-lookup"><span data-stu-id="fb80b-162">Response</span></span>

<span data-ttu-id="fb80b-163">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fb80b-163">If successful, this method returns a `200 OK` response code and an updated [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="fb80b-164">示例</span><span class="sxs-lookup"><span data-stu-id="fb80b-164">Examples</span></span>

### <a name="request"></a><span data-ttu-id="fb80b-165">请求</span><span class="sxs-lookup"><span data-stu-id="fb80b-165">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="fb80b-166">HTTP</span><span class="sxs-lookup"><span data-stu-id="fb80b-166">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="fb80b-167">C#</span><span class="sxs-lookup"><span data-stu-id="fb80b-167">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-onpremisesconnections-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="fb80b-168">JavaScript</span><span class="sxs-lookup"><span data-stu-id="fb80b-168">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-onpremisesconnections-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="fb80b-169">Objective-C</span><span class="sxs-lookup"><span data-stu-id="fb80b-169">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-onpremisesconnections-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="fb80b-170">Java</span><span class="sxs-lookup"><span data-stu-id="fb80b-170">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-onpremisesconnections-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="fb80b-171">响应</span><span class="sxs-lookup"><span data-stu-id="fb80b-171">Response</span></span>

<span data-ttu-id="fb80b-172">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fb80b-172">**Note:** The response object shown here might be shortened for readability.</span></span>

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
