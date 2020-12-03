---
title: 创建 cloudPcOnPremisesConnection
description: 创建本地连接以设置云电脑。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 0cbdbd6cb135e6adecf110ed6d18d03f9dfa5dd9
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563463"
---
# <a name="create-cloudpconpremisesconnection"></a><span data-ttu-id="f239e-103">创建 cloudPcOnPremisesConnection</span><span class="sxs-lookup"><span data-stu-id="f239e-103">Create cloudPcOnPremisesConnection</span></span>

<span data-ttu-id="f239e-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f239e-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f239e-105">创建新的 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象，用于设置云电脑。</span><span class="sxs-lookup"><span data-stu-id="f239e-105">Create a new [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object for provisioning cloud PCs.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="f239e-106">权限</span><span class="sxs-lookup"><span data-stu-id="f239e-106">Permissions</span></span>

<span data-ttu-id="f239e-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f239e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f239e-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="f239e-109">Permission type</span></span>|<span data-ttu-id="f239e-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="f239e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f239e-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f239e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="f239e-112">CloudPC</span><span class="sxs-lookup"><span data-stu-id="f239e-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="f239e-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f239e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f239e-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="f239e-114">Not supported.</span></span>|
|<span data-ttu-id="f239e-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="f239e-115">Application</span></span>|<span data-ttu-id="f239e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="f239e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f239e-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f239e-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/onPremisesConnections
```

## <a name="request-headers"></a><span data-ttu-id="f239e-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="f239e-118">Request headers</span></span>

| <span data-ttu-id="f239e-119">名称</span><span class="sxs-lookup"><span data-stu-id="f239e-119">Name</span></span>          | <span data-ttu-id="f239e-120">说明</span><span class="sxs-lookup"><span data-stu-id="f239e-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="f239e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="f239e-121">Authorization</span></span> | <span data-ttu-id="f239e-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f239e-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="f239e-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f239e-124">Content-Type</span></span>  | <span data-ttu-id="f239e-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f239e-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f239e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="f239e-127">Request body</span></span>

<span data-ttu-id="f239e-128">在请求正文中，提供 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f239e-128">In the request body, supply a JSON representation of the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object.</span></span>

<span data-ttu-id="f239e-129">下表显示创建 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="f239e-129">The following table shows the properties that are required when you create the [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md).</span></span>

|<span data-ttu-id="f239e-130">属性</span><span class="sxs-lookup"><span data-stu-id="f239e-130">Property</span></span>|<span data-ttu-id="f239e-131">类型</span><span class="sxs-lookup"><span data-stu-id="f239e-131">Type</span></span>|<span data-ttu-id="f239e-132">说明</span><span class="sxs-lookup"><span data-stu-id="f239e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f239e-133">displayName</span><span class="sxs-lookup"><span data-stu-id="f239e-133">displayName</span></span>|<span data-ttu-id="f239e-134">String</span><span class="sxs-lookup"><span data-stu-id="f239e-134">String</span></span>|<span data-ttu-id="f239e-135">本地连接的显示名称。</span><span class="sxs-lookup"><span data-stu-id="f239e-135">The display name for the on-premises connection.</span></span>|
|<span data-ttu-id="f239e-136">subscriptionId</span><span class="sxs-lookup"><span data-stu-id="f239e-136">subscriptionId</span></span>|<span data-ttu-id="f239e-137">String</span><span class="sxs-lookup"><span data-stu-id="f239e-137">String</span></span>|<span data-ttu-id="f239e-138">与你的租户关联的目标 Azure 订阅的 ID。</span><span class="sxs-lookup"><span data-stu-id="f239e-138">The ID of the target Azure subscription that’s associated with your tenant.</span></span>|
|<span data-ttu-id="f239e-139">adDomainName</span><span class="sxs-lookup"><span data-stu-id="f239e-139">adDomainName</span></span>|<span data-ttu-id="f239e-140">String</span><span class="sxs-lookup"><span data-stu-id="f239e-140">String</span></span>|<span data-ttu-id="f239e-141">要加入的 Active Directory 域 (FQDN) 的完全限定的域名称。</span><span class="sxs-lookup"><span data-stu-id="f239e-141">The fully qualified domain name (FQDN) of the Active Directory domain you want to join.</span></span>|
|<span data-ttu-id="f239e-142">adDomainUsername</span><span class="sxs-lookup"><span data-stu-id="f239e-142">adDomainUsername</span></span>|<span data-ttu-id="f239e-143">String</span><span class="sxs-lookup"><span data-stu-id="f239e-143">String</span></span>|<span data-ttu-id="f239e-144">Active Directory 帐户的用户名 (用户或服务帐户) 具有在 Active Directory 中创建计算机对象的权限。</span><span class="sxs-lookup"><span data-stu-id="f239e-144">The username of an Active Directory account (user or service account) that has permissions to create computer objects in Active Directory.</span></span> <span data-ttu-id="f239e-145">必需的格式： contoso@microsoft.com。</span><span class="sxs-lookup"><span data-stu-id="f239e-145">Required format: contoso@microsoft.com.</span></span>|
|<span data-ttu-id="f239e-146">adDomainPassword</span><span class="sxs-lookup"><span data-stu-id="f239e-146">adDomainPassword</span></span>|<span data-ttu-id="f239e-147">String</span><span class="sxs-lookup"><span data-stu-id="f239e-147">String</span></span>|<span data-ttu-id="f239e-148">与 adDomainUsername 相关联的密码。</span><span class="sxs-lookup"><span data-stu-id="f239e-148">The password associated with adDomainUsername.</span></span>|
|<span data-ttu-id="f239e-149">resourceGroupId</span><span class="sxs-lookup"><span data-stu-id="f239e-149">resourceGroupId</span></span>|<span data-ttu-id="f239e-150">String</span><span class="sxs-lookup"><span data-stu-id="f239e-150">String</span></span>|<span data-ttu-id="f239e-151">目标资源组的 ID。</span><span class="sxs-lookup"><span data-stu-id="f239e-151">The ID of the target resource group.</span></span> <span data-ttu-id="f239e-152">必需的格式： "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}"。</span><span class="sxs-lookup"><span data-stu-id="f239e-152">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}".</span></span>|
|<span data-ttu-id="f239e-153">virtualNetworkId</span><span class="sxs-lookup"><span data-stu-id="f239e-153">virtualNetworkId</span></span>|<span data-ttu-id="f239e-154">String</span><span class="sxs-lookup"><span data-stu-id="f239e-154">String</span></span>|<span data-ttu-id="f239e-155">目标虚拟网络的 ID。</span><span class="sxs-lookup"><span data-stu-id="f239e-155">The ID of the target virtual network.</span></span> <span data-ttu-id="f239e-156">必需的格式： "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}"。</span><span class="sxs-lookup"><span data-stu-id="f239e-156">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkName}".</span></span>|
|<span data-ttu-id="f239e-157">subnetId</span><span class="sxs-lookup"><span data-stu-id="f239e-157">subnetId</span></span>|<span data-ttu-id="f239e-158">String</span><span class="sxs-lookup"><span data-stu-id="f239e-158">String</span></span>|<span data-ttu-id="f239e-159">目标子网的 ID。</span><span class="sxs-lookup"><span data-stu-id="f239e-159">The ID of the target subnet.</span></span> <span data-ttu-id="f239e-160">必需的格式： "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}"。</span><span class="sxs-lookup"><span data-stu-id="f239e-160">Required format: "/subscriptions/{subscription-id}/resourceGroups/{resourceGroupName}/providers/Microsoft.Network/virtualNetworks/{virtualNetworkId}/subnets/{subnetName}".</span></span>|

## <a name="response"></a><span data-ttu-id="f239e-161">响应</span><span class="sxs-lookup"><span data-stu-id="f239e-161">Response</span></span>

<span data-ttu-id="f239e-162">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="f239e-162">If successful, this method returns a `201 Created` response code and a [cloudPcOnPremisesConnection](../resources/cloudpconpremisesconnection.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="f239e-163">示例</span><span class="sxs-lookup"><span data-stu-id="f239e-163">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f239e-164">请求</span><span class="sxs-lookup"><span data-stu-id="f239e-164">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="f239e-165">HTTP</span><span class="sxs-lookup"><span data-stu-id="f239e-165">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="f239e-166">C#</span><span class="sxs-lookup"><span data-stu-id="f239e-166">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f239e-167">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f239e-167">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f239e-168">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f239e-168">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f239e-169">Java</span><span class="sxs-lookup"><span data-stu-id="f239e-169">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpconpremisesconnection-from-cloudpconpremisesconnection-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="f239e-170">响应</span><span class="sxs-lookup"><span data-stu-id="f239e-170">Response</span></span>

<span data-ttu-id="f239e-171">**注意：** 下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="f239e-171">**Note:** Here is an example of the response.</span></span> <span data-ttu-id="f239e-172">为简洁起见，可能会截断此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="f239e-172">The response object shown here may be truncated for brevity.</span></span> <span data-ttu-id="f239e-173">将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="f239e-173">All of the properties will be returned from an actual call.</span></span>
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
  "healthCheckStatus": "pending",
  "inUse": false
}
```
