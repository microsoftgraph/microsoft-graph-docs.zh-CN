---
title: 打印机： restoreFactoryDefaults
description: 重置打印机的默认设置。
author: braedenp-msft
localization_priority: Normal
ms.prod: universal-print
doc_type: apiPageType
ms.openlocfilehash: 9bae7ed31a9ac73fdda0f576b47129a888190811
ms.sourcegitcommit: 3b9eb50b790d952c7f350433ef7531d5e6d4b963
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/22/2020
ms.locfileid: "48731104"
---
# <a name="printer-restorefactorydefaults"></a><span data-ttu-id="b13fb-103">打印机： restoreFactoryDefaults</span><span class="sxs-lookup"><span data-stu-id="b13fb-103">printer: restoreFactoryDefaults</span></span>

<span data-ttu-id="b13fb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b13fb-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b13fb-105">将 [打印机](../resources/printer.md)的设置还原为出厂设置。</span><span class="sxs-lookup"><span data-stu-id="b13fb-105">Restore a [printer](../resources/printer.md)'s settings to the factory settings.</span></span>

## <a name="permissions"></a><span data-ttu-id="b13fb-106">权限</span><span class="sxs-lookup"><span data-stu-id="b13fb-106">Permissions</span></span>
<span data-ttu-id="b13fb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b13fb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

<span data-ttu-id="b13fb-109">若要使用通用打印服务，用户或应用的租户必须具有活动的通用打印订阅，以及下表中列出的权限。</span><span class="sxs-lookup"><span data-stu-id="b13fb-109">To use the Universal Print service, the user or app's tenant must have an active Universal Print subscription, in addition to the permissions listed in the following table.</span></span> <span data-ttu-id="b13fb-110">登录用户必须是 [打印机管理员](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator)。</span><span class="sxs-lookup"><span data-stu-id="b13fb-110">The signed in user must be a [Printer Administrator](/azure/active-directory/users-groups-roles/directory-assign-admin-roles#printer-administrator).</span></span>

|<span data-ttu-id="b13fb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="b13fb-111">Permission type</span></span> | <span data-ttu-id="b13fb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b13fb-112">Permissions (from least to most privileged)</span></span> |
|:---------------|:--------------------------------------------|
|<span data-ttu-id="b13fb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b13fb-113">Delegated (work or school account)</span></span>| <span data-ttu-id="b13fb-114">完全控制和所有打印机。</span><span class="sxs-lookup"><span data-stu-id="b13fb-114">Printer.ReadWrite.All, Printer.FullControl.All</span></span> |
|<span data-ttu-id="b13fb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b13fb-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="b13fb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b13fb-116">Not Supported.</span></span>|
|<span data-ttu-id="b13fb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="b13fb-117">Application</span></span>| <span data-ttu-id="b13fb-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="b13fb-118">Not Supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="b13fb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b13fb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /print/printers/{id}/restoreFactoryDefaults
```
## <a name="request-headers"></a><span data-ttu-id="b13fb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="b13fb-120">Request headers</span></span>
| <span data-ttu-id="b13fb-121">名称</span><span class="sxs-lookup"><span data-stu-id="b13fb-121">Name</span></span>          | <span data-ttu-id="b13fb-122">说明</span><span class="sxs-lookup"><span data-stu-id="b13fb-122">Description</span></span>   |
|:--------------|:--------------|
| <span data-ttu-id="b13fb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="b13fb-123">Authorization</span></span> | <span data-ttu-id="b13fb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b13fb-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b13fb-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="b13fb-126">Request body</span></span>
<span data-ttu-id="b13fb-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b13fb-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b13fb-128">响应</span><span class="sxs-lookup"><span data-stu-id="b13fb-128">Response</span></span>
<span data-ttu-id="b13fb-p104">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="b13fb-p104">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="b13fb-131">示例</span><span class="sxs-lookup"><span data-stu-id="b13fb-131">Example</span></span>
<span data-ttu-id="b13fb-132">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b13fb-132">The following example shows how to call this API.</span></span>
### <a name="request"></a><span data-ttu-id="b13fb-133">请求</span><span class="sxs-lookup"><span data-stu-id="b13fb-133">Request</span></span>
<span data-ttu-id="b13fb-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="b13fb-134">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "printer-restorefactorydefaults"
}-->
```http
POST https://graph.microsoft.com/beta/print/printers/{id}/restoreFactoryDefaults
```

### <a name="response"></a><span data-ttu-id="b13fb-135">响应</span><span class="sxs-lookup"><span data-stu-id="b13fb-135">Response</span></span>
<span data-ttu-id="b13fb-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b13fb-136">The following is an example of the response.</span></span> 
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
  "description": "printer: restoreFactoryDefaults",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
