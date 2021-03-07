---
title: printer： create
description: 创建 (通用) 打印服务在打印机上注册。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 58285c3c6908812edce8ad80915f44f4df08fcb8
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516993"
---
# <a name="printer-create"></a><span data-ttu-id="65722-103">printer： create</span><span class="sxs-lookup"><span data-stu-id="65722-103">printer: create</span></span>
<span data-ttu-id="65722-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="65722-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="65722-105">创建 (通用) 打印服务在打印机上注册。</span><span class="sxs-lookup"><span data-stu-id="65722-105">Create (register) a printer with the Universal Print service.</span></span> <span data-ttu-id="65722-106">这是一项长时间运行的操作，因此它将返回 [一个 printerCreateOperation，](../resources/printercreateoperation.md) 该打印机可用于跟踪和验证打印机的注册。</span><span class="sxs-lookup"><span data-stu-id="65722-106">This is a long-running operation and as such, it returns a [printerCreateOperation](../resources/printercreateoperation.md) that can be used to track and verify the registration of the printer.</span></span>

<span data-ttu-id="65722-107">有关创建用于创建打印机的 CSR (证书签名请求) ，请参阅 [CSR 生成代码示例](/universal-print/hardware/universal-print-oem-certificate-signing-request)。</span><span class="sxs-lookup"><span data-stu-id="65722-107">For help creating the required Certificate Signing Request (CSR) for creating printer, see the [CSR generation code sample](/universal-print/hardware/universal-print-oem-certificate-signing-request).</span></span>

## <a name="permissions"></a><span data-ttu-id="65722-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="65722-108">Permissions</span></span>
<span data-ttu-id="65722-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="65722-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="65722-111">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="65722-111">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="65722-112">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="65722-112">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="65722-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="65722-113">Permission type</span></span> | <span data-ttu-id="65722-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="65722-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="65722-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="65722-115">Delegated (work or school account)</span></span>| <span data-ttu-id="65722-116">Printer.Create、Printer.ReadWrite.All、Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="65722-116">Printer.Create, Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="65722-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="65722-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="65722-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="65722-118">Not Supported.</span></span>|
|<span data-ttu-id="65722-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="65722-119">Application</span></span>| <span data-ttu-id="65722-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="65722-120">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="65722-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="65722-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /print/printers/create
```

## <a name="request-headers"></a><span data-ttu-id="65722-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="65722-122">Request headers</span></span>
|<span data-ttu-id="65722-123">名称</span><span class="sxs-lookup"><span data-stu-id="65722-123">Name</span></span>|<span data-ttu-id="65722-124">说明</span><span class="sxs-lookup"><span data-stu-id="65722-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="65722-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="65722-125">Authorization</span></span>|<span data-ttu-id="65722-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="65722-p104">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="65722-128">Content-Type</span><span class="sxs-lookup"><span data-stu-id="65722-128">Content-Type</span></span>|<span data-ttu-id="65722-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="65722-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="65722-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="65722-131">Request body</span></span>
<span data-ttu-id="65722-132">在请求正文中，提供参数的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="65722-132">In the request body, supply a JSON representation of the parameters.</span></span>

<span data-ttu-id="65722-133">下表显示了可用于此操作的参数。</span><span class="sxs-lookup"><span data-stu-id="65722-133">The following table shows the parameters that can be used with this action.</span></span>

| <span data-ttu-id="65722-134">参数</span><span class="sxs-lookup"><span data-stu-id="65722-134">Parameter</span></span>      | <span data-ttu-id="65722-135">类型</span><span class="sxs-lookup"><span data-stu-id="65722-135">Type</span></span>    |<span data-ttu-id="65722-136">Description</span><span class="sxs-lookup"><span data-stu-id="65722-136">Description</span></span>| <span data-ttu-id="65722-137">是否必需？</span><span class="sxs-lookup"><span data-stu-id="65722-137">Required?</span></span> |
|:---------------|:--------|:----------|:----------|
|<span data-ttu-id="65722-138">displayName</span><span class="sxs-lookup"><span data-stu-id="65722-138">displayName</span></span>|<span data-ttu-id="65722-139">String</span><span class="sxs-lookup"><span data-stu-id="65722-139">String</span></span>|<span data-ttu-id="65722-140">要显示名称打印机的打印机。</span><span class="sxs-lookup"><span data-stu-id="65722-140">The display name to assign to the printer.</span></span>|<span data-ttu-id="65722-141">是</span><span class="sxs-lookup"><span data-stu-id="65722-141">Yes</span></span>|
|<span data-ttu-id="65722-142">manufacturer</span><span class="sxs-lookup"><span data-stu-id="65722-142">manufacturer</span></span>|<span data-ttu-id="65722-143">String</span><span class="sxs-lookup"><span data-stu-id="65722-143">String</span></span>|<span data-ttu-id="65722-144">打印机的制造商。</span><span class="sxs-lookup"><span data-stu-id="65722-144">The manufacturer of the printer.</span></span>|<span data-ttu-id="65722-145">是</span><span class="sxs-lookup"><span data-stu-id="65722-145">Yes</span></span>|
|<span data-ttu-id="65722-146">model</span><span class="sxs-lookup"><span data-stu-id="65722-146">model</span></span>|<span data-ttu-id="65722-147">String</span><span class="sxs-lookup"><span data-stu-id="65722-147">String</span></span>|<span data-ttu-id="65722-148">打印机的模型。</span><span class="sxs-lookup"><span data-stu-id="65722-148">The model of the printer.</span></span>|<span data-ttu-id="65722-149">是</span><span class="sxs-lookup"><span data-stu-id="65722-149">Yes</span></span>|
|<span data-ttu-id="65722-150">physicalDeviceId</span><span class="sxs-lookup"><span data-stu-id="65722-150">physicalDeviceId</span></span>|<span data-ttu-id="65722-151">String</span><span class="sxs-lookup"><span data-stu-id="65722-151">String</span></span>|<span data-ttu-id="65722-152">打印机的物理设备 UUID。</span><span class="sxs-lookup"><span data-stu-id="65722-152">The physical device UUID of the printer.</span></span> <span data-ttu-id="65722-153">如果该属性为 `hasPhysicalDevice` true，则必需。</span><span class="sxs-lookup"><span data-stu-id="65722-153">Required if the `hasPhysicalDevice` property is true.</span></span>|<span data-ttu-id="65722-154">否</span><span class="sxs-lookup"><span data-stu-id="65722-154">No</span></span>|
|<span data-ttu-id="65722-155">hasPhysicalDevice</span><span class="sxs-lookup"><span data-stu-id="65722-155">hasPhysicalDevice</span></span>|<span data-ttu-id="65722-156">Boolean</span><span class="sxs-lookup"><span data-stu-id="65722-156">Boolean</span></span>|<span data-ttu-id="65722-157">如果打印机具有物理输出设备，则其为 True，否则为 false。</span><span class="sxs-lookup"><span data-stu-id="65722-157">True if the printer has physical output device, false otherwise.</span></span> <span data-ttu-id="65722-158">如果省略，则默认值为 true。</span><span class="sxs-lookup"><span data-stu-id="65722-158">If omitted, the default value is true.</span></span>|<span data-ttu-id="65722-159">否</span><span class="sxs-lookup"><span data-stu-id="65722-159">No</span></span>|
|<span data-ttu-id="65722-160">certificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="65722-160">certificateSigningRequest</span></span>|[<span data-ttu-id="65722-161">printCertificateSigningRequest</span><span class="sxs-lookup"><span data-stu-id="65722-161">printCertificateSigningRequest</span></span>](../resources/printcertificatesigningrequest.md)|<span data-ttu-id="65722-162">X.509 证书签名请求 (CSR) ，用于打印机创建和用于标识自己的证书。</span><span class="sxs-lookup"><span data-stu-id="65722-162">The X.509 Certificate Signing Request (CSR) for the certificate created and used by the printer to identify itself.</span></span>|<span data-ttu-id="65722-163">是</span><span class="sxs-lookup"><span data-stu-id="65722-163">Yes</span></span>|
|<span data-ttu-id="65722-164">connectorId</span><span class="sxs-lookup"><span data-stu-id="65722-164">connectorId</span></span>|<span data-ttu-id="65722-165">String</span><span class="sxs-lookup"><span data-stu-id="65722-165">String</span></span>|<span data-ttu-id="65722-166">充当打印机代理的连接器的 ID。</span><span class="sxs-lookup"><span data-stu-id="65722-166">ID of the connector acting as proxy to the printer.</span></span>|<span data-ttu-id="65722-167">否</span><span class="sxs-lookup"><span data-stu-id="65722-167">No</span></span>|

## <a name="response"></a><span data-ttu-id="65722-168">响应</span><span class="sxs-lookup"><span data-stu-id="65722-168">Response</span></span>
<span data-ttu-id="65722-169">如果成功，此方法在标头中返回响应代码和指向关联的 `202 Accepted` [printerCreateOperation](../resources/printercreateoperation.md) `Operation-Location` 的链接。</span><span class="sxs-lookup"><span data-stu-id="65722-169">If successful, this method returns a `202 Accepted` response code and a link to the associated [printerCreateOperation](../resources/printercreateoperation.md) in the `Operation-Location` header.</span></span>

<span data-ttu-id="65722-170">您可以对链接的 URL 进行 GET 请求，获取正在进行的打印机注册的状态。</span><span class="sxs-lookup"><span data-stu-id="65722-170">You make a GET request to the linked URL to get the status of an ongoing printer registration.</span></span> <span data-ttu-id="65722-171">成功完成打印机注册后，对链接 URL 的 GET 请求将包含创建的打印机对象和注册的证书。</span><span class="sxs-lookup"><span data-stu-id="65722-171">After printer registration has completed successfully, a GET request to the linked URL will contain the created printer object and registered certificate.</span></span>

## <a name="examples"></a><span data-ttu-id="65722-172">示例</span><span class="sxs-lookup"><span data-stu-id="65722-172">Examples</span></span>

### <a name="request"></a><span data-ttu-id="65722-173">请求</span><span class="sxs-lookup"><span data-stu-id="65722-173">Request</span></span>
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


### <a name="response"></a><span data-ttu-id="65722-174">响应</span><span class="sxs-lookup"><span data-stu-id="65722-174">Response</span></span>

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

