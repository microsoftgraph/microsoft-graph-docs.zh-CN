---
title: 更新 printershare
description: 更新打印机共享的属性。 此方法可用于 "交换" 打印机。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 7326a37afd351fee6cce7c89663e65cb2aba5099
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895669"
---
# <a name="update-printershare"></a><span data-ttu-id="e49d8-104">更新 printershare</span><span class="sxs-lookup"><span data-stu-id="e49d8-104">Update printershare</span></span>

<span data-ttu-id="e49d8-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e49d8-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="e49d8-106">更新打印机共享的属性。</span><span class="sxs-lookup"><span data-stu-id="e49d8-106">Update the properties of a printer share.</span></span> <span data-ttu-id="e49d8-107">此方法可用于交换[打印机](../resources/printer.md)。</span><span class="sxs-lookup"><span data-stu-id="e49d8-107">This method can be used to swap [printers](../resources/printer.md).</span></span>

<span data-ttu-id="e49d8-108">例如，如果物理打印机设备断开，则管理员可以注册新的[打印机](../resources/printer.md)设备并更新此[printerShare](../resources/printerShare.md) ，以指向新的打印机，而无需用户执行任何操作。</span><span class="sxs-lookup"><span data-stu-id="e49d8-108">For example, if a physical printer device breaks, an administrator can register a new [printer](../resources/printer.md) device and update this [printerShare](../resources/printerShare.md) to point to the new printer without requiring users to take any action.</span></span>

## <a name="permissions"></a><span data-ttu-id="e49d8-109">权限</span><span class="sxs-lookup"><span data-stu-id="e49d8-109">Permissions</span></span>
<span data-ttu-id="e49d8-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e49d8-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e49d8-112">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="e49d8-112">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="e49d8-113">权限类型</span><span class="sxs-lookup"><span data-stu-id="e49d8-113">Permission type</span></span> | <span data-ttu-id="e49d8-114">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e49d8-114">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e49d8-115">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e49d8-115">Delegated (work or school account)</span></span>| <span data-ttu-id="e49d8-116">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="e49d8-116">Users.Read.All</span></span> |
|<span data-ttu-id="e49d8-117">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e49d8-117">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e49d8-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e49d8-118">Not Supported.</span></span>|
|<span data-ttu-id="e49d8-119">应用程序</span><span class="sxs-lookup"><span data-stu-id="e49d8-119">Application</span></span>|<span data-ttu-id="e49d8-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="e49d8-120">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e49d8-121">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e49d8-121">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /print/printerShares/{id}
```

## <a name="request-headers"></a><span data-ttu-id="e49d8-122">请求标头</span><span class="sxs-lookup"><span data-stu-id="e49d8-122">Request headers</span></span>
| <span data-ttu-id="e49d8-123">名称</span><span class="sxs-lookup"><span data-stu-id="e49d8-123">Name</span></span>       | <span data-ttu-id="e49d8-124">说明</span><span class="sxs-lookup"><span data-stu-id="e49d8-124">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="e49d8-125">Authorization</span><span class="sxs-lookup"><span data-stu-id="e49d8-125">Authorization</span></span> | <span data-ttu-id="e49d8-p104">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e49d8-p104">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="e49d8-128">Content-type</span><span class="sxs-lookup"><span data-stu-id="e49d8-128">Content-type</span></span>  | <span data-ttu-id="e49d8-p105">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="e49d8-p105">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e49d8-131">请求正文</span><span class="sxs-lookup"><span data-stu-id="e49d8-131">Request body</span></span>
<span data-ttu-id="e49d8-132">在请求正文中，提供应更新的相关[printerShare](../resources/printershare.md)字段的值。</span><span class="sxs-lookup"><span data-stu-id="e49d8-132">In the request body, supply the values for relevant [printerShare](../resources/printershare.md) fields that should be updated.</span></span> <span data-ttu-id="e49d8-133">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="e49d8-133">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="e49d8-134">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="e49d8-134">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="e49d8-135">属性</span><span class="sxs-lookup"><span data-stu-id="e49d8-135">Property</span></span>     | <span data-ttu-id="e49d8-136">类型</span><span class="sxs-lookup"><span data-stu-id="e49d8-136">Type</span></span>        | <span data-ttu-id="e49d8-137">说明</span><span class="sxs-lookup"><span data-stu-id="e49d8-137">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="e49d8-138">印刷</span><span class="sxs-lookup"><span data-stu-id="e49d8-138">printer</span></span>|<span data-ttu-id="e49d8-139">String</span><span class="sxs-lookup"><span data-stu-id="e49d8-139">String</span></span>|<span data-ttu-id="e49d8-140">与此打印机共享相关联的打印机。</span><span class="sxs-lookup"><span data-stu-id="e49d8-140">The printer that this printer share is related to.</span></span> <span data-ttu-id="e49d8-141">使用以下`printer@odata.bind`示例中所示的语法更新与该打印机共享相关联的打印机。</span><span class="sxs-lookup"><span data-stu-id="e49d8-141">Use the `printer@odata.bind` syntax as shown in the following example to update which printer this printer share is associated with.</span></span>|

><span data-ttu-id="e49d8-142">**注意：** 不支持更新打印机共享名称。</span><span class="sxs-lookup"><span data-stu-id="e49d8-142">**Note:** Updating the printer share name is not supported.</span></span>

## <a name="response"></a><span data-ttu-id="e49d8-143">响应</span><span class="sxs-lookup"><span data-stu-id="e49d8-143">Response</span></span>
<span data-ttu-id="e49d8-144">如果成功，此方法在响应`200 OK`正文中返回响应代码和更新的[printerShare](../resources/printershare.md)对象。</span><span class="sxs-lookup"><span data-stu-id="e49d8-144">If successful, this method returns a `200 OK` response code and an updated [printerShare](../resources/printershare.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="e49d8-145">示例</span><span class="sxs-lookup"><span data-stu-id="e49d8-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="e49d8-146">请求</span><span class="sxs-lookup"><span data-stu-id="e49d8-146">Request</span></span>
<span data-ttu-id="e49d8-147">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="e49d8-147">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_printershare"
}-->
```http
PATCH https://graph.microsoft.com/beta/print/printerShares/{id}
Content-type: application/json
Content-length: 109

{
  "name": "ShareName",
  "printer@odata.bind": "https://graph.microsoft.com/beta/print/printers/{id}"
}
```
##### <a name="response"></a><span data-ttu-id="e49d8-148">响应</span><span class="sxs-lookup"><span data-stu-id="e49d8-148">Response</span></span>
<span data-ttu-id="e49d8-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="e49d8-149">The following is an example of the response.</span></span>
><span data-ttu-id="e49d8-p108">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="e49d8-p108">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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
  "@odata.context": "https://graph.microsoft.com/beta/$metadata#print/printerShares/$entity",
  "id": "d837c17b-3296-4384-a053-828d56e10f50",
  "name": "ShareName",
  "createdDateTime": "2020-02-04T00:00:00.0000000Z"
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