---
title: 创建 outlookTaskGroup
description: 在用户邮箱中创建 Outlook 任务组。
localization_priority: Normal
ms.openlocfilehash: 2640d540c3b5f81c14763f785c565268bb15d689
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851910"
---
# <a name="create-outlooktaskgroup"></a><span data-ttu-id="aed41-103">创建 outlookTaskGroup</span><span class="sxs-lookup"><span data-stu-id="aed41-103">Create outlookTaskGroup</span></span>

> <span data-ttu-id="aed41-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="aed41-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="aed41-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="aed41-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="aed41-106">在用户邮箱中创建 Outlook 任务组。</span><span class="sxs-lookup"><span data-stu-id="aed41-106">Create an Outlook task group in the user's mailbox.</span></span>
## <a name="permissions"></a><span data-ttu-id="aed41-107">权限</span><span class="sxs-lookup"><span data-stu-id="aed41-107">Permissions</span></span>
<span data-ttu-id="aed41-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="aed41-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="aed41-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="aed41-110">Permission type</span></span>      | <span data-ttu-id="aed41-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="aed41-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="aed41-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="aed41-112">Delegated (work or school account)</span></span> | <span data-ttu-id="aed41-113">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aed41-113">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="aed41-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="aed41-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="aed41-115">Tasks.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="aed41-115">Tasks.ReadWrite</span></span>    |
|<span data-ttu-id="aed41-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="aed41-116">Application</span></span> | <span data-ttu-id="aed41-117">不支持。</span><span class="sxs-lookup"><span data-stu-id="aed41-117">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="aed41-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="aed41-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id|userPrincipalName}/outlook/taskGroups

```
## <a name="request-headers"></a><span data-ttu-id="aed41-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="aed41-119">Request headers</span></span>
| <span data-ttu-id="aed41-120">名称</span><span class="sxs-lookup"><span data-stu-id="aed41-120">Name</span></span>       | <span data-ttu-id="aed41-121">说明</span><span class="sxs-lookup"><span data-stu-id="aed41-121">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="aed41-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="aed41-122">Authorization</span></span>  | <span data-ttu-id="aed41-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="aed41-p103">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="aed41-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="aed41-125">Request body</span></span>
<span data-ttu-id="aed41-126">在请求正文中，提供[outlookTaskGroup](../resources/outlooktaskgroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aed41-126">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="aed41-127">响应</span><span class="sxs-lookup"><span data-stu-id="aed41-127">Response</span></span>

<span data-ttu-id="aed41-128">如果成功，此方法返回`201 Created`响应正文中的响应代码和[outlookTaskGroup](../resources/outlooktaskgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="aed41-128">If successful, this method returns `201 Created` response code and [outlookTaskGroup](../resources/outlooktaskgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="aed41-129">示例</span><span class="sxs-lookup"><span data-stu-id="aed41-129">Example</span></span>
##### <a name="request"></a><span data-ttu-id="aed41-130">请求</span><span class="sxs-lookup"><span data-stu-id="aed41-130">Request</span></span>
<span data-ttu-id="aed41-131">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="aed41-131">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_outlooktaskgroup_from_outlookuser"
}-->
```http
POST https://graph.microsoft.com/beta/me/outlook/taskGroups
Content-type: application/json
Content-length: 40

{
  "name": "Leisure tasks"
}
```
<span data-ttu-id="aed41-132">在请求正文中，提供[outlookTaskGroup](../resources/outlooktaskgroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aed41-132">In the request body, supply a JSON representation of [outlookTaskGroup](../resources/outlooktaskgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="aed41-133">响应</span><span class="sxs-lookup"><span data-stu-id="aed41-133">Response</span></span>
<span data-ttu-id="aed41-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="aed41-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookTaskGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 138

{
  "id": "AAMkADIyAAAhrbe-AAA=",
  "changeKey": "hmM7Eb/jgEec8l3+gkJEawAAIbAGjg==",
  "isDefaultGroup": false,
  "name": "Leisure tasks",
  "groupKey": "63d640cf-946f-4734-9c29-60dda7b76acb"

}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Create outlookTaskGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
