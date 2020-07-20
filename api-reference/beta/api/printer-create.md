---
title: 打印机：创建
description: 创建（注册）具有通用打印服务的打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: a0b64166b6d7c95f3ad4995321b50b2c4aaadda9
ms.sourcegitcommit: 2050639c9e9a6b2dab9ce53d6a9fc87e98789b50
ms.translationtype: Auto
ms.contentlocale: zh-CN
ms.lasthandoff: 07/08/2020
ms.locfileid: "45081060"
---
# <a name="printer-create"></a><span data-ttu-id="c1a4c-103">打印机：创建</span><span class="sxs-lookup"><span data-stu-id="c1a4c-103">printer: create</span></span>

<span data-ttu-id="c1a4c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c1a4c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c1a4c-105">创建（注册）具有通用打印服务的打印机。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-105">Create (register) a printer with the Universal Print service.</span></span> <span data-ttu-id="c1a4c-106">这是一个长时间运行的操作，因此它返回可用于跟踪和验证打印机注册的[printerCreateOperation](../resources/printercreateoperation.md) 。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-106">This is a long-running operation and as such, it returns a [printerCreateOperation](../resources/printercreateoperation.md) that can be used to track and verify the registration of the printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="c1a4c-107">权限</span><span class="sxs-lookup"><span data-stu-id="c1a4c-107">Permissions</span></span>
<span data-ttu-id="c1a4c-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="c1a4c-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="c1a4c-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="c1a4c-111">Permission type</span></span> | <span data-ttu-id="c1a4c-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c1a4c-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="c1a4c-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c1a4c-113">Delegated (work or school account)</span></span>| <span data-ttu-id="c1a4c-114">User.Read.All</span><span class="sxs-lookup"><span data-stu-id="c1a4c-114">User.Read.All</span></span> |
|<span data-ttu-id="c1a4c-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c1a4c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="c1a4c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-116">Not Supported.</span></span>|
|<span data-ttu-id="c1a4c-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="c1a4c-117">Application</span></span>|<span data-ttu-id="c1a4c-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="c1a4c-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c1a4c-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/create
```
## <a name="request-headers"></a><span data-ttu-id="c1a4c-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="c1a4c-120">Request headers</span></span>
| <span data-ttu-id="c1a4c-121">名称</span><span class="sxs-lookup"><span data-stu-id="c1a4c-121">Name</span></span>       | <span data-ttu-id="c1a4c-122">说明</span><span class="sxs-lookup"><span data-stu-id="c1a4c-122">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="c1a4c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="c1a4c-123">Authorization</span></span> | <span data-ttu-id="c1a4c-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="c1a4c-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="c1a4c-126">Content-type</span></span>  | <span data-ttu-id="c1a4c-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c1a4c-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c1a4c-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="c1a4c-129">Request body</span></span>
<span data-ttu-id="c1a4c-130">在请求正文中，提供具有以下属性的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-130">In the request body, provide a JSON object with the following properties.</span></span>

| <span data-ttu-id="c1a4c-131">参数</span><span class="sxs-lookup"><span data-stu-id="c1a4c-131">Parameter</span></span>      | <span data-ttu-id="c1a4c-132">类型</span><span class="sxs-lookup"><span data-stu-id="c1a4c-132">Type</span></span>    |<span data-ttu-id="c1a4c-133">说明</span><span class="sxs-lookup"><span data-stu-id="c1a4c-133">Description</span></span>| <span data-ttu-id="c1a4c-134">是否必需？</span><span class="sxs-lookup"><span data-stu-id="c1a4c-134">Required?</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="c1a4c-135">displayName</span><span class="sxs-lookup"><span data-stu-id="c1a4c-135">displayName</span></span>|<span data-ttu-id="c1a4c-136">String</span><span class="sxs-lookup"><span data-stu-id="c1a4c-136">String</span></span>|<span data-ttu-id="c1a4c-137">要分配给打印机的显示名称。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-137">The display name to assign to the printer.</span></span>|<span data-ttu-id="c1a4c-138">是</span><span class="sxs-lookup"><span data-stu-id="c1a4c-138">Yes</span></span>|
|<span data-ttu-id="c1a4c-139">manufacturer</span><span class="sxs-lookup"><span data-stu-id="c1a4c-139">manufacturer</span></span>|<span data-ttu-id="c1a4c-140">String</span><span class="sxs-lookup"><span data-stu-id="c1a4c-140">String</span></span>|<span data-ttu-id="c1a4c-141">打印机的制造商。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-141">The manufacturer of the printer.</span></span>|<span data-ttu-id="c1a4c-142">是</span><span class="sxs-lookup"><span data-stu-id="c1a4c-142">Yes</span></span>|
|<span data-ttu-id="c1a4c-143">model</span><span class="sxs-lookup"><span data-stu-id="c1a4c-143">model</span></span>|<span data-ttu-id="c1a4c-144">String</span><span class="sxs-lookup"><span data-stu-id="c1a4c-144">String</span></span>|<span data-ttu-id="c1a4c-145">打印机的型号。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-145">The model of the printer.</span></span>|<span data-ttu-id="c1a4c-146">是</span><span class="sxs-lookup"><span data-stu-id="c1a4c-146">Yes</span></span>|
|<span data-ttu-id="c1a4c-147">physicalDeviceId</span><span class="sxs-lookup"><span data-stu-id="c1a4c-147">physicalDeviceId</span></span>|<span data-ttu-id="c1a4c-148">String</span><span class="sxs-lookup"><span data-stu-id="c1a4c-148">String</span></span>|<span data-ttu-id="c1a4c-149">打印机的物理设备 UUID。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-149">The physical device UUID of the printer.</span></span> <span data-ttu-id="c1a4c-150">如果属性为 true，则为必需 `hasPhysicalDevice` 。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-150">Required if the `hasPhysicalDevice` property is true.</span></span>|<span data-ttu-id="c1a4c-151">否</span><span class="sxs-lookup"><span data-stu-id="c1a4c-151">No</span></span>|
|<span data-ttu-id="c1a4c-152">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="c1a4c-152">hasPhysicalDevice</span></span>|<span data-ttu-id="c1a4c-153">Boolean</span><span class="sxs-lookup"><span data-stu-id="c1a4c-153">Boolean</span></span>|<span data-ttu-id="c1a4c-154">如果打印机具有物理输出设备，则为 True，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-154">True if the printer has physical output device, false otherwise.</span></span> <span data-ttu-id="c1a4c-155">如果省略，则默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-155">If omitted, the default value is true.</span></span>|<span data-ttu-id="c1a4c-156">否</span><span class="sxs-lookup"><span data-stu-id="c1a4c-156">No</span></span>|
|<span data-ttu-id="c1a4c-157">certificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="c1a4c-157">certificateSigningRequest</span></span>|[<span data-ttu-id="c1a4c-158">printCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="c1a4c-158">printCertificateSigningRequest</span></span>](../resources/printcertificatesigningrequest.md)|<span data-ttu-id="c1a4c-159">打印机创建并使用的证书的 x.509 证书签名请求（CSR），用于标识自己。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-159">The X.509 Certificate Signing Request (CSR) for the certificate created and used by the printer to identify itself.</span></span>|<span data-ttu-id="c1a4c-160">是</span><span class="sxs-lookup"><span data-stu-id="c1a4c-160">Yes</span></span>|
|<span data-ttu-id="c1a4c-161">connectorId</span><span class="sxs-lookup"><span data-stu-id="c1a4c-161">connectorId</span></span>|<span data-ttu-id="c1a4c-162">String</span><span class="sxs-lookup"><span data-stu-id="c1a4c-162">String</span></span>|<span data-ttu-id="c1a4c-163">充当打印机代理的连接器的 Id。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-163">Id of Connector acting as proxy to the printer.</span></span>|<span data-ttu-id="c1a4c-164">否</span><span class="sxs-lookup"><span data-stu-id="c1a4c-164">No</span></span>|

## <a name="response"></a><span data-ttu-id="c1a4c-165">响应</span><span class="sxs-lookup"><span data-stu-id="c1a4c-165">Response</span></span>
<span data-ttu-id="c1a4c-166">如果成功，此方法将 `202 Accepted` 在标头中返回响应代码和关联的[printerCreateOperation](../resources/printercreateoperation.md)的链接 `Operation-Location` 。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-166">If successful, this method returns a `202 Accepted` response code and a link to the associated [printerCreateOperation](../resources/printercreateoperation.md) in the `Operation-Location` header.</span></span>

<span data-ttu-id="c1a4c-167">向链接的 URL 发出 GET 请求可用于获取正在进行的打印机注册的状态。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-167">Making a GET request to the linked URL can be used to get the status of an ongoing printer registration.</span></span> <span data-ttu-id="c1a4c-168">成功完成打印机注册后，对链接的 URL 的 GET 请求将包含创建的打印机对象和已注册的证书。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-168">Once printer registration has completed successfully, a GET request to the linked URL will contain the created printer object and registered certificate.</span></span>

## <a name="example"></a><span data-ttu-id="c1a4c-169">示例</span><span class="sxs-lookup"><span data-stu-id="c1a4c-169">Example</span></span>
### <a name="request"></a><span data-ttu-id="c1a4c-170">请求</span><span class="sxs-lookup"><span data-stu-id="c1a4c-170">Request</span></span>
<span data-ttu-id="c1a4c-171">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-171">The following is an example of the request.</span></span> <span data-ttu-id="c1a4c-172">若要获取有关创建所需证书签名请求（CSR）的帮助，请参阅[CSR 生成代码示例](https://docs.microsoft.com/universal-print/hardware/universal-print-oem-certificate-signing-request)。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-172">For help creating the required Certificate Signing Request (CSR), see the [CSR generation code sample](https://docs.microsoft.com/universal-print/hardware/universal-print-oem-certificate-signing-request).</span></span>


# <a name="http"></a>[<span data-ttu-id="c1a4c-173">HTTP</span><span class="sxs-lookup"><span data-stu-id="c1a4c-173">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printer"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/create
Content-type: application/json
Content-length: 319

{
  "displayName": "Test Printer",
  "manufacturer": "Test Printer Manufacturer",
  "model": "Test Printer Model",
  "physicalDeviceId": null,
  "hasPhysicalDevice": false,
  "certificateSigningRequest": { 
    "content": "{content}",
    "transportKey": "{sampleTransportKey}"
  },
  "connectorId": null
}
```
# <a name="javascript"></a>[<span data-ttu-id="c1a4c-174">JavaScript</span><span class="sxs-lookup"><span data-stu-id="c1a4c-174">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="c1a4c-175">响应</span><span class="sxs-lookup"><span data-stu-id="c1a4c-175">Response</span></span>
<span data-ttu-id="c1a4c-176">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c1a4c-176">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 202 Accepted
Operation-Location: https://graph.microsoft.com/beta/print/operations/f221760a-52e8-4c11-b8c5-5dfaef3a49db
Retry-After: 5
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "printers: create",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
