---
title: 列出 printerShare 的 allowedGroups
description: 检索已被授予将打印作业提交到关联的打印机共享的权限的组列表。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 49555364c6ff923d746718ef37650130d85e7c30
ms.sourcegitcommit: 40947e6f4337c8c4193d85bb862e15f67263e1e7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/13/2021
ms.locfileid: "50771566"
---
# <a name="list-allowedgroups"></a><span data-ttu-id="2c7a1-103">列出 allowedGroups</span><span class="sxs-lookup"><span data-stu-id="2c7a1-103">List allowedGroups</span></span>
<span data-ttu-id="2c7a1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2c7a1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="2c7a1-105">检索已被授予向关联的 printerShare 提交打印作业的权限的组 [列表](../resources/printershare.md)。</span><span class="sxs-lookup"><span data-stu-id="2c7a1-105">Retrieve a list of groups that have been granted access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="2c7a1-106">权限</span><span class="sxs-lookup"><span data-stu-id="2c7a1-106">Permissions</span></span>
<span data-ttu-id="2c7a1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2c7a1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="2c7a1-109">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有授予 [列表](group-list.md) 组访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="2c7a1-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [List groups](group-list.md) access.</span></span> <span data-ttu-id="2c7a1-110">登录的用户必须是打印机 [管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="2c7a1-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="2c7a1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="2c7a1-111">Permission type</span></span> | <span data-ttu-id="2c7a1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2c7a1-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="2c7a1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2c7a1-113">Delegated (work or school account)</span></span>| <span data-ttu-id="2c7a1-114">PrinterShare.Read.All、PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="2c7a1-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="2c7a1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2c7a1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="2c7a1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c7a1-116">Not Supported.</span></span>|
|<span data-ttu-id="2c7a1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="2c7a1-117">Application</span></span>|<span data-ttu-id="2c7a1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="2c7a1-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="2c7a1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2c7a1-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares/{printerShareId}/allowedGroups
```

## <a name="request-headers"></a><span data-ttu-id="2c7a1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="2c7a1-120">Request headers</span></span>
|<span data-ttu-id="2c7a1-121">名称</span><span class="sxs-lookup"><span data-stu-id="2c7a1-121">Name</span></span>|<span data-ttu-id="2c7a1-122">说明</span><span class="sxs-lookup"><span data-stu-id="2c7a1-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="2c7a1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="2c7a1-123">Authorization</span></span>|<span data-ttu-id="2c7a1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2c7a1-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="2c7a1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2c7a1-126">Request body</span></span>
<span data-ttu-id="2c7a1-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2c7a1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2c7a1-128">响应</span><span class="sxs-lookup"><span data-stu-id="2c7a1-128">Response</span></span>

<span data-ttu-id="2c7a1-129">如果成功，此方法在响应正文中返回 响应代码和 `200 OK` [group](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="2c7a1-129">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="2c7a1-130">示例</span><span class="sxs-lookup"><span data-stu-id="2c7a1-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="2c7a1-131">请求</span><span class="sxs-lookup"><span data-stu-id="2c7a1-131">Request</span></span>

# <a name="http"></a>[<span data-ttu-id="2c7a1-132">HTTP</span><span class="sxs-lookup"><span data-stu-id="2c7a1-132">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "list_group"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedGroups
```
# <a name="c"></a>[<span data-ttu-id="2c7a1-133">C#</span><span class="sxs-lookup"><span data-stu-id="2c7a1-133">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/list-group-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="2c7a1-134">JavaScript</span><span class="sxs-lookup"><span data-stu-id="2c7a1-134">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/list-group-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="2c7a1-135">Objective-C</span><span class="sxs-lookup"><span data-stu-id="2c7a1-135">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/list-group-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="2c7a1-136">Java</span><span class="sxs-lookup"><span data-stu-id="2c7a1-136">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/list-group-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---



### <a name="response"></a><span data-ttu-id="2c7a1-137">响应</span><span class="sxs-lookup"><span data-stu-id="2c7a1-137">Response</span></span>
<span data-ttu-id="2c7a1-138">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="2c7a1-138">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "Collection(microsoft.graph.group)"
}
-->
``` http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#Collection(microsoft.graph.group)",
  "value": [
    {
      "id": "016b5565-3bbf-4067-b9ff-4d68167eb1a6",
      "displayName": "GroupName"
    }
  ]
}
```

