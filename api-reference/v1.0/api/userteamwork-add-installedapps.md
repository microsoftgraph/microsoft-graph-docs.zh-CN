---
title: 为用户安装应用
description: 在指定用户的个人范围内安装应用。
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 984157470aeceb019e234aa11c3bd693bcc6b9b0
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564029"
---
# <a name="install-app-for-user"></a><span data-ttu-id="c27ad-103">为用户安装应用</span><span class="sxs-lookup"><span data-stu-id="c27ad-103">Install app for user</span></span>

<span data-ttu-id="c27ad-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="c27ad-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="c27ad-105">在指定[用户](../resources/user.md)的个人作用域中安装[应用程序](../resources/teamsapp.md)。</span><span class="sxs-lookup"><span data-stu-id="c27ad-105">Install an [app](../resources/teamsapp.md) in the personal scope of the specified [user](../resources/user.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c27ad-106">权限</span><span class="sxs-lookup"><span data-stu-id="c27ad-106">Permissions</span></span>

<span data-ttu-id="c27ad-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c27ad-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c27ad-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c27ad-109">Permission type</span></span>      | <span data-ttu-id="c27ad-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c27ad-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c27ad-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c27ad-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c27ad-112">ReadWriteSelfForUser、TeamsAppInstallation、TeamsAppInstallation TeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="c27ad-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser, TeamsAppInstallation.ReadWrite</span></span> |
|<span data-ttu-id="c27ad-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c27ad-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c27ad-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c27ad-114">Not supported.</span></span>    |
|<span data-ttu-id="c27ad-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c27ad-115">Application</span></span> | <span data-ttu-id="c27ad-116">TeamsAppInstallation、TeamsAppInstallation、all、TeamsAppInstallation、All</span><span class="sxs-lookup"><span data-stu-id="c27ad-116">TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All, TeamsAppInstallation.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c27ad-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c27ad-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps
```

## <a name="request-headers"></a><span data-ttu-id="c27ad-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="c27ad-118">Request headers</span></span>

| <span data-ttu-id="c27ad-119">标头</span><span class="sxs-lookup"><span data-stu-id="c27ad-119">Header</span></span>       | <span data-ttu-id="c27ad-120">值</span><span class="sxs-lookup"><span data-stu-id="c27ad-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="c27ad-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="c27ad-121">Authorization</span></span>  | <span data-ttu-id="c27ad-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="c27ad-p102">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="c27ad-124">Content-type</span><span class="sxs-lookup"><span data-stu-id="c27ad-124">Content-type</span></span> | <span data-ttu-id="c27ad-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="c27ad-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="c27ad-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="c27ad-127">Request body</span></span>

<span data-ttu-id="c27ad-128">请求正文应包含要添加的现有目录应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="c27ad-128">The request body should contain the ID of the existing catalog app to be added.</span></span>

| <span data-ttu-id="c27ad-129">属性</span><span class="sxs-lookup"><span data-stu-id="c27ad-129">Property</span></span>   | <span data-ttu-id="c27ad-130">类型</span><span class="sxs-lookup"><span data-stu-id="c27ad-130">Type</span></span> |<span data-ttu-id="c27ad-131">说明</span><span class="sxs-lookup"><span data-stu-id="c27ad-131">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c27ad-132">teamsApp</span><span class="sxs-lookup"><span data-stu-id="c27ad-132">teamsApp</span></span>|<span data-ttu-id="c27ad-133">String</span><span class="sxs-lookup"><span data-stu-id="c27ad-133">String</span></span>|<span data-ttu-id="c27ad-134">要添加的应用程序的 ID。</span><span class="sxs-lookup"><span data-stu-id="c27ad-134">The ID of the app to add.</span></span>|

## <a name="response"></a><span data-ttu-id="c27ad-135">响应</span><span class="sxs-lookup"><span data-stu-id="c27ad-135">Response</span></span>

<span data-ttu-id="c27ad-p104">如果成功，此方法返回 `201 Created` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="c27ad-p104">If successful, this method returns a `201 Created` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c27ad-138">示例</span><span class="sxs-lookup"><span data-stu-id="c27ad-138">Example</span></span>

### <a name="request"></a><span data-ttu-id="c27ad-139">请求</span><span class="sxs-lookup"><span data-stu-id="c27ad-139">Request</span></span>

<span data-ttu-id="c27ad-140">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="c27ad-140">The following is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "user_add_teamsApp"
}-->

```http
POST https://graph.microsoft.com/v1.0/users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps
Content-type: application/json

{
   "teamsApp@odata.bind":"https://graph.microsoft.com/v1.0/appCatalogs/teamsApps/12345678-9abc-def0-123456789a"
}
```

### <a name="response"></a><span data-ttu-id="c27ad-141">响应</span><span class="sxs-lookup"><span data-stu-id="c27ad-141">Response</span></span>
<span data-ttu-id="c27ad-142">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="c27ad-142">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true
} -->

```http
HTTP/1.1 201 Created
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "User add teamsAppInstallations",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
