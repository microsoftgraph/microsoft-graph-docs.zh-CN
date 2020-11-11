---
title: 更新打印机
description: 更新 printer 对象的属性。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 95af5526edbbd40a65e3356efa7cee76cf135c14
ms.sourcegitcommit: a9720ab80625a4692f7d2450164717853535d0b0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/11/2020
ms.locfileid: "48993967"
---
# <a name="update-printer"></a><span data-ttu-id="df9e3-103">更新打印机</span><span class="sxs-lookup"><span data-stu-id="df9e3-103">Update printer</span></span>

<span data-ttu-id="df9e3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="df9e3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="df9e3-105">更新 [printer](../resources/printer.md) 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="df9e3-105">Update the properties of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="df9e3-106">权限</span><span class="sxs-lookup"><span data-stu-id="df9e3-106">Permissions</span></span>
<span data-ttu-id="df9e3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="df9e3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="df9e3-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="df9e3-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="df9e3-110">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="df9e3-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

<span data-ttu-id="df9e3-111">仅允许注册打印机的应用程序使用应用程序权限更新打印机。</span><span class="sxs-lookup"><span data-stu-id="df9e3-111">Only the app that registered the printer is allowed to update the printer using application permissions.</span></span>

|<span data-ttu-id="df9e3-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="df9e3-112">Permission type</span></span> | <span data-ttu-id="df9e3-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="df9e3-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="df9e3-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="df9e3-114">Delegated (work or school account)</span></span>| <span data-ttu-id="df9e3-115">完全控制和所有打印机。</span><span class="sxs-lookup"><span data-stu-id="df9e3-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="df9e3-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="df9e3-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="df9e3-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="df9e3-117">Not Supported.</span></span>|
|<span data-ttu-id="df9e3-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="df9e3-118">Application</span></span>| <span data-ttu-id="df9e3-119">Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="df9e3-119">Printer.ReadWrite.All</span></span> |

><span data-ttu-id="df9e3-120">**注意：** 现在，只有没有物理设备的打印机可以使用应用程序权限进行更新。</span><span class="sxs-lookup"><span data-stu-id="df9e3-120">**Note:** Right now, only printers that don't have physical device can be updated using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="df9e3-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="df9e3-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printers/{id}
```
## <a name="request-headers"></a><span data-ttu-id="df9e3-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="df9e3-122">Request headers</span></span>
| <span data-ttu-id="df9e3-123">名称</span><span class="sxs-lookup"><span data-stu-id="df9e3-123">Name</span></span>       | <span data-ttu-id="df9e3-124">说明</span><span class="sxs-lookup"><span data-stu-id="df9e3-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="df9e3-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="df9e3-125">Authorization</span></span> | <span data-ttu-id="df9e3-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="df9e3-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="df9e3-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="df9e3-128">Content-type</span></span>  | <span data-ttu-id="df9e3-129">`application/json` 使用委派权限时， `application/ipp` 使用应用程序权限时。</span><span class="sxs-lookup"><span data-stu-id="df9e3-129">`application/json` when using delegated permissions, `application/ipp` when using application permissions.</span></span> <span data-ttu-id="df9e3-130">必需。</span><span class="sxs-lookup"><span data-stu-id="df9e3-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="df9e3-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="df9e3-131">Request body</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="df9e3-132">委派权限和 JSON 有效负载</span><span class="sxs-lookup"><span data-stu-id="df9e3-132">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="df9e3-133">如果使用委派权限，则在请求正文中，提供应更新的相关 [打印机](../resources/printer.md) 字段的值。</span><span class="sxs-lookup"><span data-stu-id="df9e3-133">If using delegated permissions, in the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="df9e3-134">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="df9e3-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="df9e3-135">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="df9e3-135">For best performance, don't include existing values that haven't changed.</span></span> 

<span data-ttu-id="df9e3-136">可以使用委派权限更新以下属性。</span><span class="sxs-lookup"><span data-stu-id="df9e3-136">The following properties can be updated using delegated permissions.</span></span>

| <span data-ttu-id="df9e3-137">属性</span><span class="sxs-lookup"><span data-stu-id="df9e3-137">Property</span></span>     | <span data-ttu-id="df9e3-138">类型</span><span class="sxs-lookup"><span data-stu-id="df9e3-138">Type</span></span>        | <span data-ttu-id="df9e3-139">说明</span><span class="sxs-lookup"><span data-stu-id="df9e3-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="df9e3-140">defaults</span><span class="sxs-lookup"><span data-stu-id="df9e3-140">defaults</span></span>|[<span data-ttu-id="df9e3-141">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="df9e3-141">printerDefaults</span></span>](../resources/printerdefaults.md)|<span data-ttu-id="df9e3-142">打印机的默认打印设置。</span><span class="sxs-lookup"><span data-stu-id="df9e3-142">The printer's default print settings.</span></span>|
|<span data-ttu-id="df9e3-143">位置</span><span class="sxs-lookup"><span data-stu-id="df9e3-143">location</span></span>|[<span data-ttu-id="df9e3-144">printerLocation</span><span class="sxs-lookup"><span data-stu-id="df9e3-144">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="df9e3-145">打印机的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="df9e3-145">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="df9e3-146">displayName</span><span class="sxs-lookup"><span data-stu-id="df9e3-146">displayName</span></span>|<span data-ttu-id="df9e3-147">字符串</span><span class="sxs-lookup"><span data-stu-id="df9e3-147">String</span></span>|<span data-ttu-id="df9e3-148">打印机的名称。</span><span class="sxs-lookup"><span data-stu-id="df9e3-148">The name of the printer.</span></span>|

### <a name="application-permissions-and-json-payload"></a><span data-ttu-id="df9e3-149">应用程序权限和 JSON 有效负载</span><span class="sxs-lookup"><span data-stu-id="df9e3-149">Application permissions and JSON payload</span></span>
<span data-ttu-id="df9e3-150">在请求正文中，提供应更新的相关 [打印机](../resources/printer.md) 字段的值。</span><span class="sxs-lookup"><span data-stu-id="df9e3-150">In the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="df9e3-151">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="df9e3-151">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="df9e3-152">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="df9e3-152">For best performance, don't include existing values that haven't changed.</span></span> 

<span data-ttu-id="df9e3-153">可以使用应用程序权限更新以下属性。</span><span class="sxs-lookup"><span data-stu-id="df9e3-153">The following properties can be updated using application permissions.</span></span>

| <span data-ttu-id="df9e3-154">属性</span><span class="sxs-lookup"><span data-stu-id="df9e3-154">Property</span></span>     | <span data-ttu-id="df9e3-155">类型</span><span class="sxs-lookup"><span data-stu-id="df9e3-155">Type</span></span>        | <span data-ttu-id="df9e3-156">说明</span><span class="sxs-lookup"><span data-stu-id="df9e3-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="df9e3-157">defaults</span><span class="sxs-lookup"><span data-stu-id="df9e3-157">defaults</span></span>|[<span data-ttu-id="df9e3-158">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="df9e3-158">printerDefaults</span></span>](../resources/printerdefaults.md)|<span data-ttu-id="df9e3-159">打印机的默认打印设置。</span><span class="sxs-lookup"><span data-stu-id="df9e3-159">The printer's default print settings.</span></span>|
|<span data-ttu-id="df9e3-160">capabilities</span><span class="sxs-lookup"><span data-stu-id="df9e3-160">capabilities</span></span>|[<span data-ttu-id="df9e3-161">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="df9e3-161">printerCapabilities</span></span>](../resources/printerCapabilities.md)|<span data-ttu-id="df9e3-162">与此打印机共享相关联的打印机的功能。</span><span class="sxs-lookup"><span data-stu-id="df9e3-162">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="df9e3-163">displayName</span><span class="sxs-lookup"><span data-stu-id="df9e3-163">displayName</span></span>|<span data-ttu-id="df9e3-164">字符串</span><span class="sxs-lookup"><span data-stu-id="df9e3-164">String</span></span>|<span data-ttu-id="df9e3-165">打印机的名称。</span><span class="sxs-lookup"><span data-stu-id="df9e3-165">The name of the printer.</span></span>|
|<span data-ttu-id="df9e3-166">manufacturer</span><span class="sxs-lookup"><span data-stu-id="df9e3-166">manufacturer</span></span>|<span data-ttu-id="df9e3-167">String</span><span class="sxs-lookup"><span data-stu-id="df9e3-167">String</span></span>|<span data-ttu-id="df9e3-168">打印机的制造商。</span><span class="sxs-lookup"><span data-stu-id="df9e3-168">The manufacturer of the printer.</span></span>|
|<span data-ttu-id="df9e3-169">model</span><span class="sxs-lookup"><span data-stu-id="df9e3-169">model</span></span>|<span data-ttu-id="df9e3-170">String</span><span class="sxs-lookup"><span data-stu-id="df9e3-170">String</span></span>|<span data-ttu-id="df9e3-171">打印机的模型名称。</span><span class="sxs-lookup"><span data-stu-id="df9e3-171">The model name of the printer.</span></span>|
|<span data-ttu-id="df9e3-172">status</span><span class="sxs-lookup"><span data-stu-id="df9e3-172">status</span></span>|[<span data-ttu-id="df9e3-173">printerStatus</span><span class="sxs-lookup"><span data-stu-id="df9e3-173">printerStatus</span></span>](../resources/printerstatus.md)|<span data-ttu-id="df9e3-174">打印机的处理状态，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="df9e3-174">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="df9e3-175">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="df9e3-175">isAcceptingJobs</span></span>|<span data-ttu-id="df9e3-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="df9e3-176">Boolean</span></span>|<span data-ttu-id="df9e3-177">打印机当前是否正在接受新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="df9e3-177">Whether the printer is currently accepting new print jobs.</span></span>|

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="df9e3-178">应用程序权限和 IPP 有效负载</span><span class="sxs-lookup"><span data-stu-id="df9e3-178">Application permissions and IPP payload</span></span>

<span data-ttu-id="df9e3-179">使用应用程序权限，还可以使用 Internet 打印协议 (IPP) 有效负载更新打印机。</span><span class="sxs-lookup"><span data-stu-id="df9e3-179">With application permissions, a printer can also be updated using an Internet Printing Protocol (IPP) payload.</span></span> <span data-ttu-id="df9e3-180">在这种情况下，请求正文包含表示 [IPP 编码](https://tools.ietf.org/html/rfc8010)中的打印机属性组的二进制流。</span><span class="sxs-lookup"><span data-stu-id="df9e3-180">In this case, the request body contains a binary stream that represents the Printer Attributes group in [IPP encoding](https://tools.ietf.org/html/rfc8010).</span></span>

<span data-ttu-id="df9e3-181">客户端必须提供一组包含一个或多个值 (的打印机属性，包括在 [RFC8011 节 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) 作业模板 ( 属性中定义的显式允许的带外值) 如 "xxx-默认"、"支持 xxx" 和 "xxx-ready" 属性) 、 [Section 5.4](https://tools.ietf.org/html/rfc8011#section-5.4) 打印机说明属性和打印机支持的任何属性扩展。</span><span class="sxs-lookup"><span data-stu-id="df9e3-181">The client MUST supply a set of Printer attributes with one or more values (including explicitly allowed out-of-band values) as defined in [RFC8011 section 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) Job Template Attributes ("xxx-default", "xxx-supported", and "xxx-ready" attributes), [Section 5.4](https://tools.ietf.org/html/rfc8011#section-5.4) Printer Description Attributes, and any attribute extensions supported by the Printer.</span></span> <span data-ttu-id="df9e3-182">提供的每个打印机属性 (s) 的值将替换目标打印机对象上对应的打印机属性) 的值 (s。</span><span class="sxs-lookup"><span data-stu-id="df9e3-182">The value(s) of each Printer attribute supplied replaces the value(s) of the corresponding Printer attribute on the target Printer object.</span></span> <span data-ttu-id="df9e3-183">对于可以具有多个值 (1setOf) 的属性，客户端提供的所有值都将替换相应的打印机对象属性的所有值。</span><span class="sxs-lookup"><span data-stu-id="df9e3-183">For attributes that can have multiple values (1setOf), all values supplied by the client replace all values of the corresponding Printer object attribute.</span></span>

## <a name="response"></a><span data-ttu-id="df9e3-184">响应</span><span class="sxs-lookup"><span data-stu-id="df9e3-184">Response</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="df9e3-185">委派权限和 JSON 有效负载</span><span class="sxs-lookup"><span data-stu-id="df9e3-185">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="df9e3-186">如果使用委派权限，如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [printer](../resources/printer.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df9e3-186">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-json-payload"></a><span data-ttu-id="df9e3-187">应用程序权限和 JSON 有效负载</span><span class="sxs-lookup"><span data-stu-id="df9e3-187">Application permissions and JSON payload</span></span>

<span data-ttu-id="df9e3-188">如果使用委派权限，如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [printer](../resources/printer.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="df9e3-188">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="df9e3-189">应用程序权限和 IPP 有效负载</span><span class="sxs-lookup"><span data-stu-id="df9e3-189">Application permissions and IPP payload</span></span>

<span data-ttu-id="df9e3-190">如果使用应用程序权限，如果成功，此方法将返回 `204 No content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="df9e3-190">If using application permissions, if successful, this method returns `204 No content` response code.</span></span> <span data-ttu-id="df9e3-191">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="df9e3-191">It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="df9e3-192">示例</span><span class="sxs-lookup"><span data-stu-id="df9e3-192">Example</span></span>

### <a name="request"></a><span data-ttu-id="df9e3-193">请求</span><span class="sxs-lookup"><span data-stu-id="df9e3-193">Request</span></span>
<span data-ttu-id="df9e3-194">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="df9e3-194">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="df9e3-195">HTTP</span><span class="sxs-lookup"><span data-stu-id="df9e3-195">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printer"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/printers/{id}
Content-type: application/json
Content-length: 124

{
  "name": "PrinterName",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3
  }
}
```
# <a name="c"></a>[<span data-ttu-id="df9e3-196">C#</span><span class="sxs-lookup"><span data-stu-id="df9e3-196">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printer-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="df9e3-197">JavaScript</span><span class="sxs-lookup"><span data-stu-id="df9e3-197">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="df9e3-198">Objective-C</span><span class="sxs-lookup"><span data-stu-id="df9e3-198">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="df9e3-199">Java</span><span class="sxs-lookup"><span data-stu-id="df9e3-199">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printer-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

### <a name="response"></a><span data-ttu-id="df9e3-200">响应</span><span class="sxs-lookup"><span data-stu-id="df9e3-200">Response</span></span>
<span data-ttu-id="df9e3-201">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="df9e3-201">The following is an example of the response.</span></span>
><span data-ttu-id="df9e3-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="df9e3-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1313

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "name": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "acceptingJobs": true,
  "status": {
    "processingState": "idle",
    "processingStateReasons": [],
    "processingStateDescription": ""
  },
  "defaults": {
    "copiesPerJob":1,
    "documentMimeType": "application/oxps",
    "finishings": ["none"],
    "mediaType": "stationery"
  },
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3,
    "streetAddress": "One Microsoft Way",
    "subUnit": [
        "Main Plaza",
        "Unit 400"
    ],
    "city": "Redmond",
    "postalCode": "98052",
    "countryOrRegion": "USA",
    "site": "Puget Sound",
    "building": "Studio E",
    "floorNumber": 1,
    "floorDescription": "First Floor",
    "roomNumber": 1234,
    "roomDescription": "First floor copy room",
    "organization": [
        "C+AI",
        "Microsoft Graph"
    ],
    "subdivision": [
        "King County",
        "Red West"
    ],
    "stateOrProvince": "Washington"
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update printer",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
