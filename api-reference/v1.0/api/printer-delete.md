---
title: 删除打印机
description: 删除 (注销) 打印机。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 2a1d1b91e5f3b68995a27021c0b2fc3eb39de939
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517185"
---
# <a name="delete-printer"></a><span data-ttu-id="06bbf-103">删除打印机</span><span class="sxs-lookup"><span data-stu-id="06bbf-103">Delete printer</span></span>
<span data-ttu-id="06bbf-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="06bbf-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="06bbf-105">删除 (注销) [打印机。](../resources/printer.md)</span><span class="sxs-lookup"><span data-stu-id="06bbf-105">Delete (unregister) a [printer](../resources/printer.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="06bbf-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="06bbf-106">Permissions</span></span>
<span data-ttu-id="06bbf-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="06bbf-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="06bbf-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="06bbf-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="06bbf-110">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="06bbf-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="06bbf-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="06bbf-111">Permission type</span></span> | <span data-ttu-id="06bbf-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="06bbf-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="06bbf-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="06bbf-113">Delegated (work or school account)</span></span>| <span data-ttu-id="06bbf-114">Printer.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="06bbf-114">Printer.FullControl.All</span></span> |
|<span data-ttu-id="06bbf-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="06bbf-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="06bbf-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="06bbf-116">Not Supported.</span></span>|
|<span data-ttu-id="06bbf-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="06bbf-117">Application</span></span>|<span data-ttu-id="06bbf-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="06bbf-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="06bbf-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="06bbf-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /print/printers/{printerId}
```

## <a name="request-headers"></a><span data-ttu-id="06bbf-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="06bbf-120">Request headers</span></span>
|<span data-ttu-id="06bbf-121">名称</span><span class="sxs-lookup"><span data-stu-id="06bbf-121">Name</span></span>|<span data-ttu-id="06bbf-122">说明</span><span class="sxs-lookup"><span data-stu-id="06bbf-122">Description</span></span>|
|:---|:---|
|<span data-ttu-id="06bbf-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="06bbf-123">Authorization</span></span>|<span data-ttu-id="06bbf-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="06bbf-p103">Bearer {token}. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="06bbf-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="06bbf-126">Request body</span></span>
<span data-ttu-id="06bbf-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="06bbf-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="06bbf-128">响应</span><span class="sxs-lookup"><span data-stu-id="06bbf-128">Response</span></span>

<span data-ttu-id="06bbf-129">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="06bbf-129">If successful, this method returns a `204 No Content` response code.</span></span>

## <a name="examples"></a><span data-ttu-id="06bbf-130">示例</span><span class="sxs-lookup"><span data-stu-id="06bbf-130">Examples</span></span>

### <a name="request"></a><span data-ttu-id="06bbf-131">请求</span><span class="sxs-lookup"><span data-stu-id="06bbf-131">Request</span></span>
<!-- {
  "blockType": "request",
  "name": "delete_printer"
}
-->
``` http
DELETE https://graph.microsoft.com/v1.0/print/printers/{printerId}
```


### <a name="response"></a><span data-ttu-id="06bbf-132">响应</span><span class="sxs-lookup"><span data-stu-id="06bbf-132">Response</span></span>
<!-- {
  "blockType": "response",
  "truncated": true
}
-->
``` http
HTTP/1.1 204 No Content
```

