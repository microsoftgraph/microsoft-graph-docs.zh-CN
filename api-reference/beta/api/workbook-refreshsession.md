---
title: 刷新会话
description: '使用此 API 刷新现有的工作簿会话。 '
author: lumine2008
localization_priority: Normal
ms.prod: excel
ms.openlocfilehash: 288f0b4b41841a6393af837f1b6e5c048dfae77e
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27977449"
---
# <a name="refresh-session"></a><span data-ttu-id="7cb70-103">刷新会话</span><span class="sxs-lookup"><span data-stu-id="7cb70-103">Refresh Session</span></span>

<span data-ttu-id="7cb70-104">使用此 API 刷新现有的工作簿会话。</span><span class="sxs-lookup"><span data-stu-id="7cb70-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="7cb70-105">权限</span><span class="sxs-lookup"><span data-stu-id="7cb70-105">Permissions</span></span>
<span data-ttu-id="7cb70-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7cb70-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cb70-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="7cb70-108">Permission type</span></span>      | <span data-ttu-id="7cb70-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7cb70-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cb70-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7cb70-110">Delegated (work or school account)</span></span> | <span data-ttu-id="7cb70-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="7cb70-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="7cb70-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7cb70-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cb70-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cb70-113">Not supported.</span></span>    |
|<span data-ttu-id="7cb70-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="7cb70-114">Application</span></span> | <span data-ttu-id="7cb70-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cb70-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7cb70-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7cb70-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="7cb70-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="7cb70-117">Request headers</span></span>
| <span data-ttu-id="7cb70-118">名称</span><span class="sxs-lookup"><span data-stu-id="7cb70-118">Name</span></span>       | <span data-ttu-id="7cb70-119">说明</span><span class="sxs-lookup"><span data-stu-id="7cb70-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="7cb70-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cb70-120">Authorization</span></span>  | <span data-ttu-id="7cb70-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="7cb70-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="7cb70-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="7cb70-123">workbook-session-id</span></span> | <span data-ttu-id="7cb70-124">要刷新的工作簿会话 ID</span><span class="sxs-lookup"><span data-stu-id="7cb70-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="7cb70-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="7cb70-125">Request body</span></span>
<span data-ttu-id="7cb70-126">此 API 不需要任何请求正文。</span><span class="sxs-lookup"><span data-stu-id="7cb70-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="7cb70-127">响应</span><span class="sxs-lookup"><span data-stu-id="7cb70-127">Response</span></span>

<span data-ttu-id="7cb70-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="7cb70-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="7cb70-129">示例</span><span class="sxs-lookup"><span data-stu-id="7cb70-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7cb70-130">请求</span><span class="sxs-lookup"><span data-stu-id="7cb70-130">Request</span></span>
<span data-ttu-id="7cb70-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="7cb70-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "refresh_excel_session"
}-->
```http
POST https://graph.microsoft.com/beta/me/drive/items/{id}/workbook/refreshSession
Content-type: application/json
workbook-session-id: {session-id}
Content-length: 0

{

}
```

<span data-ttu-id="7cb70-132">请注意，workbook-session-id 标头是必需的。</span><span class="sxs-lookup"><span data-stu-id="7cb70-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="7cb70-133">响应</span><span class="sxs-lookup"><span data-stu-id="7cb70-133">Response</span></span>
<span data-ttu-id="7cb70-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="7cb70-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
