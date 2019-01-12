---
title: 关闭会话
description: '使用此 API 关闭现有的工作簿会话。 '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: ff089565cc885cc5d70fbea238335b546b41f2ce
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27930661"
---
# <a name="close-session"></a><span data-ttu-id="550fa-103">关闭会话</span><span class="sxs-lookup"><span data-stu-id="550fa-103">Close Session</span></span>

<span data-ttu-id="550fa-104">使用此 API 关闭现有的工作簿会话。</span><span class="sxs-lookup"><span data-stu-id="550fa-104">Use this API to close an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="550fa-105">权限</span><span class="sxs-lookup"><span data-stu-id="550fa-105">Permissions</span></span>
<span data-ttu-id="550fa-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="550fa-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="550fa-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="550fa-108">Permission type</span></span>      | <span data-ttu-id="550fa-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="550fa-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="550fa-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="550fa-110">Delegated (work or school account)</span></span> | <span data-ttu-id="550fa-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="550fa-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="550fa-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="550fa-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="550fa-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="550fa-113">Not supported.</span></span>    |
|<span data-ttu-id="550fa-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="550fa-114">Application</span></span> | <span data-ttu-id="550fa-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="550fa-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="550fa-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="550fa-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/closeSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="550fa-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="550fa-117">Request headers</span></span>
| <span data-ttu-id="550fa-118">名称</span><span class="sxs-lookup"><span data-stu-id="550fa-118">Name</span></span>       | <span data-ttu-id="550fa-119">说明</span><span class="sxs-lookup"><span data-stu-id="550fa-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="550fa-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="550fa-120">Authorization</span></span>  | <span data-ttu-id="550fa-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="550fa-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="550fa-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="550fa-123">workbook-session-id</span></span> | <span data-ttu-id="550fa-124">要关闭的工作簿会话 ID</span><span class="sxs-lookup"><span data-stu-id="550fa-124">Workbook session Id to be closed</span></span> |

## <a name="request-body"></a><span data-ttu-id="550fa-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="550fa-125">Request body</span></span>
<span data-ttu-id="550fa-126">此 API 不需要任何请求正文。</span><span class="sxs-lookup"><span data-stu-id="550fa-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="550fa-127">响应</span><span class="sxs-lookup"><span data-stu-id="550fa-127">Response</span></span>

<span data-ttu-id="550fa-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="550fa-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="550fa-129">示例</span><span class="sxs-lookup"><span data-stu-id="550fa-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="550fa-130">请求</span><span class="sxs-lookup"><span data-stu-id="550fa-130">Request</span></span>
<span data-ttu-id="550fa-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="550fa-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "close_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/closeSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="550fa-132">请注意，workbook-session-id 标头是必需的。</span><span class="sxs-lookup"><span data-stu-id="550fa-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="550fa-133">响应</span><span class="sxs-lookup"><span data-stu-id="550fa-133">Response</span></span>
<span data-ttu-id="550fa-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="550fa-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
