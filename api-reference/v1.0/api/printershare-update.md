---
title: 更新打印机共享
description: 更新打印机共享的属性。 此方法可用于"交换"打印机。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: ea7da18300105e5c177b126635740fcee918b996
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517309"
---
# <a name="update-printershare"></a><span data-ttu-id="0d3bd-104">更新 printerShare</span><span class="sxs-lookup"><span data-stu-id="0d3bd-104">Update printerShare</span></span>
<span data-ttu-id="0d3bd-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="0d3bd-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="0d3bd-106">更新打印机共享的属性。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-106">Update the properties of a printer share.</span></span> <span data-ttu-id="0d3bd-107">此方法可用于交换 [打印机](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-107">This method can be used to swap [printers](../resources/printer.md).</span></span>

<span data-ttu-id="0d3bd-108">例如，如果物理打印机设备中断，管理员可以注册新的打印机设备，并更新此[](../resources/printer.md) [printerShare](../resources/printerShare.md)以指向新打印机，而无需用户执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-108">For example, if a physical printer device breaks, an administrator can register a new [printer](../resources/printer.md) device and update this [printerShare](../resources/printerShare.md) to point to the new printer without requiring users to take any action.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d3bd-109">Permissions</span><span class="sxs-lookup"><span data-stu-id="0d3bd-109">Permissions</span></span>
<span data-ttu-id="0d3bd-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="0d3bd-112">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="0d3bd-113">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-113">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="0d3bd-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d3bd-114">Permission type</span></span> | <span data-ttu-id="0d3bd-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d3bd-115">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="0d3bd-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d3bd-116">Delegated (work or school account)</span></span>| <span data-ttu-id="0d3bd-117">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="0d3bd-117">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="0d3bd-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d3bd-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="0d3bd-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-119">Not Supported.</span></span>|
|<span data-ttu-id="0d3bd-120">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d3bd-120">Application</span></span>|<span data-ttu-id="0d3bd-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-121">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="0d3bd-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d3bd-122">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /print/shares/{printerShareId}
```

## <a name="request-headers"></a><span data-ttu-id="0d3bd-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d3bd-123">Request headers</span></span>
|<span data-ttu-id="0d3bd-124">名称</span><span class="sxs-lookup"><span data-stu-id="0d3bd-124">Name</span></span>|<span data-ttu-id="0d3bd-125">说明</span><span class="sxs-lookup"><span data-stu-id="0d3bd-125">Description</span></span>|
|:---|:---|
|<span data-ttu-id="0d3bd-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d3bd-126">Authorization</span></span>|<span data-ttu-id="0d3bd-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-p105">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="0d3bd-129">Content-Type</span><span class="sxs-lookup"><span data-stu-id="0d3bd-129">Content-Type</span></span>|<span data-ttu-id="0d3bd-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="0d3bd-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="0d3bd-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d3bd-132">Request body</span></span>
<span data-ttu-id="0d3bd-133">在请求正文中，提供应更新的相关 [printerShare](../resources/printershare.md) 字段的值。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-133">In the request body, supply the values for relevant [printerShare](../resources/printershare.md) fields that should be updated.</span></span> <span data-ttu-id="0d3bd-134">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="0d3bd-135">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-135">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="0d3bd-136">可以更新以下属性：</span><span class="sxs-lookup"><span data-stu-id="0d3bd-136">Following properties can be updated:</span></span> 

| <span data-ttu-id="0d3bd-137">属性</span><span class="sxs-lookup"><span data-stu-id="0d3bd-137">Property</span></span>     | <span data-ttu-id="0d3bd-138">类型</span><span class="sxs-lookup"><span data-stu-id="0d3bd-138">Type</span></span>        | <span data-ttu-id="0d3bd-139">Description</span><span class="sxs-lookup"><span data-stu-id="0d3bd-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="0d3bd-140">打印机</span><span class="sxs-lookup"><span data-stu-id="0d3bd-140">printer</span></span>|<span data-ttu-id="0d3bd-141">microsoft.graph.printer</span><span class="sxs-lookup"><span data-stu-id="0d3bd-141">microsoft.graph.printer</span></span>|<span data-ttu-id="0d3bd-142">此打印机共享相关的打印机。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-142">The printer that this printer share is related to.</span></span> <span data-ttu-id="0d3bd-143">使用 `printer@odata.bind` 以下示例所示的语法更新与此打印机共享关联的打印机。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-143">Use the `printer@odata.bind` syntax as shown in the following example to update which printer this printer share is associated with.</span></span>|
|<span data-ttu-id="0d3bd-144">displayName</span><span class="sxs-lookup"><span data-stu-id="0d3bd-144">displayName</span></span>|<span data-ttu-id="0d3bd-145">String</span><span class="sxs-lookup"><span data-stu-id="0d3bd-145">String</span></span>|<span data-ttu-id="0d3bd-146">打印客户端应显示的打印机共享的名称。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-146">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="0d3bd-147">allowAllUsers</span><span class="sxs-lookup"><span data-stu-id="0d3bd-147">allowAllUsers</span></span>|<span data-ttu-id="0d3bd-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="0d3bd-148">Boolean</span></span>| <span data-ttu-id="0d3bd-149">如果为 true，将授予所有用户和组对此打印机共享的访问权限。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-149">If true, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="0d3bd-150">这将取代 allowedUsers 和 allowedGroups 导航属性定义的允许列表。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-150">This supersedes the allow lists defined by the allowedUsers and allowedGroups navigation properties.</span></span>|

## <a name="response"></a><span data-ttu-id="0d3bd-151">响应</span><span class="sxs-lookup"><span data-stu-id="0d3bd-151">Response</span></span>

<span data-ttu-id="0d3bd-152">如果成功，此方法在响应正文中返回响应 `200 OK` 代码和更新的 [printerShare](../resources/printershare.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-152">If successful, this method returns a `200 OK` response code and an updated [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="0d3bd-153">示例</span><span class="sxs-lookup"><span data-stu-id="0d3bd-153">Examples</span></span>

### <a name="request"></a><span data-ttu-id="0d3bd-154">请求</span><span class="sxs-lookup"><span data-stu-id="0d3bd-154">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "update_printershare"
}
-->
``` http
PATCH https://graph.microsoft.com/v1.0/print/shares/{printerShareId}
Content-Type: application/json
Content-length: 509

{
  "displayName": "PrinterShare Name",
  "printer@odata.bind": "https://graph.microsoft.com/v1.0/print/printers/{printerId}",
  "allowAllUsers": false
}
```

### <a name="response"></a><span data-ttu-id="0d3bd-155">响应</span><span class="sxs-lookup"><span data-stu-id="0d3bd-155">Response</span></span>
<span data-ttu-id="0d3bd-156">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="0d3bd-156">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "PrinterShare Name",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
  "allowAllUsers": false,
  "status": {
    "state": "stopped",
    "details": ["disconnected"],
    "description": ""
  }
}
```

