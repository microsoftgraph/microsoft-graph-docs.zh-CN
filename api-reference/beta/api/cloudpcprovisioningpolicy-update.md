---
title: 更新 cloudPcProvisioningPolicy
description: 更新 cloudPcProvisioningPolicy 对象的属性。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: b070f24cc91562626467aa3b4645e67fffd6d13c
ms.sourcegitcommit: eacd2a6e46c19dd3cd8519592b1668fabe14d85d
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/15/2021
ms.locfileid: "49872728"
---
# <a name="update-cloudpcprovisioningpolicy"></a><span data-ttu-id="70eed-103">更新 cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="70eed-103">Update cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="70eed-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="70eed-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70eed-105">更新 [cloudPcProvisioningPolicy 对象](../resources/cloudpcprovisioningpolicy.md) 的属性。</span><span class="sxs-lookup"><span data-stu-id="70eed-105">Update the properties of a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="70eed-106">权限</span><span class="sxs-lookup"><span data-stu-id="70eed-106">Permissions</span></span>

<span data-ttu-id="70eed-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70eed-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70eed-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="70eed-109">Permission type</span></span>|<span data-ttu-id="70eed-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70eed-110">Permissions (from least to most privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70eed-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70eed-111">Delegated (work or school account)</span></span>|<span data-ttu-id="70eed-112">CloudPC.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70eed-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="70eed-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70eed-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70eed-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="70eed-114">Not supported.</span></span>|
|<span data-ttu-id="70eed-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="70eed-115">Application</span></span>|<span data-ttu-id="70eed-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="70eed-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70eed-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70eed-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
PATCH /deviceManagement/virtualEndpoint/provisioningPolicies/{id}
```

## <a name="request-headers"></a><span data-ttu-id="70eed-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="70eed-118">Request headers</span></span>

| <span data-ttu-id="70eed-119">名称</span><span class="sxs-lookup"><span data-stu-id="70eed-119">Name</span></span>          | <span data-ttu-id="70eed-120">说明</span><span class="sxs-lookup"><span data-stu-id="70eed-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="70eed-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="70eed-121">Authorization</span></span> | <span data-ttu-id="70eed-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="70eed-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="70eed-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="70eed-124">Content-Type</span></span>  | <span data-ttu-id="70eed-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="70eed-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="70eed-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="70eed-127">Request body</span></span>

<span data-ttu-id="70eed-128">在请求正文中，提供 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70eed-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

<span data-ttu-id="70eed-129">下表显示创建 [cloudPcProvisioningPolicy 时所需的属性](../resources/cloudpcprovisioningpolicy.md)。</span><span class="sxs-lookup"><span data-stu-id="70eed-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).</span></span>

|<span data-ttu-id="70eed-130">属性</span><span class="sxs-lookup"><span data-stu-id="70eed-130">Property</span></span>|<span data-ttu-id="70eed-131">类型</span><span class="sxs-lookup"><span data-stu-id="70eed-131">Type</span></span>|<span data-ttu-id="70eed-132">说明</span><span class="sxs-lookup"><span data-stu-id="70eed-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70eed-133">displayName</span><span class="sxs-lookup"><span data-stu-id="70eed-133">displayName</span></span>|<span data-ttu-id="70eed-134">String</span><span class="sxs-lookup"><span data-stu-id="70eed-134">String</span></span>|<span data-ttu-id="70eed-135">设置显示名称策略的策略。</span><span class="sxs-lookup"><span data-stu-id="70eed-135">The display name for the provisioning policy.</span></span> |
|<span data-ttu-id="70eed-136">说明</span><span class="sxs-lookup"><span data-stu-id="70eed-136">description</span></span>|<span data-ttu-id="70eed-137">String</span><span class="sxs-lookup"><span data-stu-id="70eed-137">String</span></span>|<span data-ttu-id="70eed-138">设置策略说明。</span><span class="sxs-lookup"><span data-stu-id="70eed-138">The provisioning policy description.</span></span>|
|<span data-ttu-id="70eed-139">onPremisesConnectionId</span><span class="sxs-lookup"><span data-stu-id="70eed-139">onPremisesConnectionId</span></span>|<span data-ttu-id="70eed-140">String</span><span class="sxs-lookup"><span data-stu-id="70eed-140">String</span></span>|<span data-ttu-id="70eed-141">cloudPcOnPremisesConnection 的 ID。</span><span class="sxs-lookup"><span data-stu-id="70eed-141">The ID of the cloudPcOnPremisesConnection.</span></span> <span data-ttu-id="70eed-142">若要确保云电脑具有网络连接并且它们已加入域，请选择与由云电脑服务验证的虚拟网络的连接。</span><span class="sxs-lookup"><span data-stu-id="70eed-142">To ensure that cloud PCs have network connectivity and that they domain join, choose a connection with a virtual network that’s validated by the cloud PC service.</span></span>|
|<span data-ttu-id="70eed-143">imageId</span><span class="sxs-lookup"><span data-stu-id="70eed-143">imageId</span></span>|<span data-ttu-id="70eed-144">String</span><span class="sxs-lookup"><span data-stu-id="70eed-144">String</span></span>|<span data-ttu-id="70eed-145">你想要在云电脑中预配的操作系统映像的 ID。</span><span class="sxs-lookup"><span data-stu-id="70eed-145">The ID of the OS image you want to provision on cloud PCs.</span></span> <span data-ttu-id="70eed-146">库类型图像的格式为：{publisher_offer_sku}。</span><span class="sxs-lookup"><span data-stu-id="70eed-146">The format for a gallery type image is: {publisher_offer_sku}.</span></span>|
|<span data-ttu-id="70eed-147">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="70eed-147">imageDisplayName</span></span>|<span data-ttu-id="70eed-148">String</span><span class="sxs-lookup"><span data-stu-id="70eed-148">String</span></span>|<span data-ttu-id="70eed-149">用于显示名称操作系统映像的映像。</span><span class="sxs-lookup"><span data-stu-id="70eed-149">The display name for the OS image you’re provisioning.</span></span>|
|<span data-ttu-id="70eed-150">imageType</span><span class="sxs-lookup"><span data-stu-id="70eed-150">imageType</span></span>|<span data-ttu-id="70eed-151">cloudPcProvisioningPolicyImageType</span><span class="sxs-lookup"><span data-stu-id="70eed-151">cloudPcProvisioningPolicyImageType</span></span>|<span data-ttu-id="70eed-152">要预配 (自定义) 库的操作系统映像类型。</span><span class="sxs-lookup"><span data-stu-id="70eed-152">The type of OS image (custom or gallery) you want to provision on cloud PCs.</span></span> <span data-ttu-id="70eed-153">可取值为：`gallery`、`custom`。</span><span class="sxs-lookup"><span data-stu-id="70eed-153">Possible values are: `gallery`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="70eed-154">响应</span><span class="sxs-lookup"><span data-stu-id="70eed-154">Response</span></span>

<span data-ttu-id="70eed-155">如果成功，此方法在响应正文中返回响应代码和更新的 `200 OK` [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="70eed-155">If successful, this method returns a `200 OK` response code and an updated [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="70eed-156">示例</span><span class="sxs-lookup"><span data-stu-id="70eed-156">Examples</span></span>

### <a name="request"></a><span data-ttu-id="70eed-157">请求</span><span class="sxs-lookup"><span data-stu-id="70eed-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="70eed-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="70eed-158">HTTP</span></span>](#tab/http)
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
# <a name="c"></a>[<span data-ttu-id="70eed-159">C#</span><span class="sxs-lookup"><span data-stu-id="70eed-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-provisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="70eed-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="70eed-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-provisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="70eed-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="70eed-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-provisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="70eed-162">Java</span><span class="sxs-lookup"><span data-stu-id="70eed-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-provisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="70eed-163">响应</span><span class="sxs-lookup"><span data-stu-id="70eed-163">Response</span></span>

<span data-ttu-id="70eed-164">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="70eed-164">**Note:** The response object shown here might be shortened for readability.</span></span>
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
