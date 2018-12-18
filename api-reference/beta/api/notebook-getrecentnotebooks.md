---
title: 笔记本：getRecentNotebooks
description: 获取登录用户访问的 recentNotebook 实例列表。
author: Jewan-microsoft
ms.openlocfilehash: 43141d7734a3427a3325a852d8185ebbee5d752c
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/18/2018
ms.locfileid: "27350496"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="b3b6a-103">笔记本：getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="b3b6a-103">notebook: getRecentNotebooks</span></span>

> <span data-ttu-id="b3b6a-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="b3b6a-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="b3b6a-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="b3b6a-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="b3b6a-106">获取登录用户访问的 [recentNotebook](../resources/recentnotebook.md) 实例列表。</span><span class="sxs-lookup"><span data-stu-id="b3b6a-106">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="b3b6a-107">权限</span><span class="sxs-lookup"><span data-stu-id="b3b6a-107">Permissions</span></span>
<span data-ttu-id="b3b6a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b3b6a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b3b6a-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="b3b6a-110">Permission type</span></span>      | <span data-ttu-id="b3b6a-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b3b6a-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b3b6a-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b3b6a-112">Delegated (work or school account)</span></span> | <span data-ttu-id="b3b6a-113">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3b6a-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="b3b6a-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b3b6a-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b3b6a-115">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b3b6a-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="b3b6a-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="b3b6a-116">Application</span></span> | <span data-ttu-id="b3b6a-117">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b3b6a-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b3b6a-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b3b6a-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/<id | userPrincipalName>/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="b3b6a-119">用户的 `<id | userPrincipalName>` 必须与用于发出请求的授权令牌中编码的用户一致。</span><span class="sxs-lookup"><span data-stu-id="b3b6a-119">The `<id | userPrincipalName>` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="b3b6a-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="b3b6a-120">Function parameters</span></span>

| <span data-ttu-id="b3b6a-121">参数</span><span class="sxs-lookup"><span data-stu-id="b3b6a-121">Parameter</span></span>    | <span data-ttu-id="b3b6a-122">Type</span><span class="sxs-lookup"><span data-stu-id="b3b6a-122">Type</span></span>   |<span data-ttu-id="b3b6a-123">说明</span><span class="sxs-lookup"><span data-stu-id="b3b6a-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b3b6a-124">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="b3b6a-124">includePersonalNotebooks</span></span>|<span data-ttu-id="b3b6a-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="b3b6a-125">Boolean</span></span>|<span data-ttu-id="b3b6a-126">添加用户拥有的笔记本。</span><span class="sxs-lookup"><span data-stu-id="b3b6a-126">Include notebooks owned by the user.</span></span> <span data-ttu-id="b3b6a-127">若要添加用户拥有的笔记本，请设置为 `true`；否则，设置为 `false`。</span><span class="sxs-lookup"><span data-stu-id="b3b6a-127">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="b3b6a-128">如果不添加 `includePersonalNotebooks` 参数，请求会返回 `400` 错误响应。</span><span class="sxs-lookup"><span data-stu-id="b3b6a-128">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="b3b6a-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="b3b6a-129">Request headers</span></span>
| <span data-ttu-id="b3b6a-130">Name</span><span class="sxs-lookup"><span data-stu-id="b3b6a-130">Name</span></span>       | <span data-ttu-id="b3b6a-131">说明</span><span class="sxs-lookup"><span data-stu-id="b3b6a-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b3b6a-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="b3b6a-132">Authorization</span></span>  | <span data-ttu-id="b3b6a-133">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b3b6a-133">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b3b6a-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="b3b6a-134">Request body</span></span>
<span data-ttu-id="b3b6a-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b3b6a-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b3b6a-136">响应</span><span class="sxs-lookup"><span data-stu-id="b3b6a-136">Response</span></span>
<span data-ttu-id="b3b6a-137">如果成功响应，则返回 `200 OK`，其中包含 **recentNotebooks** 的 JSON 集合。</span><span class="sxs-lookup"><span data-stu-id="b3b6a-137">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="b3b6a-138">示例</span><span class="sxs-lookup"><span data-stu-id="b3b6a-138">Example</span></span>
<span data-ttu-id="b3b6a-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b3b6a-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b3b6a-140">请求</span><span class="sxs-lookup"><span data-stu-id="b3b6a-140">Request</span></span>
<span data-ttu-id="b3b6a-141">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="b3b6a-141">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)
```

##### <a name="response"></a><span data-ttu-id="b3b6a-142">响应</span><span class="sxs-lookup"><span data-stu-id="b3b6a-142">Response</span></span>
<span data-ttu-id="b3b6a-143">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="b3b6a-143">The following example shows the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.notebook",
  "isCollection": true
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-Length: 1110

{
  "value":[
    {
      "name":"Personal Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDrive"
    },{
      "name":"Team Shared Notebook","lastAccessedTime":"timestamp","links":{
        "oneNoteClientUrl":{
          "href":"onenote:href-value"
        },"oneNoteWebUrl":{
          "href":"href-value"
        }
      },"sourceService":"OneDriveForBusiness"
    }
  ]
}
```
