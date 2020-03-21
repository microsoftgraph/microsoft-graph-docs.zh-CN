---
title: 创建 allowedGroup
description: 向指定的组授予向关联打印机提交打印作业的权限。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 58fdb75eb7e4f8e87691f7f11eaf7b65d9a06b91
ms.sourcegitcommit: 7baf4847486885edf08ead533c76503cd31a98a4
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/21/2020
ms.locfileid: "42895685"
---
# <a name="create-allowedgroup"></a><span data-ttu-id="ed359-103">创建 allowedGroup</span><span class="sxs-lookup"><span data-stu-id="ed359-103">Create allowedGroup</span></span>

<span data-ttu-id="ed359-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="ed359-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ed359-105">向指定的组授予向关联[打印机](../resources/printer.md)提交**打印作业**的权限。</span><span class="sxs-lookup"><span data-stu-id="ed359-105">Grant the specified group access to submit **print jobs** to the associated [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ed359-106">权限</span><span class="sxs-lookup"><span data-stu-id="ed359-106">Permissions</span></span>
<span data-ttu-id="ed359-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ed359-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="ed359-109">除了以下权限之外，用户的租户还必须具有活动的通用打印订阅。</span><span class="sxs-lookup"><span data-stu-id="ed359-109">In addition to the following permissions, the user's tenant must have an active Universal Print subscription.</span></span>

|<span data-ttu-id="ed359-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="ed359-110">Permission type</span></span> | <span data-ttu-id="ed359-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ed359-111">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="ed359-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ed359-112">Delegated (work or school account)</span></span>| <span data-ttu-id="ed359-113">已阅读的用户。所有</span><span class="sxs-lookup"><span data-stu-id="ed359-113">Users.Read.All</span></span> |
|<span data-ttu-id="ed359-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ed359-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ed359-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed359-115">Not Supported.</span></span>|
|<span data-ttu-id="ed359-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="ed359-116">Application</span></span>|<span data-ttu-id="ed359-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="ed359-117">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ed359-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ed359-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/allowedGroups/$ref
```
## <a name="request-headers"></a><span data-ttu-id="ed359-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="ed359-119">Request headers</span></span>
| <span data-ttu-id="ed359-120">名称</span><span class="sxs-lookup"><span data-stu-id="ed359-120">Name</span></span>          | <span data-ttu-id="ed359-121">说明</span><span class="sxs-lookup"><span data-stu-id="ed359-121">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="ed359-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ed359-122">Authorization</span></span> | <span data-ttu-id="ed359-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ed359-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="ed359-125">Content-type</span><span class="sxs-lookup"><span data-stu-id="ed359-125">Content-type</span></span>  | <span data-ttu-id="ed359-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="ed359-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="ed359-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="ed359-128">Request body</span></span>
<span data-ttu-id="ed359-129">在请求正文中，通过使用`@odata.id`格式提供对组实体的引用，如下面的示例所示。</span><span class="sxs-lookup"><span data-stu-id="ed359-129">In the request body, supply a reference to a group entity by using the `@odata.id` format, as shown in the following example.</span></span>

## <a name="response"></a><span data-ttu-id="ed359-130">响应</span><span class="sxs-lookup"><span data-stu-id="ed359-130">Response</span></span>
<span data-ttu-id="ed359-131">如果成功，此方法返回 `201 Created` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="ed359-131">If successful, this method returns a `201 Created` response code.</span></span>

## <a name="example"></a><span data-ttu-id="ed359-132">示例</span><span class="sxs-lookup"><span data-stu-id="ed359-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ed359-133">请求</span><span class="sxs-lookup"><span data-stu-id="ed359-133">Request</span></span>
<span data-ttu-id="ed359-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="ed359-134">The following is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_allowedgroup_from_printers"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/allowedGroups/$ref
Content-type: application/json
Content-length: 67

{
  "@odata.id": "https://graph.microsoft.com/beta/groups/{id}"
}
```
<span data-ttu-id="ed359-135">在请求正文中，通过在 JSON 正文的`@odata.id`字段中包含组的 MICROSOFT Graph URI，提供对组实体的引用。</span><span class="sxs-lookup"><span data-stu-id="ed359-135">In the request body, supply a reference to a group entity by including the group's Microsoft Graph URI in the `@odata.id` field of the JSON body.</span></span>

##### <a name="response"></a><span data-ttu-id="ed359-136">响应</span><span class="sxs-lookup"><span data-stu-id="ed359-136">Response</span></span>
<span data-ttu-id="ed359-137">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="ed359-137">The following is an example of the response.</span></span> 
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.None"
} -->
```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create allowedGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->