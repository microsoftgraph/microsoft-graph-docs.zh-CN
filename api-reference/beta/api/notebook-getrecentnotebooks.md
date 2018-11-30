---
title: 笔记本：getRecentNotebooks
description: 获取登录用户访问的 recentNotebook 实例列表。
ms.openlocfilehash: dd273197ecfc417bd385ff6d769f96efd3972362
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044260"
---
# <a name="notebook-getrecentnotebooks"></a><span data-ttu-id="45b4d-103">笔记本：getRecentNotebooks</span><span class="sxs-lookup"><span data-stu-id="45b4d-103">notebook: getRecentNotebooks</span></span>

> <span data-ttu-id="45b4d-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="45b4d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="45b4d-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="45b4d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="45b4d-106">获取登录用户访问的 [recentNotebook](../resources/recentnotebook.md) 实例列表。</span><span class="sxs-lookup"><span data-stu-id="45b4d-106">Get a list of [recentNotebook](../resources/recentnotebook.md) instances that have been accessed by the signed-in user.</span></span>

## <a name="permissions"></a><span data-ttu-id="45b4d-107">权限</span><span class="sxs-lookup"><span data-stu-id="45b4d-107">Permissions</span></span>
<span data-ttu-id="45b4d-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="45b4d-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45b4d-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="45b4d-110">Permission type</span></span>      | <span data-ttu-id="45b4d-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="45b4d-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="45b4d-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="45b4d-112">Delegated (work or school account)</span></span> | <span data-ttu-id="45b4d-113">Notes.Create、Notes.Read、Notes.ReadWrite、Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45b4d-113">Notes.Create, Notes.Read, Notes.ReadWrite, Notes.Read.All, Notes.ReadWrite.All,</span></span>|
|<span data-ttu-id="45b4d-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="45b4d-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="45b4d-115">Notes.Create、Notes.Read、Notes.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="45b4d-115">Notes.Create, Notes.Read, Notes.ReadWrite</span></span> |
|<span data-ttu-id="45b4d-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="45b4d-116">Application</span></span> | <span data-ttu-id="45b4d-117">Notes.Read.All、Notes.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45b4d-117">Notes.Read.All, Notes.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="45b4d-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="45b4d-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->
```http
GET /me/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
GET /users/<id | userPrincipalName>/onenote/notebooks/getRecentNotebooks(includePersonalNotebooks=includePersonalNotebooks-value)
```

<span data-ttu-id="45b4d-119">用户的 `<id | userPrincipalName>` 必须与用于发出请求的授权令牌中编码的用户一致。</span><span class="sxs-lookup"><span data-stu-id="45b4d-119">The `<id | userPrincipalName>` for the user must match the user encoded in the authorization token used to make the request.</span></span>

## <a name="function-parameters"></a><span data-ttu-id="45b4d-120">函数参数</span><span class="sxs-lookup"><span data-stu-id="45b4d-120">Function parameters</span></span>

| <span data-ttu-id="45b4d-121">参数</span><span class="sxs-lookup"><span data-stu-id="45b4d-121">Parameter</span></span>    | <span data-ttu-id="45b4d-122">类型</span><span class="sxs-lookup"><span data-stu-id="45b4d-122">Type</span></span>   |<span data-ttu-id="45b4d-123">说明</span><span class="sxs-lookup"><span data-stu-id="45b4d-123">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="45b4d-124">includePersonalNotebooks</span><span class="sxs-lookup"><span data-stu-id="45b4d-124">includePersonalNotebooks</span></span>|<span data-ttu-id="45b4d-125">Boolean</span><span class="sxs-lookup"><span data-stu-id="45b4d-125">Boolean</span></span>|<span data-ttu-id="45b4d-126">添加用户拥有的笔记本。</span><span class="sxs-lookup"><span data-stu-id="45b4d-126">Include notebooks owned by the user.</span></span> <span data-ttu-id="45b4d-127">若要添加用户拥有的笔记本，请设置为 `true`；否则，设置为 `false`。</span><span class="sxs-lookup"><span data-stu-id="45b4d-127">Set to `true` to include notebooks owned by the user; otherwise, set to `false`.</span></span> <span data-ttu-id="45b4d-128">如果不添加 `includePersonalNotebooks` 参数，请求会返回 `400` 错误响应。</span><span class="sxs-lookup"><span data-stu-id="45b4d-128">If you don't include the `includePersonalNotebooks` parameter, your request will return a `400` error response.</span></span>|

## <a name="request-headers"></a><span data-ttu-id="45b4d-129">请求标头</span><span class="sxs-lookup"><span data-stu-id="45b4d-129">Request headers</span></span>
| <span data-ttu-id="45b4d-130">名称</span><span class="sxs-lookup"><span data-stu-id="45b4d-130">Name</span></span>       | <span data-ttu-id="45b4d-131">说明</span><span class="sxs-lookup"><span data-stu-id="45b4d-131">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="45b4d-132">Authorization</span><span class="sxs-lookup"><span data-stu-id="45b4d-132">Authorization</span></span>  | <span data-ttu-id="45b4d-133">Bearer {code}</span><span class="sxs-lookup"><span data-stu-id="45b4d-133">Bearer {code}</span></span>|

## <a name="request-body"></a><span data-ttu-id="45b4d-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="45b4d-134">Request body</span></span>
<span data-ttu-id="45b4d-135">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="45b4d-135">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="45b4d-136">响应</span><span class="sxs-lookup"><span data-stu-id="45b4d-136">Response</span></span>
<span data-ttu-id="45b4d-137">如果成功响应，则返回 `200 OK`，其中包含 **recentNotebooks** 的 JSON 集合。</span><span class="sxs-lookup"><span data-stu-id="45b4d-137">A successful response returns a `200 OK` that contains a JSON collection of **recentNotebooks**.</span></span>

## <a name="example"></a><span data-ttu-id="45b4d-138">示例</span><span class="sxs-lookup"><span data-stu-id="45b4d-138">Example</span></span>
<span data-ttu-id="45b4d-139">以下示例演示如何调用此 API。</span><span class="sxs-lookup"><span data-stu-id="45b4d-139">The following example shows how to call this API.</span></span>

##### <a name="request"></a><span data-ttu-id="45b4d-140">请求</span><span class="sxs-lookup"><span data-stu-id="45b4d-140">Request</span></span>
<span data-ttu-id="45b4d-141">下面为请求示例。</span><span class="sxs-lookup"><span data-stu-id="45b4d-141">The following example shows the request.</span></span>
<!-- { "blockType": "request", "name": "recent_notebooks", "scopes": "notes.read" } -->
```http
GET https://graph.microsoft.com/v1.0/onenote/notebooks/getrecentnotebooks(includePersonalNotebooks=true)
```

##### <a name="response"></a><span data-ttu-id="45b4d-142">响应</span><span class="sxs-lookup"><span data-stu-id="45b4d-142">Response</span></span>
<span data-ttu-id="45b4d-143">以下示例显示了相应的响应。</span><span class="sxs-lookup"><span data-stu-id="45b4d-143">The following example shows the response.</span></span>

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
