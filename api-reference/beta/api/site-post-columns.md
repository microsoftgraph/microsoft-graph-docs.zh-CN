---
author: swapnil1993
ms.date: 08/30/2020
title: 在网站创建 columnDefinition
description: 创建网站栏。
localization_priority: Normal
doc_type: apiPageType
ms.prod: sites-and-lists
ms.openlocfilehash: 1404707dc2a98b4ac60e663fd25d595c977148f7
ms.sourcegitcommit: aa18eb8a9965f99cc97680808abba8df46f31ba5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/08/2021
ms.locfileid: "51638836"
---
# <a name="create-columndefinition-for-a-site"></a><span data-ttu-id="6b8e4-103">为网站创建 columnDefinition</span><span class="sxs-lookup"><span data-stu-id="6b8e4-103">Create columnDefinition for a site</span></span>
<span data-ttu-id="6b8e4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="6b8e4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]
<span data-ttu-id="6b8e4-105">为网站创建 [列][site] by specifying a [columnDefinition][columnDefinition] 。</span><span class="sxs-lookup"><span data-stu-id="6b8e4-105">Create a column for a [site][site] by specifying a [columnDefinition][columnDefinition].</span></span>

## <a name="permissions"></a><span data-ttu-id="6b8e4-106">权限</span><span class="sxs-lookup"><span data-stu-id="6b8e4-106">Permissions</span></span>

<span data-ttu-id="6b8e4-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/concepts/permissions_reference.md)。</span><span class="sxs-lookup"><span data-stu-id="6b8e4-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/concepts/permissions_reference.md).</span></span>

  

|<span data-ttu-id="6b8e4-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="6b8e4-109">Permission type</span></span> | <span data-ttu-id="6b8e4-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="6b8e4-110">Permissions (from least to most privileged)</span></span> |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="6b8e4-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="6b8e4-111">Delegated (work or school account)</span></span> | <span data-ttu-id="6b8e4-112">Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6b8e4-112">Sites.Manage.All, Sites.FullControl.All</span></span> |
|<span data-ttu-id="6b8e4-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="6b8e4-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="6b8e4-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="6b8e4-114">Not supported.</span></span> |
|<span data-ttu-id="6b8e4-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="6b8e4-115">Application</span></span> | <span data-ttu-id="6b8e4-116">Sites.Manage.All、Sites.FullControl.All</span><span class="sxs-lookup"><span data-stu-id="6b8e4-116">Sites.Manage.All, Sites.FullControl.All</span></span> |

  

## <a name="http-request"></a><span data-ttu-id="6b8e4-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="6b8e4-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
POST /sites/{site-id}/columns
```

## <a name="request-body"></a><span data-ttu-id="6b8e4-118">请求正文</span><span class="sxs-lookup"><span data-stu-id="6b8e4-118">Request body</span></span>

<span data-ttu-id="6b8e4-119">在请求正文中，提供要添加的 [columnDefinition 资源的][] JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6b8e4-119">In the request body, supply a JSON representation of the [columnDefinition][] resource to add.</span></span>  

## <a name="response"></a><span data-ttu-id="6b8e4-120">响应</span><span class="sxs-lookup"><span data-stu-id="6b8e4-120">Response</span></span>

<span data-ttu-id="6b8e4-121">如果成功，此方法在响应 `201 Created` 正文中返回 响应代码和 [columnDefinition][] 对象。</span><span class="sxs-lookup"><span data-stu-id="6b8e4-121">If successful, this method returns a `201 Created` response code and [columnDefinition][] object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="6b8e4-122">示例</span><span class="sxs-lookup"><span data-stu-id="6b8e4-122">Example</span></span>

### <a name="request"></a><span data-ttu-id="6b8e4-123">请求</span><span class="sxs-lookup"><span data-stu-id="6b8e4-123">Request</span></span>
<!-- { "blockType": "request" } -->
```http
POST https://graph.microsoft.com/beta/sites/{site-id}/columns
Content-Type: application/json

{
   "description":"test",
   "enforceUniqueValues":false,
   "hidden":false,
   "indexed":false,
   "name":"Title",
   "text":{
      "allowMultipleLines":false,
      "appendChangesToExistingText":false,
      "linesForEditing":0,
      "maxLength":255
   }
}
```

### <a name="response"></a><span data-ttu-id="6b8e4-124">响应</span><span class="sxs-lookup"><span data-stu-id="6b8e4-124">Response</span></span>

<!-- { "blockType": "response", "@type": "microsoft.graph.columnDefinition", "truncated": true } -->

  

```http
HTTP/1.1 201 Created
Content-type: application/json

{
   "description":"test",
   "displayName":"Title",
   "enforceUniqueValues":false,
   "hidden":false,
   "id":"99ddcf45-e2f7-4f17-82b0-6fba34445103",
   "indexed":false,
   "name":"Title",
   "text":{
      "allowMultipleLines":false,
      "appendChangesToExistingText":false,
      "linesForEditing":0,
      "maxLength":255
   }
}
```

  

[columnDefinition]: ../resources/columnDefinition.md
[site]: ../resources/site.md
  

