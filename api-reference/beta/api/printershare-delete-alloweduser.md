---
title: 从 printerShare 中删除 allowedUser
description: 撤销指定用户的访问权限，以将打印作业提交到关联的打印机共享。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: b5a6c8028c84fa509e6cb21609ee105f0b29a1b2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48035524"
---
# <a name="delete-alloweduser-from-printershare"></a><span data-ttu-id="ecc07-103">从 printerShare 中删除 allowedUser</span><span class="sxs-lookup"><span data-stu-id="ecc07-103">Delete allowedUser from printerShare</span></span>

<span data-ttu-id="ecc07-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ecc07-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ecc07-105">撤销指定用户的访问权限，以将打印作业提交到关联的 [printerShare](../resources/printershare.md)。</span><span class="sxs-lookup"><span data-stu-id="ecc07-105">Revoke the specified user's access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ecc07-106">权限</span><span class="sxs-lookup"><span data-stu-id="ecc07-106">Permissions</span></span>
<span data-ttu-id="ecc07-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ecc07-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ecc07-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="ecc07-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="ecc07-110">登录用户必须是 [打印机管理员](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="ecc07-110">The signed in user must be a [Printer Administrator](https://docs.microsoft.com/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="ecc07-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="ecc07-111">Permission type</span></span> | <span data-ttu-id="ecc07-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ecc07-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ecc07-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ecc07-113">Delegated (work or school account)</span></span>| <span data-ttu-id="ecc07-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ecc07-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="ecc07-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ecc07-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ecc07-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="ecc07-116">Not Supported.</span></span>|
|<span data-ttu-id="ecc07-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="ecc07-117">Application</span></span>|<span data-ttu-id="ecc07-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="ecc07-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ecc07-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ecc07-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printerShare/{id}/allowedUsers/{id}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ecc07-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="ecc07-120">Request headers</span></span>
| <span data-ttu-id="ecc07-121">名称</span><span class="sxs-lookup"><span data-stu-id="ecc07-121">Name</span></span>          | <span data-ttu-id="ecc07-122">说明</span><span class="sxs-lookup"><span data-stu-id="ecc07-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ecc07-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ecc07-123">Authorization</span></span> | <span data-ttu-id="ecc07-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ecc07-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="ecc07-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ecc07-126">Request body</span></span>
<span data-ttu-id="ecc07-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ecc07-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ecc07-128">响应</span><span class="sxs-lookup"><span data-stu-id="ecc07-128">Response</span></span>
<span data-ttu-id="ecc07-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="ecc07-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ecc07-131">示例</span><span class="sxs-lookup"><span data-stu-id="ecc07-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="ecc07-132">请求</span><span class="sxs-lookup"><span data-stu-id="ecc07-132">Request</span></span>
<span data-ttu-id="ecc07-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ecc07-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_alloweduser"
}-->
```http
DELETE https://graph.microsoft.com/beta/print/printerShare/{id}/allowedUsers/{id}/$ref
```

### <a name="response"></a><span data-ttu-id="ecc07-134">响应</span><span class="sxs-lookup"><span data-stu-id="ecc07-134">Response</span></span>
<span data-ttu-id="ecc07-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ecc07-135">The following is an example of the response.</span></span>
><span data-ttu-id="ecc07-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="ecc07-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Delete allowedUser",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


