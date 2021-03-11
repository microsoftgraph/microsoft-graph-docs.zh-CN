---
title: 笔记本：getRecentNotebooks
description: 获取登录用户访问的 recentNotebook 实例列表。
author: jewan-microsoft
localization_priority: Normal
ms.prod: onenote
doc_type: apiPageType
ms.openlocfilehash: 98cd3631ccf62d7ea20f7bfe5bf53a4101c5e6d0
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721711"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="b5c81-103">笔记本：getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="b5c81-103">notebook: getRecentNotebooks</span></span>

<span data-ttu-id="b5c81-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b5c81-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b5c81-105">获取登录用户访问的 [recentNotebook](../resources/recentnotebook.md) 实例列表。</span><span class="sxs-lookup"><span data-stu-id="b5c81-105">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="b5c81-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="b5c81-106">Permissions</span></span>
<span data-ttu-id="b5c81-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b5c81-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="b5c81-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b5c81-109">Permission type</span></span>      | <span data-ttu-id="b5c81-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b5c81-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="b5c81-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b5c81-111">Delegated (work or school account)</span></span> | <span data-ttu-id="b5c81-112">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5c81-112">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="b5c81-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b5c81-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b5c81-114">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="b5c81-114">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="b5c81-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b5c81-115">Application</span></span> | <span data-ttu-id="b5c81-116">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="b5c81-116">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="b5c81-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b5c81-117">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/{id | userPrincipalName}/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="b5c81-118">用户的 `{id | userPrincipalName}` 必须与用于发出请求的授权令牌中编码的用户一致。</span><span class="sxs-lookup"><span data-stu-id="b5c81-118">The `{id | userPrincipalName}` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="b5c81-119">函数参数</span><span class="sxs-lookup"><span data-stu-id="b5c81-119">Function parameters</span></span>

| <span data-ttu-id="b5c81-120">参数</span><span class="sxs-lookup"><span data-stu-id="b5c81-120">Parameter</span></span>    | <span data-ttu-id="b5c81-121">类型</span><span class="sxs-lookup"><span data-stu-id="b5c81-121">Type</span></span>   |<span data-ttu-id="b5c81-122">说明</span><span class="sxs-lookup"><span data-stu-id="b5c81-122">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b5c81-123">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="b5c81-123">includePersonalNotebooks</span></span>|<span data-ttu-id="b5c81-124">Boolean</span><span class="sxs-lookup"><span data-stu-id="b5c81-124">Boolean</span></span>|<span data-ttu-id="b5c81-125">添加用户拥有的笔记本。</span><span class="sxs-lookup"><span data-stu-id="b5c81-125">Include notebooks owned by the user.</span></span> <span data-ttu-id="b5c81-126">若要添加用户拥有的笔记本，请设置为 `true`；否则，设置为 `false`。</span><span class="sxs-lookup"><span data-stu-id="b5c81-126">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="b5c81-127">如果不添加 `includePersonalNotebooks` 参数，请求会返回 `400` 错误响应。</span><span class="sxs-lookup"><span data-stu-id="b5c81-127">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="b5c81-128">请求标头</span><span class="sxs-lookup"><span data-stu-id="b5c81-128">Request headers</span></span>
| <span data-ttu-id="b5c81-129">名称</span><span class="sxs-lookup"><span data-stu-id="b5c81-129">Name</span></span>       | <span data-ttu-id="b5c81-130">说明</span><span class="sxs-lookup"><span data-stu-id="b5c81-130">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="b5c81-131">Authorization</span><span class="sxs-lookup"><span data-stu-id="b5c81-131">Authorization</span></span>  | <span data-ttu-id="b5c81-132">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="b5c81-132">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="b5c81-133">请求正文</span><span class="sxs-lookup"><span data-stu-id="b5c81-133">Request body</span></span>
<span data-ttu-id="b5c81-134">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="b5c81-134">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="b5c81-135">响应</span><span class="sxs-lookup"><span data-stu-id="b5c81-135">Response</span></span>
<span data-ttu-id="b5c81-136">如果成功响应，则返回 `200 OK`，其中包含 **recentNotebooks** 的 JSON 集合。</span><span class="sxs-lookup"><span data-stu-id="b5c81-136">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="b5c81-137">示例</span><span class="sxs-lookup"><span data-stu-id="b5c81-137">Example</span></span>
<span data-ttu-id="b5c81-138">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="b5c81-138">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="b5c81-139">请求</span><span class="sxs-lookup"><span data-stu-id="b5c81-139">Request</span></span>
<span data-ttu-id="b5c81-140">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="b5c81-140">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/me/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)
```

##### <a name="response"></a><span data-ttu-id="b5c81-141">响应</span><span class="sxs-lookup"><span data-stu-id="b5c81-141">Response</span></span>
<span data-ttu-id="b5c81-142">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="b5c81-142">The following example shows the response.</span></span>

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


