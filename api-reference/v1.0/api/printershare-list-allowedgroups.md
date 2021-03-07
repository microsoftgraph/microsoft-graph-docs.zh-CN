---
title: 列出 printerShare 的 allowedGroups
description: 检索已被授予将打印作业提交到关联的打印机共享的访问权限的组列表。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: a7254feef5bc0c320ab39404c7c7a2f9bc3ccd9c
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50516979"
---
# <a name="list-allowedgroups"></a><span data-ttu-id="e11ea-103">列出 allowedGroups</span><span class="sxs-lookup"><span data-stu-id="e11ea-103">List allowedGroups</span></span>
<span data-ttu-id="e11ea-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="e11ea-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="e11ea-105">检索已被授予将打印作业提交到关联的 [printerShare 的访问权限](../resources/printershare.md)的组列表。</span><span class="sxs-lookup"><span data-stu-id="e11ea-105">Retrieve a list of groups that have been granted access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="e11ea-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="e11ea-106">Permissions</span></span>
<span data-ttu-id="e11ea-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="e11ea-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="e11ea-109">除了以下权限之外，用户或应用的租户还必须具有活动的通用打印订阅，并且具有授予 [列表](group-list.md) 组访问权限的权限。</span><span class="sxs-lookup"><span data-stu-id="e11ea-109">In addition to the following permissions, the user or app's tenant must have an active Universal Print subscription and have a permission that grants [List groups](group-list.md) access.</span></span> <span data-ttu-id="e11ea-110">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="e11ea-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="e11ea-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="e11ea-111">Permission type</span></span> | <span data-ttu-id="e11ea-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="e11ea-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="e11ea-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="e11ea-113">Delegated (work or school account)</span></span>| <span data-ttu-id="e11ea-114">PrinterShare.Read.All、PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e11ea-114">PrinterShare.Read.All, PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="e11ea-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="e11ea-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e11ea-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="e11ea-116">Not Supported.</span></span>|
|<span data-ttu-id="e11ea-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="e11ea-117">Application</span></span>|<span data-ttu-id="e11ea-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="e11ea-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e11ea-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="e11ea-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
GET /print/shares/{printerShareId}/allowedGroups
```

## <a name="request-headers"></a><span data-ttu-id="e11ea-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="e11ea-120">Request headers</span></span>
|<span data-ttu-id="e11ea-121">名称</span><span class="sxs-lookup"><span data-stu-id="e11ea-121">Name</span></span>|<span data-ttu-id="e11ea-122">说明</span><span class="sxs-lookup"><span data-stu-id="e11ea-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="e11ea-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e11ea-123">Authorization</span></span>|<span data-ttu-id="e11ea-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="e11ea-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="e11ea-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="e11ea-126">Request body</span></span>
<span data-ttu-id="e11ea-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="e11ea-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="e11ea-128">响应</span><span class="sxs-lookup"><span data-stu-id="e11ea-128">Response</span></span>

<span data-ttu-id="e11ea-129">如果成功，此方法在响应正文中返回响应代码和 `200 OK` [组](../resources/group.md) 对象集合。</span><span class="sxs-lookup"><span data-stu-id="e11ea-129">If successful, this method returns a `200 OK` response code and a collection of [group](../resources/group.md) objects in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="e11ea-130">示例</span><span class="sxs-lookup"><span data-stu-id="e11ea-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="e11ea-131">请求</span><span class="sxs-lookup"><span data-stu-id="e11ea-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "list_group"
}
-->
``` http
GET https://graph.microsoft.com/v1.0/print/shares/{printerShareId}/allowedGroups
```


### <a name="response"></a><span data-ttu-id="e11ea-132">响应</span><span class="sxs-lookup"><span data-stu-id="e11ea-132">Response</span></span>
<span data-ttu-id="e11ea-133">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="e11ea-133">**Note:** The response object shown here might be shortened for readability.</span></span>
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

