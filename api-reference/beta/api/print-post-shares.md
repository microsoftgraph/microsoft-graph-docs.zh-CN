---
title: 创建 printerShare
description: 为指定的打印机创建新的打印机共享。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: b5617bcc02fa705c100aeeb54c440f7d4270721b
ms.sourcegitcommit: 412507a3c3a8e407fcc43b7cd227d4db35791f58
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2021
ms.locfileid: "51766495"
---
# <a name="create-printershare"></a><span data-ttu-id="7883d-103">创建 printerShare</span><span class="sxs-lookup"><span data-stu-id="7883d-103">Create printerShare</span></span>

<span data-ttu-id="7883d-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="7883d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7883d-105">新建 **printerShare** for the specified [printer](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="7883d-105">Create a new **printerShare** for the specified [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7883d-106">权限</span><span class="sxs-lookup"><span data-stu-id="7883d-106">Permissions</span></span>
<span data-ttu-id="7883d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7883d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="7883d-109">若要使用通用打印服务，除了下表中列出的权限之外，用户或应用的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="7883d-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="7883d-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="7883d-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="7883d-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7883d-111">Permission type</span></span> | <span data-ttu-id="7883d-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7883d-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="7883d-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7883d-113">Delegated (work or school account)</span></span>| <span data-ttu-id="7883d-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7883d-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="7883d-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7883d-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7883d-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7883d-116">Not Supported.</span></span>|
|<span data-ttu-id="7883d-117">Application</span><span class="sxs-lookup"><span data-stu-id="7883d-117">Application</span></span>|<span data-ttu-id="7883d-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="7883d-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7883d-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7883d-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/shares
```
## <a name="request-headers"></a><span data-ttu-id="7883d-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="7883d-120">Request headers</span></span>
| <span data-ttu-id="7883d-121">名称</span><span class="sxs-lookup"><span data-stu-id="7883d-121">Name</span></span>          | <span data-ttu-id="7883d-122">说明</span><span class="sxs-lookup"><span data-stu-id="7883d-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="7883d-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="7883d-123">Authorization</span></span> | <span data-ttu-id="7883d-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7883d-p103">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7883d-126">Content-type</span><span class="sxs-lookup"><span data-stu-id="7883d-126">Content-type</span></span>  | <span data-ttu-id="7883d-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="7883d-p104">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="7883d-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="7883d-129">Request body</span></span>
<span data-ttu-id="7883d-130">在请求正文中，提供 [printerShare](../resources/printershare.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7883d-130">In the request body, supply a JSON representation of the [printerShare](../resources/printershare.md) object.</span></span>

<span data-ttu-id="7883d-131">下表显示创建 [printerShare](../resources/printershare.md)时提供的属性。</span><span class="sxs-lookup"><span data-stu-id="7883d-131">The following table shows the properties that can be provided when you create the [printerShare](../resources/printershare.md).</span></span>

|<span data-ttu-id="7883d-132">属性</span><span class="sxs-lookup"><span data-stu-id="7883d-132">Property</span></span>|<span data-ttu-id="7883d-133">类型</span><span class="sxs-lookup"><span data-stu-id="7883d-133">Type</span></span>|<span data-ttu-id="7883d-134">说明</span><span class="sxs-lookup"><span data-stu-id="7883d-134">Description</span></span>|<span data-ttu-id="7883d-135">是否必需？</span><span class="sxs-lookup"><span data-stu-id="7883d-135">Required?</span></span>|
|:---|:---|:---|:---|
|<span data-ttu-id="7883d-136">printer</span><span class="sxs-lookup"><span data-stu-id="7883d-136">printer</span></span>|<span data-ttu-id="7883d-137">microsoft.graph.printer</span><span class="sxs-lookup"><span data-stu-id="7883d-137">microsoft.graph.printer</span></span>|<span data-ttu-id="7883d-138">此打印机共享相关的打印机。</span><span class="sxs-lookup"><span data-stu-id="7883d-138">The printer that this printer share is related to.</span></span> <span data-ttu-id="7883d-139">使用 `printer@odata.bind` 以下示例中所示的语法。</span><span class="sxs-lookup"><span data-stu-id="7883d-139">Use the `printer@odata.bind` syntax as shown in the following example.</span></span>|<span data-ttu-id="7883d-140">是</span><span class="sxs-lookup"><span data-stu-id="7883d-140">Yes</span></span>|
|<span data-ttu-id="7883d-141">displayName</span><span class="sxs-lookup"><span data-stu-id="7883d-141">displayName</span></span>|<span data-ttu-id="7883d-142">String</span><span class="sxs-lookup"><span data-stu-id="7883d-142">String</span></span>|<span data-ttu-id="7883d-143">打印客户端应显示的打印机共享的名称。</span><span class="sxs-lookup"><span data-stu-id="7883d-143">The name of the printer share that print clients should display.</span></span> <span data-ttu-id="7883d-144">允许的最大长度为 50 个字符。</span><span class="sxs-lookup"><span data-stu-id="7883d-144">Maximum length allowed is 50 characters.</span></span>|<span data-ttu-id="7883d-145">是</span><span class="sxs-lookup"><span data-stu-id="7883d-145">Yes</span></span>|
|<span data-ttu-id="7883d-146">allowAllUsers</span><span class="sxs-lookup"><span data-stu-id="7883d-146">allowAllUsers</span></span>|<span data-ttu-id="7883d-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="7883d-147">Boolean</span></span>| <span data-ttu-id="7883d-148">如果为 true，将授予所有用户和组对此打印机共享的访问权限。</span><span class="sxs-lookup"><span data-stu-id="7883d-148">If true, all users and groups will be granted access to this printer share.</span></span> <span data-ttu-id="7883d-149">这将取代 allowedUsers 和 allowedGroups 导航属性定义的允许列表。</span><span class="sxs-lookup"><span data-stu-id="7883d-149">This supersedes the allow lists defined by the allowedUsers and allowedGroups navigation properties.</span></span>|<span data-ttu-id="7883d-150">否</span><span class="sxs-lookup"><span data-stu-id="7883d-150">No</span></span>|

## <a name="response"></a><span data-ttu-id="7883d-151">响应</span><span class="sxs-lookup"><span data-stu-id="7883d-151">Response</span></span>
<span data-ttu-id="7883d-152">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [printerShare](../resources/printershare.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="7883d-152">If successful, this method returns a `201 Created` response code and a [printerShare](../resources/printershare.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7883d-153">示例</span><span class="sxs-lookup"><span data-stu-id="7883d-153">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7883d-154">请求</span><span class="sxs-lookup"><span data-stu-id="7883d-154">Request</span></span>
<span data-ttu-id="7883d-155">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="7883d-155">The following is an example of the request.</span></span>

# <a name="http"></a>[<span data-ttu-id="7883d-156">HTTP</span><span class="sxs-lookup"><span data-stu-id="7883d-156">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_printershare_from_print"
}-->
```http
POST https://graph.microsoft.com/beta/print/shares
Content-type: application/json
Content-length: 114

{
  "name": "name-value",
  "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}"
}
```

---

##### <a name="response"></a><span data-ttu-id="7883d-157">响应</span><span class="sxs-lookup"><span data-stu-id="7883d-157">Response</span></span>
<span data-ttu-id="7883d-158">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="7883d-158">The following is an example of the response.</span></span>
><span data-ttu-id="7883d-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7883d-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.printerShare"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 233

{
    "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/shares/$entity",
    "id": "7361c7c1-ff07-4565-9897-bef6895a7d04",
    "displayName": "ShareName",
    "createdDateTime": "2020-02-04T00:00:00.0000000Z"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create printerShare",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
