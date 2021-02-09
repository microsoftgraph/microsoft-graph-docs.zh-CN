---
title: 创建 cloudPcOnPremisesConnection
description: 创建本地连接以预配云电脑。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 22f2e0f4b66742322f3ff6b1f18a50092fdf4895
ms.sourcegitcommit: eb31a6b4a582a59b44df3453450a82fd366342d0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/09/2021
ms.locfileid: "50162074"
---
# <a name="create-cloudpconpremisesconnection"></a><span data-ttu-id="3460b-103">创建 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="3460b-103">Create cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="3460b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3460b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3460b-105">创建新的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象，用于预配云电脑。</span><span class="sxs-lookup"><span data-stu-id="3460b-105">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object for provisioning cloud PCs.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="3460b-106">权限</span><span class="sxs-lookup"><span data-stu-id="3460b-106">Permissions</span></span>

<span data-ttu-id="3460b-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="3460b-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3460b-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="3460b-109">Permission type</span></span>|<span data-ttu-id="3460b-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="3460b-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3460b-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="3460b-111">Delegated (work or school account)</span></span>|<span data-ttu-id="3460b-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3460b-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="3460b-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="3460b-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3460b-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="3460b-114">Not supported.</span></span>|
|<span data-ttu-id="3460b-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="3460b-115">Application</span></span>|<span data-ttu-id="3460b-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="3460b-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3460b-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="3460b-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections
```

## <a name="request-headers"></a><span data-ttu-id="3460b-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="3460b-118">Request headers</span></span>

| <span data-ttu-id="3460b-119">名称</span><span class="sxs-lookup"><span data-stu-id="3460b-119">Name</span></span>          | <span data-ttu-id="3460b-120">说明</span><span class="sxs-lookup"><span data-stu-id="3460b-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="3460b-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="3460b-121">Authorization</span></span> | <span data-ttu-id="3460b-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="3460b-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="3460b-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="3460b-124">Content-Type</span></span>  | <span data-ttu-id="3460b-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="3460b-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="3460b-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="3460b-127">Request body</span></span>

<span data-ttu-id="3460b-128">在请求正文中，提供 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3460b-128">In the request body, supply a JSON representation of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="3460b-129">下表显示创建 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="3460b-129">The following table shows the properties that are required when you create the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

|<span data-ttu-id="3460b-130">属性</span><span class="sxs-lookup"><span data-stu-id="3460b-130">Property</span></span>|<span data-ttu-id="3460b-131">类型</span><span class="sxs-lookup"><span data-stu-id="3460b-131">Type</span></span>|<span data-ttu-id="3460b-132">说明</span><span class="sxs-lookup"><span data-stu-id="3460b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3460b-133">displayName</span><span class="sxs-lookup"><span data-stu-id="3460b-133">displayName</span></span>|<span data-ttu-id="3460b-134">String</span><span class="sxs-lookup"><span data-stu-id="3460b-134">String</span></span>|<span data-ttu-id="3460b-135">本地显示名称的基础结构。</span><span class="sxs-lookup"><span data-stu-id="3460b-135">The display name for the on-premises connection.</span></span>|
|<span data-ttu-id="3460b-136">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="3460b-136">subscriptionId</span></span>|<span data-ttu-id="3460b-137">String</span><span class="sxs-lookup"><span data-stu-id="3460b-137">String</span></span>|<span data-ttu-id="3460b-138">与租户关联的目标 Azure 订阅的 ID。</span><span class="sxs-lookup"><span data-stu-id="3460b-138">The ID of the target Azure subscription that’s associated with your tenant.</span></span>|
|<span data-ttu-id="3460b-139">adDomainName</span><span class="sxs-lookup"><span data-stu-id="3460b-139">adDomainName</span></span>|<span data-ttu-id="3460b-140">String</span><span class="sxs-lookup"><span data-stu-id="3460b-140">String</span></span>|<span data-ttu-id="3460b-141">要加入的 Active Directory (的 FQDN) 完全限定域名。</span><span class="sxs-lookup"><span data-stu-id="3460b-141">The fully qualified domain name (FQDN) of the Active Directory domain you want to join.</span></span>|
|<span data-ttu-id="3460b-142">adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="3460b-142">adDomainUsername</span></span>|<span data-ttu-id="3460b-143">String</span><span class="sxs-lookup"><span data-stu-id="3460b-143">String</span></span>|<span data-ttu-id="3460b-144">Active Directory 帐户的用户名 (拥有在 Active Directory) 创建计算机对象的权限的用户或服务帐户。</span><span class="sxs-lookup"><span data-stu-id="3460b-144">The username of an Active Directory account (user or service account) that has permissions to create computer objects in Active Directory.</span></span> <span data-ttu-id="3460b-145">所需格式：admin@contoso.com。</span><span class="sxs-lookup"><span data-stu-id="3460b-145">Required format: admin@contoso.com.</span></span>|
|<span data-ttu-id="3460b-146">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="3460b-146">adDomainPassword</span></span>|<span data-ttu-id="3460b-147">String</span><span class="sxs-lookup"><span data-stu-id="3460b-147">String</span></span>|<span data-ttu-id="3460b-148">与 adDomainUsername 关联的密码。</span><span class="sxs-lookup"><span data-stu-id="3460b-148">The password associated with adDomainUsername.</span></span>|
|<span data-ttu-id="3460b-149">resourceGroupId</span><span class="sxs-lookup"><span data-stu-id="3460b-149">resourceGroupId</span></span>|<span data-ttu-id="3460b-150">String</span><span class="sxs-lookup"><span data-stu-id="3460b-150">String</span></span>|<span data-ttu-id="3460b-151">目标资源组的 ID。</span><span class="sxs-lookup"><span data-stu-id="3460b-151">The ID of the target resource group.</span></span> <span data-ttu-id="3460b-152">必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}"。</span><span class="sxs-lookup"><span data-stu-id="3460b-152">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span></span>|
|<span data-ttu-id="3460b-153">virtualNetworkId</span><span class="sxs-lookup"><span data-stu-id="3460b-153">virtualNetworkId</span></span>|<span data-ttu-id="3460b-154">String</span><span class="sxs-lookup"><span data-stu-id="3460b-154">String</span></span>|<span data-ttu-id="3460b-155">目标虚拟网络的 ID。</span><span class="sxs-lookup"><span data-stu-id="3460b-155">The ID of the target virtual network.</span></span> <span data-ttu-id="3460b-156">必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}"。</span><span class="sxs-lookup"><span data-stu-id="3460b-156">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span></span>|
|<span data-ttu-id="3460b-157">subnetId</span><span class="sxs-lookup"><span data-stu-id="3460b-157">subnetId</span></span>|<span data-ttu-id="3460b-158">String</span><span class="sxs-lookup"><span data-stu-id="3460b-158">String</span></span>|<span data-ttu-id="3460b-159">目标子网的 ID。</span><span class="sxs-lookup"><span data-stu-id="3460b-159">The ID of the target subnet.</span></span> <span data-ttu-id="3460b-160">必需格式："/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}"。</span><span class="sxs-lookup"><span data-stu-id="3460b-160">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span></span>|

## <a name="response"></a><span data-ttu-id="3460b-161">响应</span><span class="sxs-lookup"><span data-stu-id="3460b-161">Response</span></span>

<span data-ttu-id="3460b-162">如果成功，此方法在响应正文中返回响应代码和 `201 Created` [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="3460b-162">If successful, this method returns a `201 Created` response code and a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="3460b-163">示例</span><span class="sxs-lookup"><span data-stu-id="3460b-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="3460b-164">请求</span><span class="sxs-lookup"><span data-stu-id="3460b-164">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="3460b-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="3460b-165">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_cloudpconpremisesconnection_from_cloudpconpremisesconnection"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/onPremisesConnections
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
# <a name="c"></a>[<span data-ttu-id="3460b-166">C#</span><span class="sxs-lookup"><span data-stu-id="3460b-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="3460b-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="3460b-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="3460b-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="3460b-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="3460b-169">Java</span><span class="sxs-lookup"><span data-stu-id="3460b-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="3460b-170">响应</span><span class="sxs-lookup"><span data-stu-id="3460b-170">Response</span></span>

<span data-ttu-id="3460b-171">**注意：** 下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="3460b-171">**Note:** Here is an example of the response.</span></span> <span data-ttu-id="3460b-172">为简洁起见，可能会截断此处所示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="3460b-172">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="3460b-173">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="3460b-173">All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcOnPremisesConnection"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 897

{
  "@odata.type": "#microsoft.graph.cloudPcOnPremisesConnection",
  "id": "ac2ad805-167e-49ee-9bef-196c4ce7ffff",
  "displayName": "Display Name value",
  "subscriptionId": "0ac520ee-14c0-480f-b6c9-0a90c585ffff",
  "subscriptionName": "Subscription Name value",
  "adDomainName": "Active Directory Domain Name value",
  "adDomainUsername": "Active Directory Domain User Name value",
  "organizationalUnit": "Organization Unit value",
  "resourceGroupId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG",
  "virtualNetworkId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c58ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet",
  "subnetId": "/subscriptions/0ac520ee-14c0-480f-b6c9-0a90c585ffff/resourceGroups/ExampleRG/providers/Microsoft.Network/virtualNetworks/ExampleVNet/subnets/default",
  "healthCheckStatus": "pending"
}
```
