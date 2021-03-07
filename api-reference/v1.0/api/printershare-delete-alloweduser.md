---
title: 从 printerShare 中删除 allowedUser
description: 撤消指定用户向关联的打印机共享提交打印作业的访问权限。
author: nilakhan
localization_priority: Normal
ms.prod: cloud-printing
doc_type: apiPageType
ms.openlocfilehash: 540fea358367e6d0daa025ccc005df551ba151e2
ms.sourcegitcommit: 3edf187fe4b42f81c09610782671776a27161126
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/06/2021
ms.locfileid: "50517168"
---
# <a name="delete-alloweduser-from-printershare"></a><span data-ttu-id="71aa1-103">从 printerShare 中删除 allowedUser</span><span class="sxs-lookup"><span data-stu-id="71aa1-103">Delete allowedUser from printerShare</span></span>

<span data-ttu-id="71aa1-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="71aa1-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [cloudprinting-pricing-disclaimer](../../includes/cloudprinting-pricing-disclaimer.md)]

<span data-ttu-id="71aa1-105">撤销指定用户向关联的 [printerShare](../resources/printershare.md)提交打印作业的访问权限。</span><span class="sxs-lookup"><span data-stu-id="71aa1-105">Revoke the specified user's access to submit print jobs to the associated [printerShare](../resources/printershare.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="71aa1-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="71aa1-106">Permissions</span></span>
<span data-ttu-id="71aa1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="71aa1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="71aa1-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="71aa1-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="71aa1-110">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="71aa1-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="71aa1-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="71aa1-111">Permission type</span></span> | <span data-ttu-id="71aa1-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="71aa1-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="71aa1-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="71aa1-113">Delegated (work or school account)</span></span>| <span data-ttu-id="71aa1-114">PrinterShare.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="71aa1-114">PrinterShare.ReadWrite.All</span></span> |
|<span data-ttu-id="71aa1-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="71aa1-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="71aa1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="71aa1-116">Not Supported.</span></span>|
|<span data-ttu-id="71aa1-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="71aa1-117">Application</span></span>|<span data-ttu-id="71aa1-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="71aa1-118">Not Supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="71aa1-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="71aa1-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
DELETE /print/printerShare/{printerShareId}/allowedUsers/{userId}/$ref
```
## <a name="request-headers"></a><span data-ttu-id="71aa1-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="71aa1-120">Request headers</span></span>
| <span data-ttu-id="71aa1-121">名称</span><span class="sxs-lookup"><span data-stu-id="71aa1-121">Name</span></span>          | <span data-ttu-id="71aa1-122">说明</span><span class="sxs-lookup"><span data-stu-id="71aa1-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="71aa1-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="71aa1-123">Authorization</span></span> | <span data-ttu-id="71aa1-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="71aa1-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="71aa1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="71aa1-126">Request body</span></span>
<span data-ttu-id="71aa1-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="71aa1-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="71aa1-128">响应</span><span class="sxs-lookup"><span data-stu-id="71aa1-128">Response</span></span>
<span data-ttu-id="71aa1-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="71aa1-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="71aa1-131">示例</span><span class="sxs-lookup"><span data-stu-id="71aa1-131">Example</span></span>
### <a name="request"></a><span data-ttu-id="71aa1-132">请求</span><span class="sxs-lookup"><span data-stu-id="71aa1-132">Request</span></span>
<span data-ttu-id="71aa1-133">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="71aa1-133">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "delete_alloweduser"
}-->
```http
DELETE https://graph.microsoft.com/v1.0/print/printerShare/{printerShareId}/allowedUsers/{userId}/$ref
```

### <a name="response"></a><span data-ttu-id="71aa1-134">响应</span><span class="sxs-lookup"><span data-stu-id="71aa1-134">Response</span></span>
<span data-ttu-id="71aa1-135">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="71aa1-135">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
