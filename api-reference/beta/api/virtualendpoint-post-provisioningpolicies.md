---
title: 创建 cloudPcProvisioningPolicy
description: 创建新的云电脑预配策略。
author: AshleyYangSZ
localization_priority: Normal
ms.prod: cloud-pc
doc_type: apiPageType
ms.openlocfilehash: 45410405c88d7bb8a3e8de544e40279af490386a
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49563870"
---
# <a name="create-cloudpcprovisioningpolicy"></a><span data-ttu-id="c919a-103">创建 cloudPcProvisioningPolicy</span><span class="sxs-lookup"><span data-stu-id="c919a-103">Create cloudPcProvisioningPolicy</span></span>

<span data-ttu-id="c919a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c919a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c919a-105">创建新的 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c919a-105">Create a new [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

[!INCLUDE [cloudpc-api-preview](../../includes/cloudpc-api-preview.md)]

## <a name="permissions"></a><span data-ttu-id="c919a-106">权限</span><span class="sxs-lookup"><span data-stu-id="c919a-106">Permissions</span></span>

<span data-ttu-id="c919a-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c919a-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c919a-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c919a-109">Permission type</span></span>|<span data-ttu-id="c919a-110">权限（从最高特权到最低特权）</span><span class="sxs-lookup"><span data-stu-id="c919a-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="c919a-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c919a-111">Delegated (work or school account)</span></span>|<span data-ttu-id="c919a-112">CloudPC</span><span class="sxs-lookup"><span data-stu-id="c919a-112">CloudPC.ReadWrite.All</span></span>|
|<span data-ttu-id="c919a-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c919a-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c919a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c919a-114">Not supported.</span></span>|
|<span data-ttu-id="c919a-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c919a-115">Application</span></span>|<span data-ttu-id="c919a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c919a-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c919a-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c919a-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

``` http
POST /deviceManagement/virtualEndpoint/provisioningPolicies
```

## <a name="request-headers"></a><span data-ttu-id="c919a-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c919a-118">Request headers</span></span>

| <span data-ttu-id="c919a-119">名称</span><span class="sxs-lookup"><span data-stu-id="c919a-119">Name</span></span>          | <span data-ttu-id="c919a-120">说明</span><span class="sxs-lookup"><span data-stu-id="c919a-120">Description</span></span>                |
| :------------ | :------------------------  |
| <span data-ttu-id="c919a-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c919a-121">Authorization</span></span> | <span data-ttu-id="c919a-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c919a-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c919a-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="c919a-124">Content-Type</span></span>  | <span data-ttu-id="c919a-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c919a-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c919a-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c919a-127">Request body</span></span>

<span data-ttu-id="c919a-128">在请求正文中，提供 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c919a-128">In the request body, supply a JSON representation of the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object.</span></span>

<span data-ttu-id="c919a-129">下表显示创建 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="c919a-129">The following table shows the properties that are required when you create the [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md).</span></span>

|<span data-ttu-id="c919a-130">属性</span><span class="sxs-lookup"><span data-stu-id="c919a-130">Property</span></span>|<span data-ttu-id="c919a-131">类型</span><span class="sxs-lookup"><span data-stu-id="c919a-131">Type</span></span>|<span data-ttu-id="c919a-132">说明</span><span class="sxs-lookup"><span data-stu-id="c919a-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="c919a-133">displayName</span><span class="sxs-lookup"><span data-stu-id="c919a-133">displayName</span></span>|<span data-ttu-id="c919a-134">String</span><span class="sxs-lookup"><span data-stu-id="c919a-134">String</span></span>|<span data-ttu-id="c919a-135">设置策略的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c919a-135">The display name for the provisioning policy.</span></span>|
|<span data-ttu-id="c919a-136">说明</span><span class="sxs-lookup"><span data-stu-id="c919a-136">description</span></span>|<span data-ttu-id="c919a-137">String</span><span class="sxs-lookup"><span data-stu-id="c919a-137">String</span></span>|<span data-ttu-id="c919a-138">设置策略说明。</span><span class="sxs-lookup"><span data-stu-id="c919a-138">The provisioning policy description.</span></span>|
|<span data-ttu-id="c919a-139">onPremisesConnectionId</span><span class="sxs-lookup"><span data-stu-id="c919a-139">onPremisesConnectionId</span></span>|<span data-ttu-id="c919a-140">String</span><span class="sxs-lookup"><span data-stu-id="c919a-140">String</span></span>|<span data-ttu-id="c919a-141">CloudPcOnPremisesConnection 的 ID。</span><span class="sxs-lookup"><span data-stu-id="c919a-141">The ID of the cloudPcOnPremisesConnection.</span></span> <span data-ttu-id="c919a-142">若要确保云电脑具有网络连接且它们加入域，请选择与云电脑服务验证的虚拟网络的连接。</span><span class="sxs-lookup"><span data-stu-id="c919a-142">To ensure that cloud PCs have network connectivity and that they domain join, choose a connection with a virtual network that’s validated by the cloud PC service.</span></span>|
|<span data-ttu-id="c919a-143">imageId</span><span class="sxs-lookup"><span data-stu-id="c919a-143">imageId</span></span>|<span data-ttu-id="c919a-144">String</span><span class="sxs-lookup"><span data-stu-id="c919a-144">String</span></span>|<span data-ttu-id="c919a-145">要在云电脑上预配的 OS 映像的 ID。</span><span class="sxs-lookup"><span data-stu-id="c919a-145">The ID of the OS image you want to provision on cloud PCs.</span></span> <span data-ttu-id="c919a-146">库类型图像的格式为： {publisher_offer_sku}。</span><span class="sxs-lookup"><span data-stu-id="c919a-146">The format for a gallery type image is: {publisher_offer_sku}.</span></span>|
|<span data-ttu-id="c919a-147">imageDisplayName</span><span class="sxs-lookup"><span data-stu-id="c919a-147">imageDisplayName</span></span>|<span data-ttu-id="c919a-148">String</span><span class="sxs-lookup"><span data-stu-id="c919a-148">String</span></span>|<span data-ttu-id="c919a-149">您正在设置的 OS 映像的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c919a-149">The display name for the OS image you’re provisioning.</span></span>|
|<span data-ttu-id="c919a-150">imageType</span><span class="sxs-lookup"><span data-stu-id="c919a-150">imageType</span></span>|<span data-ttu-id="c919a-151">cloudPcProvisioningPolicyImageType</span><span class="sxs-lookup"><span data-stu-id="c919a-151">cloudPcProvisioningPolicyImageType</span></span>|<span data-ttu-id="c919a-152">要在云电脑上预配的 OS 映像 (自定义或库) 的类型。</span><span class="sxs-lookup"><span data-stu-id="c919a-152">The type of OS image (custom or gallery) you want to provision on cloud PCs.</span></span> <span data-ttu-id="c919a-153">可取值为：`gallery`、`custom`。</span><span class="sxs-lookup"><span data-stu-id="c919a-153">Possible values are: `gallery`, `custom`.</span></span>|

## <a name="response"></a><span data-ttu-id="c919a-154">响应</span><span class="sxs-lookup"><span data-stu-id="c919a-154">Response</span></span>

<span data-ttu-id="c919a-155">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c919a-155">If successful, this method returns a `201 Created` response code and a [cloudPcProvisioningPolicy](../resources/cloudpcprovisioningpolicy.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="c919a-156">示例</span><span class="sxs-lookup"><span data-stu-id="c919a-156">Examples</span></span>

### <a name="request"></a><span data-ttu-id="c919a-157">请求</span><span class="sxs-lookup"><span data-stu-id="c919a-157">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="c919a-158">HTTP</span><span class="sxs-lookup"><span data-stu-id="c919a-158">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_cloudpcprovisioningpolicy_from_cloudpcprovisioningpolicy"
}
-->

``` http
POST https://graph.microsoft.com/beta/deviceManagement/virtualEndpoint/provisioningPolicies
Content-Type: application/json
Content-length: 309

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "displayName": "Display Name value",
  "description": "Description value",
  "onPremisesConnectionId": "6bf90392-5fea-459a-9e9d-a2484abbffff",
  "imageId": "Image ID value",
  "imageDisplayName": "Image Display Name value",
  "imageType": "gallery"
}
```
# <a name="c"></a>[<span data-ttu-id="c919a-159">C#</span><span class="sxs-lookup"><span data-stu-id="c919a-159">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="c919a-160">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c919a-160">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="c919a-161">Objective-C</span><span class="sxs-lookup"><span data-stu-id="c919a-161">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="c919a-162">Java</span><span class="sxs-lookup"><span data-stu-id="c919a-162">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/create-cloudpcprovisioningpolicy-from-cloudpcprovisioningpolicy-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c919a-163">响应</span><span class="sxs-lookup"><span data-stu-id="c919a-163">Response</span></span>

<span data-ttu-id="c919a-164">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="c919a-164">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.cloudPcProvisioningPolicy"
}
-->

``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-length: 357

{
  "@odata.type": "#microsoft.graph.cloudPcProvisioningPolicy",
  "id": "1d164206-bf41-4fd2-8424-a3192d39ffff",
  "displayName": "Display Name value",
  "description": "Description value",
  "onPremisesConnectionId": "6bf90392-5fea-459a-9e9d-a2484abbffff",
  "imageId": "Image ID value",
  "imageDisplayName": "Image Display Name value",
  "imageType": "custom"
  }
```
