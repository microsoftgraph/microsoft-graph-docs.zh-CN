---
title: printer： create
description: 创建 (通用) 在打印机上注册。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: bd07e04aa2a4c8b459e90a55d537c683a677d8e9
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50772042"
---
# <a name="printer-create"></a><span data-ttu-id="f2b79-103">printer： create</span><span class="sxs-lookup"><span data-stu-id="f2b79-103">printer: create</span></span>
<span data-ttu-id="f2b79-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f2b79-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="f2b79-105">创建 (通用) 在打印机上注册。</span><span class="sxs-lookup"><span data-stu-id="f2b79-105">Create (register) a printer with the Universal Print service.</span></span> <span data-ttu-id="f2b79-106">这是一个长时间运行的操作，因此它将返回一个 [printerCreateOperation，](../resources/printercreateoperation.md) 该打印机可用于跟踪和验证打印机的注册。</span><span class="sxs-lookup"><span data-stu-id="f2b79-106">This is a long-running operation and as such, it returns a [printerCreateOperation](../resources/printercreateoperation.md) that can be used to track and verify the registration of the printer.</span></span>

<span data-ttu-id="f2b79-107">有关创建创建打印机所需的证书签名请求 (CSR) ，请参阅 [CSR 生成代码示例](/universal-print/hardware/universal-print-oem-certificate-signing-request)。</span><span class="sxs-lookup"><span data-stu-id="f2b79-107">For help creating the required Certificate Signing Request (CSR) for creating printer, see the [CSR generation code sample](/universal-print/hardware/universal-print-oem-certificate-signing-request).</span></span>

## <a name="permissions"></a><span data-ttu-id="f2b79-108">权限</span><span class="sxs-lookup"><span data-stu-id="f2b79-108">Permissions</span></span>
<span data-ttu-id="f2b79-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="f2b79-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="f2b79-111">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="f2b79-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="f2b79-112">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="f2b79-112">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="f2b79-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="f2b79-113">Permission type</span></span> | <span data-ttu-id="f2b79-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="f2b79-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="f2b79-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="f2b79-115">Delegated (work or school account)</span></span>| <span data-ttu-id="f2b79-116">Printer.Create、Printer.ReadWrite.All、Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="f2b79-116">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="f2b79-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="f2b79-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2b79-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2b79-118">Not Supported.</span></span>|
|<span data-ttu-id="f2b79-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="f2b79-119">Application</span></span>| <span data-ttu-id="f2b79-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="f2b79-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="f2b79-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="f2b79-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/create
```

## <a name="request-headers"></a><span data-ttu-id="f2b79-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="f2b79-122">Request headers</span></span>
|<span data-ttu-id="f2b79-123">名称</span><span class="sxs-lookup"><span data-stu-id="f2b79-123">Name</span></span>|<span data-ttu-id="f2b79-124">说明</span><span class="sxs-lookup"><span data-stu-id="f2b79-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="f2b79-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2b79-125">Authorization</span></span>|<span data-ttu-id="f2b79-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="f2b79-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="f2b79-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="f2b79-128">Content-Type</span></span>|<span data-ttu-id="f2b79-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="f2b79-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2b79-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="f2b79-131">Request body</span></span>
<span data-ttu-id="f2b79-132">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f2b79-132">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="f2b79-133">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="f2b79-133">The following table shows the parameters that can be used with this action.</span></span>

| <span data-ttu-id="f2b79-134">参数</span><span class="sxs-lookup"><span data-stu-id="f2b79-134">Parameter</span></span>      | <span data-ttu-id="f2b79-135">类型</span><span class="sxs-lookup"><span data-stu-id="f2b79-135">Type</span></span>    |<span data-ttu-id="f2b79-136">说明</span><span class="sxs-lookup"><span data-stu-id="f2b79-136">Description</span></span>| <span data-ttu-id="f2b79-137">是否必需？</span><span class="sxs-lookup"><span data-stu-id="f2b79-137">Required?</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="f2b79-138">displayName</span><span class="sxs-lookup"><span data-stu-id="f2b79-138">displayName</span></span>|<span data-ttu-id="f2b79-139">字符串</span><span class="sxs-lookup"><span data-stu-id="f2b79-139">String</span></span>|<span data-ttu-id="f2b79-140">要显示名称打印机的打印机。</span><span class="sxs-lookup"><span data-stu-id="f2b79-140">The display name to assign to the printer.</span></span>|<span data-ttu-id="f2b79-141">是</span><span class="sxs-lookup"><span data-stu-id="f2b79-141">Yes</span></span>|
|<span data-ttu-id="f2b79-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="f2b79-142">manufacturer</span></span>|<span data-ttu-id="f2b79-143">String</span><span class="sxs-lookup"><span data-stu-id="f2b79-143">String</span></span>|<span data-ttu-id="f2b79-144">打印机的制造商。</span><span class="sxs-lookup"><span data-stu-id="f2b79-144">The manufacturer of the printer.</span></span>|<span data-ttu-id="f2b79-145">是</span><span class="sxs-lookup"><span data-stu-id="f2b79-145">Yes</span></span>|
|<span data-ttu-id="f2b79-146">model</span><span class="sxs-lookup"><span data-stu-id="f2b79-146">model</span></span>|<span data-ttu-id="f2b79-147">String</span><span class="sxs-lookup"><span data-stu-id="f2b79-147">String</span></span>|<span data-ttu-id="f2b79-148">打印机的模型。</span><span class="sxs-lookup"><span data-stu-id="f2b79-148">The model of the printer.</span></span>|<span data-ttu-id="f2b79-149">是</span><span class="sxs-lookup"><span data-stu-id="f2b79-149">Yes</span></span>|
|<span data-ttu-id="f2b79-150">physicalDeviceId</span><span class="sxs-lookup"><span data-stu-id="f2b79-150">physicalDeviceId</span></span>|<span data-ttu-id="f2b79-151">字符串</span><span class="sxs-lookup"><span data-stu-id="f2b79-151">String</span></span>|<span data-ttu-id="f2b79-152">打印机的物理设备 UUID。</span><span class="sxs-lookup"><span data-stu-id="f2b79-152">The physical device UUID of the printer.</span></span> <span data-ttu-id="f2b79-153">如果属性为 `hasPhysicalDevice` true，则必需。</span><span class="sxs-lookup"><span data-stu-id="f2b79-153">Required if the `hasPhysicalDevice` property is true.</span></span>|<span data-ttu-id="f2b79-154">否</span><span class="sxs-lookup"><span data-stu-id="f2b79-154">No</span></span>|
|<span data-ttu-id="f2b79-155">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="f2b79-155">hasPhysicalDevice</span></span>|<span data-ttu-id="f2b79-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="f2b79-156">Boolean</span></span>|<span data-ttu-id="f2b79-157">如果打印机具有物理输出设备，则其为 True，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="f2b79-157">True if the printer has physical output device, false otherwise.</span></span> <span data-ttu-id="f2b79-158">如果省略，则默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="f2b79-158">If omitted, the default value is true.</span></span>|<span data-ttu-id="f2b79-159">否</span><span class="sxs-lookup"><span data-stu-id="f2b79-159">No</span></span>|
|<span data-ttu-id="f2b79-160">certificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="f2b79-160">certificateSigningRequest</span></span>|[<span data-ttu-id="f2b79-161">printCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="f2b79-161">printCertificateSigningRequest</span></span>](../resources/printcertificatesigningrequest.md)|<span data-ttu-id="f2b79-162">X.509 证书签名请求 (CSR) 由打印机创建和用于标识自身的证书。</span><span class="sxs-lookup"><span data-stu-id="f2b79-162">The X.509 Certificate Signing Request (CSR) for the certificate created and used by the printer to identify itself.</span></span>|<span data-ttu-id="f2b79-163">是</span><span class="sxs-lookup"><span data-stu-id="f2b79-163">Yes</span></span>|
|<span data-ttu-id="f2b79-164">connectorId</span><span class="sxs-lookup"><span data-stu-id="f2b79-164">connectorId</span></span>|<span data-ttu-id="f2b79-165">字符串</span><span class="sxs-lookup"><span data-stu-id="f2b79-165">String</span></span>|<span data-ttu-id="f2b79-166">充当打印机代理的连接器的 ID。</span><span class="sxs-lookup"><span data-stu-id="f2b79-166">ID of the connector acting as proxy to the printer.</span></span>|<span data-ttu-id="f2b79-167">否</span><span class="sxs-lookup"><span data-stu-id="f2b79-167">No</span></span>|

## <a name="response"></a><span data-ttu-id="f2b79-168">响应</span><span class="sxs-lookup"><span data-stu-id="f2b79-168">Response</span></span>
<span data-ttu-id="f2b79-169">如果成功，此方法在标头中返回 响应代码和关联 `202 Accepted` [printerCreateOperation](../resources/printercreateoperation.md) `Operation-Location` 的链接。</span><span class="sxs-lookup"><span data-stu-id="f2b79-169">If successful, this method returns a `202 Accepted` response code and a link to the associated [printerCreateOperation](../resources/printercreateoperation.md) in the `Operation-Location` header.</span></span>

<span data-ttu-id="f2b79-170">对链接的 URL 进行 GET 请求，获取正在进行的打印机注册的状态。</span><span class="sxs-lookup"><span data-stu-id="f2b79-170">You make a GET request to the linked URL to get the status of an ongoing printer registration.</span></span> <span data-ttu-id="f2b79-171">成功完成打印机注册后，对链接 URL 的 GET 请求将包含创建的打印机对象和注册的证书。</span><span class="sxs-lookup"><span data-stu-id="f2b79-171">After printer registration has completed successfully, a GET request to the linked URL will contain the created printer object and registered certificate.</span></span>

## <a name="examples"></a><span data-ttu-id="f2b79-172">示例</span><span class="sxs-lookup"><span data-stu-id="f2b79-172">Examples</span></span>

### <a name="request"></a><span data-ttu-id="f2b79-173">请求</span><span class="sxs-lookup"><span data-stu-id="f2b79-173">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="f2b79-174">HTTP</span><span class="sxs-lookup"><span data-stu-id="f2b79-174">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "printer_create"
}
-->
``` http
POST https://graph.microsoft.com/v1.0/print/printers/create
Content-Type: application/json
Content-length: 287

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
# <a name="c"></a>[<span data-ttu-id="f2b79-175">C#</span><span class="sxs-lookup"><span data-stu-id="f2b79-175">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/printer-create-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="f2b79-176">JavaScript</span><span class="sxs-lookup"><span data-stu-id="f2b79-176">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/printer-create-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="f2b79-177">Objective-C</span><span class="sxs-lookup"><span data-stu-id="f2b79-177">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/printer-create-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="f2b79-178">Java</span><span class="sxs-lookup"><span data-stu-id="f2b79-178">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/printer-create-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="f2b79-179">响应</span><span class="sxs-lookup"><span data-stu-id="f2b79-179">Response</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 202 Accepted
Operation-Location: https://graph.microsoft.com/v1.0/print/operations/f221760a-52e8-4c11-b8c5-5dfaef3a49db
Retry-After: 5
```

