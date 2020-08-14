---
title: 打印机：创建
description: 使用通用打印服务创建 (寄存器) 打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: bf100a99d573c186efa64af1692250534a31c50a
ms.sourcegitcommit: 5c3f4a3e2620d1d9e635e09231bbaa73cb0c3cdd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/14/2020
ms.locfileid: "46674090"
---
# <a name="printer-create"></a><span data-ttu-id="ac1c6-103">打印机：创建</span><span class="sxs-lookup"><span data-stu-id="ac1c6-103">printer: create</span></span>

<span data-ttu-id="ac1c6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ac1c6-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ac1c6-105">创建 (注册) 使用通用打印服务的打印机。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-105">Create (register) a printer with the Universal Print service.</span></span> <span data-ttu-id="ac1c6-106">这是一个长时间运行的操作，因此它返回可用于跟踪和验证打印机注册的 [printerCreateOperation](../resources/printercreateoperation.md) 。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-106">This is a long-running operation and as such, it returns a [printerCreateOperation](../resources/printercreateoperation.md) that can be used to track and verify the registration of the printer.</span></span>

## <a name="permissions"></a><span data-ttu-id="ac1c6-107">权限</span><span class="sxs-lookup"><span data-stu-id="ac1c6-107">Permissions</span></span>
<span data-ttu-id="ac1c6-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ac1c6-110">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-110">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="ac1c6-111">登录用户必须是 [打印机管理员](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-111">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="ac1c6-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="ac1c6-112">Permission type</span></span> | <span data-ttu-id="ac1c6-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ac1c6-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ac1c6-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ac1c6-114">Delegated (work or school account)</span></span>| <span data-ttu-id="ac1c6-115">"完全控制"、"全部"、"全打印机"</span><span class="sxs-lookup"><span data-stu-id="ac1c6-115">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="ac1c6-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ac1c6-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ac1c6-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-117">Not Supported.</span></span>|
|<span data-ttu-id="ac1c6-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="ac1c6-118">Application</span></span>| <span data-ttu-id="ac1c6-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-119">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="ac1c6-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ac1c6-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/create
```
## <a name="request-headers"></a><span data-ttu-id="ac1c6-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="ac1c6-121">Request headers</span></span>
| <span data-ttu-id="ac1c6-122">名称</span><span class="sxs-lookup"><span data-stu-id="ac1c6-122">Name</span></span>       | <span data-ttu-id="ac1c6-123">说明</span><span class="sxs-lookup"><span data-stu-id="ac1c6-123">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ac1c6-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="ac1c6-124">Authorization</span></span> | <span data-ttu-id="ac1c6-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ac1c6-127">Content-type</span><span class="sxs-lookup"><span data-stu-id="ac1c6-127">Content-type</span></span>  | <span data-ttu-id="ac1c6-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ac1c6-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ac1c6-130">请求正文</span><span class="sxs-lookup"><span data-stu-id="ac1c6-130">Request body</span></span>
<span data-ttu-id="ac1c6-131">在请求正文中，提供具有以下属性的 JSON 对象。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-131">In the request body, provide a JSON object with the following properties.</span></span>

| <span data-ttu-id="ac1c6-132">参数</span><span class="sxs-lookup"><span data-stu-id="ac1c6-132">Parameter</span></span>      | <span data-ttu-id="ac1c6-133">类型</span><span class="sxs-lookup"><span data-stu-id="ac1c6-133">Type</span></span>    |<span data-ttu-id="ac1c6-134">说明</span><span class="sxs-lookup"><span data-stu-id="ac1c6-134">Description</span></span>| <span data-ttu-id="ac1c6-135">是否必需？</span><span class="sxs-lookup"><span data-stu-id="ac1c6-135">Required?</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="ac1c6-136">displayName</span><span class="sxs-lookup"><span data-stu-id="ac1c6-136">displayName</span></span>|<span data-ttu-id="ac1c6-137">String</span><span class="sxs-lookup"><span data-stu-id="ac1c6-137">String</span></span>|<span data-ttu-id="ac1c6-138">要分配给打印机的显示名称。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-138">The display name to assign to the printer.</span></span>|<span data-ttu-id="ac1c6-139">是</span><span class="sxs-lookup"><span data-stu-id="ac1c6-139">Yes</span></span>|
|<span data-ttu-id="ac1c6-140">manufacturer</span><span class="sxs-lookup"><span data-stu-id="ac1c6-140">manufacturer</span></span>|<span data-ttu-id="ac1c6-141">String</span><span class="sxs-lookup"><span data-stu-id="ac1c6-141">String</span></span>|<span data-ttu-id="ac1c6-142">打印机的制造商。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-142">The manufacturer of the printer.</span></span>|<span data-ttu-id="ac1c6-143">是</span><span class="sxs-lookup"><span data-stu-id="ac1c6-143">Yes</span></span>|
|<span data-ttu-id="ac1c6-144">model</span><span class="sxs-lookup"><span data-stu-id="ac1c6-144">model</span></span>|<span data-ttu-id="ac1c6-145">String</span><span class="sxs-lookup"><span data-stu-id="ac1c6-145">String</span></span>|<span data-ttu-id="ac1c6-146">打印机的型号。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-146">The model of the printer.</span></span>|<span data-ttu-id="ac1c6-147">是</span><span class="sxs-lookup"><span data-stu-id="ac1c6-147">Yes</span></span>|
|<span data-ttu-id="ac1c6-148">physicalDeviceId</span><span class="sxs-lookup"><span data-stu-id="ac1c6-148">physicalDeviceId</span></span>|<span data-ttu-id="ac1c6-149">String</span><span class="sxs-lookup"><span data-stu-id="ac1c6-149">String</span></span>|<span data-ttu-id="ac1c6-150">打印机的物理设备 UUID。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-150">The physical device UUID of the printer.</span></span> <span data-ttu-id="ac1c6-151">如果属性为 true，则为必需 `hasPhysicalDevice` 。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-151">Required if the `hasPhysicalDevice` property is true.</span></span>|<span data-ttu-id="ac1c6-152">否</span><span class="sxs-lookup"><span data-stu-id="ac1c6-152">No</span></span>|
|<span data-ttu-id="ac1c6-153">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="ac1c6-153">hasPhysicalDevice</span></span>|<span data-ttu-id="ac1c6-154">布尔值</span><span class="sxs-lookup"><span data-stu-id="ac1c6-154">Boolean</span></span>|<span data-ttu-id="ac1c6-155">如果打印机具有物理输出设备，则为 True，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-155">True if the printer has physical output device, false otherwise.</span></span> <span data-ttu-id="ac1c6-156">如果省略，则默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-156">If omitted, the default value is true.</span></span>|<span data-ttu-id="ac1c6-157">否</span><span class="sxs-lookup"><span data-stu-id="ac1c6-157">No</span></span>|
|<span data-ttu-id="ac1c6-158">certificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="ac1c6-158">certificateSigningRequest</span></span>|[<span data-ttu-id="ac1c6-159">printCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="ac1c6-159">printCertificateSigningRequest</span></span>](../resources/printcertificatesigningrequest.md)|<span data-ttu-id="ac1c6-160">X.509 证书签名请求 (CSR) 为打印机创建并使用的证书来标识自己。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-160">The X.509 Certificate Signing Request (CSR) for the certificate created and used by the printer to identify itself.</span></span>|<span data-ttu-id="ac1c6-161">是</span><span class="sxs-lookup"><span data-stu-id="ac1c6-161">Yes</span></span>|
|<span data-ttu-id="ac1c6-162">connectorId</span><span class="sxs-lookup"><span data-stu-id="ac1c6-162">connectorId</span></span>|<span data-ttu-id="ac1c6-163">String</span><span class="sxs-lookup"><span data-stu-id="ac1c6-163">String</span></span>|<span data-ttu-id="ac1c6-164">充当打印机代理的连接器的 Id。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-164">Id of Connector acting as proxy to the printer.</span></span>|<span data-ttu-id="ac1c6-165">否</span><span class="sxs-lookup"><span data-stu-id="ac1c6-165">No</span></span>|

## <a name="response"></a><span data-ttu-id="ac1c6-166">响应</span><span class="sxs-lookup"><span data-stu-id="ac1c6-166">Response</span></span>
<span data-ttu-id="ac1c6-167">如果成功，此方法将 `202 Accepted` 在标头中返回响应代码和关联的 [printerCreateOperation](../resources/printercreateoperation.md) 的链接 `Operation-Location` 。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-167">If successful, this method returns a `202 Accepted` response code and a link to the associated [printerCreateOperation](../resources/printercreateoperation.md) in the `Operation-Location` header.</span></span>

<span data-ttu-id="ac1c6-168">向链接的 URL 发出 GET 请求可用于获取正在进行的打印机注册的状态。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-168">Making a GET request to the linked URL can be used to get the status of an ongoing printer registration.</span></span> <span data-ttu-id="ac1c6-169">成功完成打印机注册后，对链接的 URL 的 GET 请求将包含创建的打印机对象和已注册的证书。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-169">Once printer registration has completed successfully, a GET request to the linked URL will contain the created printer object and registered certificate.</span></span>

## <a name="example"></a><span data-ttu-id="ac1c6-170">示例</span><span class="sxs-lookup"><span data-stu-id="ac1c6-170">Example</span></span>
### <a name="request"></a><span data-ttu-id="ac1c6-171">请求</span><span class="sxs-lookup"><span data-stu-id="ac1c6-171">Request</span></span>
<span data-ttu-id="ac1c6-172">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-172">The following is an example of the request.</span></span> <span data-ttu-id="ac1c6-173">若要获取有关创建 (CSR) 所需的证书签名请求的帮助，请参阅 [CSR 生成代码示例](https://docs.microsoft.com/universal-print/hardware/universal-print-oem-certificate-signing-request)。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-173">For help creating the required Certificate Signing Request (CSR), see the [CSR generation code sample](https://docs.microsoft.com/universal-print/hardware/universal-print-oem-certificate-signing-request).</span></span>


# <a name="http"></a>[<span data-ttu-id="ac1c6-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="ac1c6-174">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="ac1c6-175">JavaScript</span><span class="sxs-lookup"><span data-stu-id="ac1c6-175">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="ac1c6-176">C#</span><span class="sxs-lookup"><span data-stu-id="ac1c6-176">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="ac1c6-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="ac1c6-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="ac1c6-178">响应</span><span class="sxs-lookup"><span data-stu-id="ac1c6-178">Response</span></span>
<span data-ttu-id="ac1c6-179">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ac1c6-179">The following is an example of the response.</span></span>

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
