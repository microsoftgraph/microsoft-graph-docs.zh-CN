---
title: 更新打印机
description: 更新打印机对象的属性。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: a479aff38b24105e80d3fc0c3f098299b9eeafb4
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51765879"
---
# <a name="update-printer"></a><span data-ttu-id="625bc-103">更新打印机</span><span class="sxs-lookup"><span data-stu-id="625bc-103">Update printer</span></span>
<span data-ttu-id="625bc-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="625bc-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="625bc-105">更新 [打印机对象的属性](../resources/printer.md) 。</span><span class="sxs-lookup"><span data-stu-id="625bc-105">Update the properties of a [printer](../resources/printer.md) object.</span></span>

## <a name="permissions"></a><span data-ttu-id="625bc-106">权限</span><span class="sxs-lookup"><span data-stu-id="625bc-106">Permissions</span></span>
<span data-ttu-id="625bc-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="625bc-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="625bc-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="625bc-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="625bc-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="625bc-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

><span data-ttu-id="625bc-111">**注意：** 仅允许注册打印机的应用使用应用程序权限更新打印机。</span><span class="sxs-lookup"><span data-stu-id="625bc-111">**Note:** Only the app that registered the printer is allowed to update the printer using application permissions.</span></span>

|<span data-ttu-id="625bc-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="625bc-112">Permission type</span></span> | <span data-ttu-id="625bc-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="625bc-113">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="625bc-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="625bc-114">Delegated (work or school account)</span></span>| <span data-ttu-id="625bc-115">Printer.ReadWrite.All、Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="625bc-115">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="625bc-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="625bc-116">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="625bc-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="625bc-117">Not Supported.</span></span>|
|<span data-ttu-id="625bc-118">Application</span><span class="sxs-lookup"><span data-stu-id="625bc-118">Application</span></span>| <span data-ttu-id="625bc-119">Printer.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="625bc-119">Printer.ReadWrite.All</span></span> |

><span data-ttu-id="625bc-120">**注意：** 目前，只有没有物理设备的打印机可以使用应用程序权限进行更新。</span><span class="sxs-lookup"><span data-stu-id="625bc-120">**Note:** Right now, only printers that don't have physical device can be updated using application permissions.</span></span>

## <a name="http-request"></a><span data-ttu-id="625bc-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="625bc-121">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/printers/{printerId}
```

## <a name="request-headers"></a><span data-ttu-id="625bc-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="625bc-122">Request headers</span></span>
|<span data-ttu-id="625bc-123">名称</span><span class="sxs-lookup"><span data-stu-id="625bc-123">Name</span></span>|<span data-ttu-id="625bc-124">说明</span><span class="sxs-lookup"><span data-stu-id="625bc-124">Description</span></span>|
|:---|:---|
|<span data-ttu-id="625bc-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="625bc-125">Authorization</span></span>|<span data-ttu-id="625bc-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="625bc-p103">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="625bc-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="625bc-128">Content-type</span></span>|<span data-ttu-id="625bc-129">`application/json` 使用委派权限时， `application/ipp` 或者 `application/json` 使用应用程序权限时。</span><span class="sxs-lookup"><span data-stu-id="625bc-129">`application/json` when using delegated permissions, `application/ipp` or `application/json` when using application permissions.</span></span> <span data-ttu-id="625bc-130">必填。</span><span class="sxs-lookup"><span data-stu-id="625bc-130">Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="625bc-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="625bc-131">Request body</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="625bc-132">委派的权限和 JSON 有效负载</span><span class="sxs-lookup"><span data-stu-id="625bc-132">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="625bc-133">如果使用委派权限，在请求正文中， [提供应更新](../resources/printer.md) 的相关打印机字段的值。</span><span class="sxs-lookup"><span data-stu-id="625bc-133">If using delegated permissions, in the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="625bc-134">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="625bc-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="625bc-135">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="625bc-135">For best performance, don't include existing values that haven't changed.</span></span> 

<span data-ttu-id="625bc-136">可以使用委派权限更新以下属性。</span><span class="sxs-lookup"><span data-stu-id="625bc-136">The following properties can be updated using delegated permissions.</span></span>

| <span data-ttu-id="625bc-137">属性</span><span class="sxs-lookup"><span data-stu-id="625bc-137">Property</span></span>     | <span data-ttu-id="625bc-138">类型</span><span class="sxs-lookup"><span data-stu-id="625bc-138">Type</span></span>        | <span data-ttu-id="625bc-139">说明</span><span class="sxs-lookup"><span data-stu-id="625bc-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="625bc-140">defaults</span><span class="sxs-lookup"><span data-stu-id="625bc-140">defaults</span></span>|[<span data-ttu-id="625bc-141">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="625bc-141">printerDefaults</span></span>](../resources/printerdefaults.md)|<span data-ttu-id="625bc-142">打印机的默认打印设置。</span><span class="sxs-lookup"><span data-stu-id="625bc-142">The printer's default print settings.</span></span>|
|<span data-ttu-id="625bc-143">位置</span><span class="sxs-lookup"><span data-stu-id="625bc-143">location</span></span>|[<span data-ttu-id="625bc-144">printerLocation</span><span class="sxs-lookup"><span data-stu-id="625bc-144">printerLocation</span></span>](../resources/printerlocation.md)|<span data-ttu-id="625bc-145">打印机的物理和/或组织位置。</span><span class="sxs-lookup"><span data-stu-id="625bc-145">The physical and/or organizational location of the printer.</span></span>|
|<span data-ttu-id="625bc-146">displayName</span><span class="sxs-lookup"><span data-stu-id="625bc-146">displayName</span></span>|<span data-ttu-id="625bc-147">String</span><span class="sxs-lookup"><span data-stu-id="625bc-147">String</span></span>|<span data-ttu-id="625bc-148">打印机的名称。</span><span class="sxs-lookup"><span data-stu-id="625bc-148">The name of the printer.</span></span>|

### <a name="application-permissions-and-json-payload"></a><span data-ttu-id="625bc-149">应用程序权限和 JSON 有效负载</span><span class="sxs-lookup"><span data-stu-id="625bc-149">Application permissions and JSON payload</span></span>
<span data-ttu-id="625bc-150">在请求正文中， [提供应更新](../resources/printer.md) 的相关打印机字段的值。</span><span class="sxs-lookup"><span data-stu-id="625bc-150">In the request body, supply the values for the relevant [printer](../resources/printer.md) fields that should be updated.</span></span> <span data-ttu-id="625bc-151">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="625bc-151">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="625bc-152">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="625bc-152">For best performance, don't include existing values that haven't changed.</span></span> 

<span data-ttu-id="625bc-153">可以使用应用程序权限更新以下属性。</span><span class="sxs-lookup"><span data-stu-id="625bc-153">The following properties can be updated using application permissions.</span></span>

| <span data-ttu-id="625bc-154">属性</span><span class="sxs-lookup"><span data-stu-id="625bc-154">Property</span></span>     | <span data-ttu-id="625bc-155">类型</span><span class="sxs-lookup"><span data-stu-id="625bc-155">Type</span></span>        | <span data-ttu-id="625bc-156">说明</span><span class="sxs-lookup"><span data-stu-id="625bc-156">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="625bc-157">defaults</span><span class="sxs-lookup"><span data-stu-id="625bc-157">defaults</span></span>|[<span data-ttu-id="625bc-158">printerDefaults</span><span class="sxs-lookup"><span data-stu-id="625bc-158">printerDefaults</span></span>](../resources/printerdefaults.md)|<span data-ttu-id="625bc-159">打印机的默认打印设置。</span><span class="sxs-lookup"><span data-stu-id="625bc-159">The printer's default print settings.</span></span>|
|<span data-ttu-id="625bc-160">capabilities</span><span class="sxs-lookup"><span data-stu-id="625bc-160">capabilities</span></span>|[<span data-ttu-id="625bc-161">printerCapabilities</span><span class="sxs-lookup"><span data-stu-id="625bc-161">printerCapabilities</span></span>](../resources/printerCapabilities.md)|<span data-ttu-id="625bc-162">与此打印机共享关联的打印机的功能。</span><span class="sxs-lookup"><span data-stu-id="625bc-162">The capabilities of the printer associated with this printer share.</span></span>|
|<span data-ttu-id="625bc-163">displayName</span><span class="sxs-lookup"><span data-stu-id="625bc-163">displayName</span></span>|<span data-ttu-id="625bc-164">String</span><span class="sxs-lookup"><span data-stu-id="625bc-164">String</span></span>|<span data-ttu-id="625bc-165">打印机的名称。</span><span class="sxs-lookup"><span data-stu-id="625bc-165">The name of the printer.</span></span>|
|<span data-ttu-id="625bc-166">manufacturer</span><span class="sxs-lookup"><span data-stu-id="625bc-166">manufacturer</span></span>|<span data-ttu-id="625bc-167">String</span><span class="sxs-lookup"><span data-stu-id="625bc-167">String</span></span>|<span data-ttu-id="625bc-168">打印机的制造商。</span><span class="sxs-lookup"><span data-stu-id="625bc-168">The manufacturer of the printer.</span></span>|
|<span data-ttu-id="625bc-169">model</span><span class="sxs-lookup"><span data-stu-id="625bc-169">model</span></span>|<span data-ttu-id="625bc-170">String</span><span class="sxs-lookup"><span data-stu-id="625bc-170">String</span></span>|<span data-ttu-id="625bc-171">打印机的模型名称。</span><span class="sxs-lookup"><span data-stu-id="625bc-171">The model name of the printer.</span></span>|
|<span data-ttu-id="625bc-172">状态</span><span class="sxs-lookup"><span data-stu-id="625bc-172">status</span></span>|[<span data-ttu-id="625bc-173">printerStatus</span><span class="sxs-lookup"><span data-stu-id="625bc-173">printerStatus</span></span>](../resources/printerstatus.md)|<span data-ttu-id="625bc-174">打印机的处理状态，包括任何错误。</span><span class="sxs-lookup"><span data-stu-id="625bc-174">The processing status of the printer, including any errors.</span></span>|
|<span data-ttu-id="625bc-175">isAcceptingJobs</span><span class="sxs-lookup"><span data-stu-id="625bc-175">isAcceptingJobs</span></span>|<span data-ttu-id="625bc-176">Boolean</span><span class="sxs-lookup"><span data-stu-id="625bc-176">Boolean</span></span>|<span data-ttu-id="625bc-177">打印机当前是否接受新的打印作业。</span><span class="sxs-lookup"><span data-stu-id="625bc-177">Whether the printer is currently accepting new print jobs.</span></span>|

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="625bc-178">应用程序权限和 IPP 有效负载</span><span class="sxs-lookup"><span data-stu-id="625bc-178">Application permissions and IPP payload</span></span>

<span data-ttu-id="625bc-179">使用应用程序权限，还可使用 IPP 负载中的 Internet 打印 (更新) 打印机。</span><span class="sxs-lookup"><span data-stu-id="625bc-179">With application permissions, a printer can also be updated using an Internet Printing Protocol (IPP) payload.</span></span> <span data-ttu-id="625bc-180">在这种情况下，请求正文包含表示 [IPP](https://tools.ietf.org/html/rfc8010)编码中的 Printer Attributes 组的二进制流。</span><span class="sxs-lookup"><span data-stu-id="625bc-180">In this case, the request body contains a binary stream that represents the Printer Attributes group in [IPP encoding](https://tools.ietf.org/html/rfc8010).</span></span>

<span data-ttu-id="625bc-181">客户端必须为一组 Printer 属性提供一个或多个值 (包括 [RFC8011 第 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) 节中定义的明确允许的带外值) 作业模板属性 ("xxx-default"、"xxx-supported"和"xxx-ready"属性) 、 [第 5.4](https://tools.ietf.org/html/rfc8011#section-5.4) 节打印机说明属性以及打印机支持的任何属性扩展。</span><span class="sxs-lookup"><span data-stu-id="625bc-181">The client MUST supply a set of Printer attributes with one or more values (including explicitly allowed out-of-band values) as defined in [RFC8011 section 5.2](https://tools.ietf.org/html/rfc8011#section-5.2) Job Template Attributes ("xxx-default", "xxx-supported", and "xxx-ready" attributes), [Section 5.4](https://tools.ietf.org/html/rfc8011#section-5.4) Printer Description Attributes, and any attribute extensions supported by the Printer.</span></span> <span data-ttu-id="625bc-182">提供 (每个 Printer) 的值将替换 (Printer) 的对应 Printer 属性的值。</span><span class="sxs-lookup"><span data-stu-id="625bc-182">The value(s) of each Printer attribute supplied replaces the value(s) of the corresponding Printer attribute on the target Printer object.</span></span> <span data-ttu-id="625bc-183">对于在 1setOf (可以有多个值) ，客户端提供的所有值将替换相应的 Printer 对象属性的所有值。</span><span class="sxs-lookup"><span data-stu-id="625bc-183">For attributes that can have multiple values (1setOf), all values supplied by the client replace all values of the corresponding Printer object attribute.</span></span>

> <span data-ttu-id="625bc-184">**注意：** 不要传递请求正文中的操作属性。</span><span class="sxs-lookup"><span data-stu-id="625bc-184">**Note:** Do not pass operation attributes in the request body.</span></span> <span data-ttu-id="625bc-185">请求正文应仅包含打印机属性。</span><span class="sxs-lookup"><span data-stu-id="625bc-185">The request body should only contain printer attributes.</span></span>


> <span data-ttu-id="625bc-186">**注意：** 对于使用特定平台的打印机，它应满足该平台的要求。</span><span class="sxs-lookup"><span data-stu-id="625bc-186">**Note:** For printers to work with a particular platform, it should meet the requirements of that platform.</span></span> <span data-ttu-id="625bc-187">例如，在 Windows 客户端上，打印机应根据 [一些功能](https://mopria.org) 规范指定视为必需的所有属性。</span><span class="sxs-lookup"><span data-stu-id="625bc-187">For example, on windows client, it is expected that printer specifies all attributes that are considered mandatory as per [MOPRIA](https://mopria.org) specs.</span></span> <span data-ttu-id="625bc-188">请注意，一些 SPECRIA 规范仅适用于 PAIDRIA 的付费成员。</span><span class="sxs-lookup"><span data-stu-id="625bc-188">Please note MOPRIA specs are available to only the paid members of MOPRIA.</span></span>

## <a name="response"></a><span data-ttu-id="625bc-189">响应</span><span class="sxs-lookup"><span data-stu-id="625bc-189">Response</span></span>

### <a name="delegated-permissions-and-json-payload"></a><span data-ttu-id="625bc-190">委派的权限和 JSON 有效负载</span><span class="sxs-lookup"><span data-stu-id="625bc-190">Delegated permissions and JSON payload</span></span>

<span data-ttu-id="625bc-191">如果使用委派权限，如果成功，此方法在响应正文中返回 响应 `200 OK` 代码和更新的 [printer](../resources/printer.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="625bc-191">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-json-payload"></a><span data-ttu-id="625bc-192">应用程序权限和 JSON 有效负载</span><span class="sxs-lookup"><span data-stu-id="625bc-192">Application permissions and JSON payload</span></span>

<span data-ttu-id="625bc-193">如果使用委派权限，如果成功，此方法在响应正文中返回 响应 `200 OK` 代码和更新的 [printer](../resources/printer.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="625bc-193">If using delegated permissions, if successful, this method returns a `200 OK` response code and an updated [printer](../resources/printer.md) object in the response body.</span></span>

### <a name="application-permissions-and-ipp-payload"></a><span data-ttu-id="625bc-194">应用程序权限和 IPP 有效负载</span><span class="sxs-lookup"><span data-stu-id="625bc-194">Application permissions and IPP payload</span></span>

<span data-ttu-id="625bc-195">如果使用应用程序权限，如果成功，此方法将返回 `204 No content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="625bc-195">If using application permissions, if successful, this method returns `204 No content` response code.</span></span> <span data-ttu-id="625bc-196">它不会在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="625bc-196">It does not return anything in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="625bc-197">示例</span><span class="sxs-lookup"><span data-stu-id="625bc-197">Examples</span></span>

### <a name="request"></a><span data-ttu-id="625bc-198">请求</span><span class="sxs-lookup"><span data-stu-id="625bc-198">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="625bc-199">HTTP</span><span class="sxs-lookup"><span data-stu-id="625bc-199">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printer"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/printers/{printerId}
Content-Type: application/json
Content-length: 581

{
  "name": "PrinterName",
  "location": {
    "latitude": 1.1,
    "longitude": 2.2,
    "altitudeInMeters": 3
  }
}
```
# <a name="javascript"></a>[<span data-ttu-id="625bc-200">JavaScript</span><span class="sxs-lookup"><span data-stu-id="625bc-200">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printer-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="625bc-201">Objective-C</span><span class="sxs-lookup"><span data-stu-id="625bc-201">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printer-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="625bc-202">响应</span><span class="sxs-lookup"><span data-stu-id="625bc-202">Response</span></span>
<span data-ttu-id="625bc-203">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="625bc-203">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printer"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/printers/$entity",
  "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
  "displayName": "PrinterName",
  "manufacturer": "PrinterManufacturer",
  "model": "PrinterModel",
  "isShared": true,
  "registeredDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
  "status": {
    "state": "idle",
    "details": [],
    "description": ""
  },
  "defaults": {
    "copiesPerJob":1,
    "contentType": "application/oxps",
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
    "floor": "1",
    "floorDescription": "First Floor",
    "roomName": "1234",
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

