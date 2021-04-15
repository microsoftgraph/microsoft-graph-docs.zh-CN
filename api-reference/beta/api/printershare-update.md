---
title: 更新 printershare
description: 更新打印机共享的属性。 此方法可用于"交换"打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 81f5f9e6742ad19ea6d9966f92729876a1eb95eb
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766404"
---
# <a name="update-printershare"></a><span data-ttu-id="a7e38-104">更新 printershare</span><span class="sxs-lookup"><span data-stu-id="a7e38-104">Update printershare</span></span>

<span data-ttu-id="a7e38-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="a7e38-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="a7e38-106">更新打印机共享的属性。</span><span class="sxs-lookup"><span data-stu-id="a7e38-106">Update the properties of a printer share.</span></span> <span data-ttu-id="a7e38-107">此方法可用于交换 [打印机](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="a7e38-107">This method can be used to swap [printers](../resources/printer.md).</span></span>

<span data-ttu-id="a7e38-108">例如，如果物理打印机设备中断，管理员可以注册新的打印机设备，并更新此[](../resources/printer.md) [printerShare](../resources/printerShare.md)以指向新打印机，而无需用户执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="a7e38-108">For example, if a physical printer device breaks, an administrator can register a new [printer](../resources/printer.md) device and update this [printerShare](../resources/printerShare.md) to point to the new printer without requiring users to take any action.</span></span>

## <a name="permissions"></a><span data-ttu-id="a7e38-109">权限</span><span class="sxs-lookup"><span data-stu-id="a7e38-109">Permissions</span></span>
<span data-ttu-id="a7e38-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a7e38-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="a7e38-112">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="a7e38-112">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription.</span></span> <span data-ttu-id="a7e38-113">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="a7e38-113">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="a7e38-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="a7e38-114">Permission type</span></span> | <span data-ttu-id="a7e38-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a7e38-115">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="a7e38-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a7e38-116">Delegated (work or school account)</span></span>| <span data-ttu-id="a7e38-117">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a7e38-117">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="a7e38-118">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a7e38-118">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a7e38-119">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7e38-119">Not Supported.</span></span>|
|<span data-ttu-id="a7e38-120">Application</span><span class="sxs-lookup"><span data-stu-id="a7e38-120">Application</span></span>|<span data-ttu-id="a7e38-121">不支持。</span><span class="sxs-lookup"><span data-stu-id="a7e38-121">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a7e38-122">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a7e38-122">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/shares/{id}
```

## <a name="request-headers"></a><span data-ttu-id="a7e38-123">请求标头</span><span class="sxs-lookup"><span data-stu-id="a7e38-123">Request headers</span></span>
| <span data-ttu-id="a7e38-124">名称</span><span class="sxs-lookup"><span data-stu-id="a7e38-124">Name</span></span>       | <span data-ttu-id="a7e38-125">说明</span><span class="sxs-lookup"><span data-stu-id="a7e38-125">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="a7e38-126">Authorization</span><span class="sxs-lookup"><span data-stu-id="a7e38-126">Authorization</span></span> | <span data-ttu-id="a7e38-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="a7e38-p105">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="a7e38-129">Content-type</span><span class="sxs-lookup"><span data-stu-id="a7e38-129">Content-type</span></span>  | <span data-ttu-id="a7e38-p106">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="a7e38-p106">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="a7e38-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="a7e38-132">Request body</span></span>
<span data-ttu-id="a7e38-133">在请求正文中，提供相关 printer [的值共享](../resources/printershare.md) 应更新的字段。</span><span class="sxs-lookup"><span data-stu-id="a7e38-133">In the request body, supply the values for relevant [printerShare](../resources/printershare.md) fields that should be updated.</span></span> <span data-ttu-id="a7e38-134">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="a7e38-134">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="a7e38-135">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="a7e38-135">For best performance, don't include existing values that haven't changed.</span></span>

<span data-ttu-id="a7e38-136">可以更新以下属性：</span><span class="sxs-lookup"><span data-stu-id="a7e38-136">Following properties can be updated:</span></span> 

| <span data-ttu-id="a7e38-137">属性</span><span class="sxs-lookup"><span data-stu-id="a7e38-137">Property</span></span>     | <span data-ttu-id="a7e38-138">类型</span><span class="sxs-lookup"><span data-stu-id="a7e38-138">Type</span></span>        | <span data-ttu-id="a7e38-139">说明</span><span class="sxs-lookup"><span data-stu-id="a7e38-139">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="a7e38-140">printer</span><span class="sxs-lookup"><span data-stu-id="a7e38-140">printer</span></span>|<span data-ttu-id="a7e38-141">microsoft.graph.printer</span><span class="sxs-lookup"><span data-stu-id="a7e38-141">microsoft.graph.printer</span></span>|<span data-ttu-id="a7e38-142">此打印机共享相关的打印机。</span><span class="sxs-lookup"><span data-stu-id="a7e38-142">The printer that this printer share is related to.</span></span> <span data-ttu-id="a7e38-143">使用 `printer@odata.bind` 以下示例中所示的语法更新与此打印机共享关联的打印机。</span><span class="sxs-lookup"><span data-stu-id="a7e38-143">Use the `printer@odata.bind` syntax as shown in the following example to update which printer this printer share is associated with.</span></span>|
|<span data-ttu-id="a7e38-144">displayName</span><span class="sxs-lookup"><span data-stu-id="a7e38-144">displayName</span></span>|<span data-ttu-id="a7e38-145">String</span><span class="sxs-lookup"><span data-stu-id="a7e38-145">String</span></span>|<span data-ttu-id="a7e38-146">打印客户端应显示的打印机共享的名称。</span><span class="sxs-lookup"><span data-stu-id="a7e38-146">The name of the printer share that print clients should display.</span></span>|
|<span data-ttu-id="a7e38-147">allowAllUsers</span><span class="sxs-lookup"><span data-stu-id="a7e38-147">allowAllUsers</span></span>|<span data-ttu-id="a7e38-148">Boolean</span><span class="sxs-lookup"><span data-stu-id="a7e38-148">Boolean</span></span>| <span data-ttu-id="a7e38-149">如果为 true，将授予所有用户和组对此打印机共享的访问权限。</span><span class="sxs-lookup"><span data-stu-id="a7e38-149">If true, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="a7e38-150">这将取代 allowedUsers 和 allowedGroups 导航属性定义的允许列表。</span><span class="sxs-lookup"><span data-stu-id="a7e38-150">This supersedes the allow lists defined by the allowedUsers and allowedGroups navigation properties.</span></span>|

## <a name="response"></a><span data-ttu-id="a7e38-151">响应</span><span class="sxs-lookup"><span data-stu-id="a7e38-151">Response</span></span>
<span data-ttu-id="a7e38-152">如果成功，此方法在响应 `200 OK` 正文中返回 响应代码和更新的 [printerShare](../resources/printershare.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="a7e38-152">If successful, this method returns a `200 OK` response code and an updated [printerShare](../resources/printershare.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="a7e38-153">示例</span><span class="sxs-lookup"><span data-stu-id="a7e38-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="a7e38-154">请求</span><span class="sxs-lookup"><span data-stu-id="a7e38-154">Request</span></span>
<span data-ttu-id="a7e38-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="a7e38-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="a7e38-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="a7e38-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_printershare"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/shares/{id}
Content-type: application/json
Content-length: 109

{
  "displayName": "ShareName",
  "allowAllUsers": true,
  "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}"
}
```
# <a name="c"></a>[<span data-ttu-id="a7e38-157">C#</span><span class="sxs-lookup"><span data-stu-id="a7e38-157">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-printershare-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="a7e38-158">JavaScript</span><span class="sxs-lookup"><span data-stu-id="a7e38-158">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-printershare-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="a7e38-159">Objective-C</span><span class="sxs-lookup"><span data-stu-id="a7e38-159">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-printershare-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="a7e38-160">Java</span><span class="sxs-lookup"><span data-stu-id="a7e38-160">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-printershare-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---

##### <a name="response"></a><span data-ttu-id="a7e38-161">响应</span><span class="sxs-lookup"><span data-stu-id="a7e38-161">Response</span></span>
<span data-ttu-id="a7e38-162">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="a7e38-162">The following is an example of the response.</span></span>
><span data-ttu-id="a7e38-p110">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="a7e38-p110">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 225

{
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "displayName": "ShareName",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z",
  "isAcceptingJobs": true,
  "allowAllUsers": true,
  "status": {
    "state": "stopped",
    "details": ["disconnected"],
    "description": ""
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update printershare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
