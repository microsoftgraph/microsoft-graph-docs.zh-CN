---
title: 刷新会话
description: '使用此 API 刷新现有的工作簿会话。 '
author: lumine2008
localization_priority: Normal
ms.openlocfilehash: 2f4d454214d2f21d1f6447ee224f3013cebb9078
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27822335"
---
# <a name="refresh-session"></a><span data-ttu-id="271e1-103">刷新会话</span><span class="sxs-lookup"><span data-stu-id="271e1-103">Refresh Session</span></span>

<span data-ttu-id="271e1-104">使用此 API 刷新现有的工作簿会话。</span><span class="sxs-lookup"><span data-stu-id="271e1-104">Use this API to refresh an existing workbook session.</span></span> 

## <a name="permissions"></a><span data-ttu-id="271e1-105">权限</span><span class="sxs-lookup"><span data-stu-id="271e1-105">Permissions</span></span>
<span data-ttu-id="271e1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="271e1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="271e1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="271e1-108">Permission type</span></span>      | <span data-ttu-id="271e1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="271e1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="271e1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="271e1-110">Delegated (work or school account)</span></span> | <span data-ttu-id="271e1-111">Files.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="271e1-111">Files.ReadWrite</span></span>    |
|<span data-ttu-id="271e1-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="271e1-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="271e1-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="271e1-113">Not supported.</span></span>    |
|<span data-ttu-id="271e1-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="271e1-114">Application</span></span> | <span data-ttu-id="271e1-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="271e1-115">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="271e1-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="271e1-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /workbook/refreshSession
workbook-session-id: {session-id}
```
## <a name="request-headers"></a><span data-ttu-id="271e1-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="271e1-117">Request headers</span></span>
| <span data-ttu-id="271e1-118">名称</span><span class="sxs-lookup"><span data-stu-id="271e1-118">Name</span></span>       | <span data-ttu-id="271e1-119">说明</span><span class="sxs-lookup"><span data-stu-id="271e1-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="271e1-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="271e1-120">Authorization</span></span>  | <span data-ttu-id="271e1-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="271e1-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="271e1-123">workbook-session-id</span><span class="sxs-lookup"><span data-stu-id="271e1-123">workbook-session-id</span></span> | <span data-ttu-id="271e1-124">要刷新的工作簿会话 ID</span><span class="sxs-lookup"><span data-stu-id="271e1-124">Workbook session Id to be refreshed</span></span> |

## <a name="request-body"></a><span data-ttu-id="271e1-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="271e1-125">Request body</span></span>
<span data-ttu-id="271e1-126">此 API 不需要任何请求正文。</span><span class="sxs-lookup"><span data-stu-id="271e1-126">This API does not require any request body.</span></span>

## <a name="response"></a><span data-ttu-id="271e1-127">响应</span><span class="sxs-lookup"><span data-stu-id="271e1-127">Response</span></span>

<span data-ttu-id="271e1-128">如果成功，此方法返回 `204 No Content` 响应代码。</span><span class="sxs-lookup"><span data-stu-id="271e1-128">If successful, this method returns `204 No Content` response code.</span></span>

## <a name="example"></a><span data-ttu-id="271e1-129">示例</span><span class="sxs-lookup"><span data-stu-id="271e1-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="271e1-130">请求</span><span class="sxs-lookup"><span data-stu-id="271e1-130">Request</span></span>
<span data-ttu-id="271e1-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="271e1-131">Here is an example of the request.</span></span>
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

<span data-ttu-id="271e1-132">请注意，workbook-session-id 标头是必需的。</span><span class="sxs-lookup"><span data-stu-id="271e1-132">Note that workbook-session-id header is required.</span></span> 


##### <a name="response"></a><span data-ttu-id="271e1-133">响应</span><span class="sxs-lookup"><span data-stu-id="271e1-133">Response</span></span>
<span data-ttu-id="271e1-134">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="271e1-134">Here is an example of the response.</span></span> 

<!-- {
  "blockType": "response",
  "truncated": true
} -->
```http
HTTP/1.1 204 No Content
```
