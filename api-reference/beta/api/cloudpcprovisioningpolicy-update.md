---
title: 更新 cloudPcProvisioningPolicy
description: 更新 cloudPcProvisioningPolicy 对象的属性。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: d33f0395dbcff1794a7171882a3bc152f731f1f8
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563308"
---
# <a name="update-cloudpcprovisioningpolicy"></a><span data-ttu-id="2ea78-103">更新 cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="2ea78-103">Update cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="2ea78-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ea78-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ea78-105">更新 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="2ea78-105">Update the properties of a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="2ea78-106">权限</span><span class="sxs-lookup"><span data-stu-id="2ea78-106">Permissions</span></span>

<span data-ttu-id="2ea78-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2ea78-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2ea78-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2ea78-109">Permission type</span></span>|<span data-ttu-id="2ea78-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="2ea78-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="2ea78-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2ea78-111">Delegated (work or school account)</span></span>|<span data-ttu-id="2ea78-112">CloudPC</span><span class="sxs-lookup"><span data-stu-id="2ea78-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="2ea78-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2ea78-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2ea78-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ea78-114">Not supported.</span></span>|
|<span data-ttu-id="2ea78-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2ea78-115">Application</span></span>|<span data-ttu-id="2ea78-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2ea78-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2ea78-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2ea78-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="2ea78-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2ea78-118">Request headers</span></span>

| <span data-ttu-id="2ea78-119">名称</span><span class="sxs-lookup"><span data-stu-id="2ea78-119">Name</span></span>          | <span data-ttu-id="2ea78-120">说明</span><span class="sxs-lookup"><span data-stu-id="2ea78-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="2ea78-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="2ea78-121">Authorization</span></span> | <span data-ttu-id="2ea78-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2ea78-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="2ea78-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="2ea78-124">Content-Type</span></span>  | <span data-ttu-id="2ea78-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="2ea78-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2ea78-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="2ea78-127">Request body</span></span>

<span data-ttu-id="2ea78-128">在请求正文中，提供 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ea78-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

<span data-ttu-id="2ea78-129">下表显示创建 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="2ea78-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).</span></span>

|<span data-ttu-id="2ea78-130">属性</span><span class="sxs-lookup"><span data-stu-id="2ea78-130">Property</span></span>|<span data-ttu-id="2ea78-131">类型</span><span class="sxs-lookup"><span data-stu-id="2ea78-131">Type</span></span>|<span data-ttu-id="2ea78-132">说明</span><span class="sxs-lookup"><span data-stu-id="2ea78-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2ea78-133">displayName</span><span class="sxs-lookup"><span data-stu-id="2ea78-133">displayName</span></span>|<span data-ttu-id="2ea78-134">String</span><span class="sxs-lookup"><span data-stu-id="2ea78-134">String</span></span>|<span data-ttu-id="2ea78-135">设置策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2ea78-135">The display name for the provisioning policy.</span></span> |
|<span data-ttu-id="2ea78-136">说明</span><span class="sxs-lookup"><span data-stu-id="2ea78-136">description</span></span>|<span data-ttu-id="2ea78-137">String</span><span class="sxs-lookup"><span data-stu-id="2ea78-137">String</span></span>|<span data-ttu-id="2ea78-138">设置策略说明。</span><span class="sxs-lookup"><span data-stu-id="2ea78-138">The provisioning policy description.</span></span>|
|<span data-ttu-id="2ea78-139">onPremisesConnectionId</span><span class="sxs-lookup"><span data-stu-id="2ea78-139">onPremisesConnectionId</span></span>|<span data-ttu-id="2ea78-140">String</span><span class="sxs-lookup"><span data-stu-id="2ea78-140">String</span></span>|<span data-ttu-id="2ea78-141">CloudPcOnPremisesConnection 的 ID。</span><span class="sxs-lookup"><span data-stu-id="2ea78-141">The ID of the cloudPcOnPremisesConnection.</span></span> <span data-ttu-id="2ea78-142">若要确保云电脑具有网络连接且它们加入域，请选择与云电脑服务验证的虚拟网络的连接。</span><span class="sxs-lookup"><span data-stu-id="2ea78-142">To ensure that cloud PCs have network connectivity and that they domain join, choose a connection with a virtual network that’s validated by the cloud PC service.</span></span>|
|<span data-ttu-id="2ea78-143">imageId</span><span class="sxs-lookup"><span data-stu-id="2ea78-143">imageId</span></span>|<span data-ttu-id="2ea78-144">String</span><span class="sxs-lookup"><span data-stu-id="2ea78-144">String</span></span>|<span data-ttu-id="2ea78-145">要在云电脑上预配的 OS 映像的 ID。</span><span class="sxs-lookup"><span data-stu-id="2ea78-145">The ID of the OS image you want to provision on cloud PCs.</span></span> <span data-ttu-id="2ea78-146">库类型图像的格式为： {publisher_offer_sku}。</span><span class="sxs-lookup"><span data-stu-id="2ea78-146">The format for a gallery type image is: {publisher_offer_sku}.</span></span>|
|<span data-ttu-id="2ea78-147">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="2ea78-147">imageDisplayName</span></span>|<span data-ttu-id="2ea78-148">String</span><span class="sxs-lookup"><span data-stu-id="2ea78-148">String</span></span>|<span data-ttu-id="2ea78-149">您正在设置的 OS 映像的显示名称。</span><span class="sxs-lookup"><span data-stu-id="2ea78-149">The display name for the OS image you’re provisioning.</span></span>|
|<span data-ttu-id="2ea78-150">imageType</span><span class="sxs-lookup"><span data-stu-id="2ea78-150">imageType</span></span>|<span data-ttu-id="2ea78-151">cloudPcProvisioningPolicyImageType</span><span class="sxs-lookup"><span data-stu-id="2ea78-151">cloudPcProvisioningPolicyImageType</span></span>|<span data-ttu-id="2ea78-152">要在云电脑上预配的 OS 映像 (自定义或库) 的类型。</span><span class="sxs-lookup"><span data-stu-id="2ea78-152">The type of OS image (custom or gallery) you want to provision on cloud PCs.</span></span> <span data-ttu-id="2ea78-153">可取值为：`gallery`、`custom`。</span><span class="sxs-lookup"><span data-stu-id="2ea78-153">Possible values are: `gallery`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="2ea78-154">响应</span><span class="sxs-lookup"><span data-stu-id="2ea78-154">Response</span></span>

<span data-ttu-id="2ea78-155">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="2ea78-155">If successful, this method returns a `200 OK` response code and an updated [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2ea78-156">示例</span><span class="sxs-lookup"><span data-stu-id="2ea78-156">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2ea78-157">请求</span><span class="sxs-lookup"><span data-stu-id="2ea78-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="2ea78-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="2ea78-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_provisioningpolicy"
}
-->

``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies/{id}
Content-Type: application/json
Content-length: 308

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
  "imageId": "Image ID value",
  "imageDisplayName": "Image Display Name value",
  "imageType": "custom"
}
```
# <a name="c"></a>[<span data-ttu-id="2ea78-159">C#</span><span class="sxs-lookup"><span data-stu-id="2ea78-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-provisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2ea78-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2ea78-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-provisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2ea78-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2ea78-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-provisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2ea78-162">Java</span><span class="sxs-lookup"><span data-stu-id="2ea78-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-provisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="2ea78-163">响应</span><span class="sxs-lookup"><span data-stu-id="2ea78-163">Response</span></span>

<span data-ttu-id="2ea78-164">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2ea78-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy"
}
-->

``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-length: 355

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "id": "8931f750-f750-8931-50f7-318950f7ffff",
  "displayName": "Display Name value",
  "description": "Description value",
  "onPremisesConnectionId": "4e47d0f6-6f77-44f0-8893-c0fe1701ffff",
  "imageId": "Image ID value",
  "imageDisplayName": "Image Display Name value",
  "imageType": "custom"
}
```
