---
title: teamsAppInstallation： upgrade
description: 在用户的个人作用域中升级应用程序安装
author: clearab
doc_type: apiPageType
localization_priority: Normal
ms.prod: microsoft-teams
ms.openlocfilehash: 8b38ef1ab60dc2d38a52acaeabe0e2c5491d2d5a
ms.sourcegitcommit: 958b540f118ef3ce64d4d4e96b29264e2b56d703
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/03/2020
ms.locfileid: "49564026"
---
# <a name="teamsappinstallation-upgrade"></a><span data-ttu-id="174e6-103">teamsAppInstallation： upgrade</span><span class="sxs-lookup"><span data-stu-id="174e6-103">teamsAppInstallation: upgrade</span></span>

<span data-ttu-id="174e6-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="174e6-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="174e6-105">将指定[用户](../resources/user.md)的个人作用域中的[应用程序安装](../resources/teamsappinstallation.md)升级到最新版本的应用程序。</span><span class="sxs-lookup"><span data-stu-id="174e6-105">Upgrade an [app installation](../resources/teamsappinstallation.md) in the personal scope of the specified [user](../resources/user.md) to the latest version of the app.</span></span>

## <a name="permissions"></a><span data-ttu-id="174e6-106">权限</span><span class="sxs-lookup"><span data-stu-id="174e6-106">Permissions</span></span>

<span data-ttu-id="174e6-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="174e6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="174e6-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="174e6-109">Permission type</span></span>      | <span data-ttu-id="174e6-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="174e6-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="174e6-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="174e6-111">Delegated (work or school account)</span></span> | <span data-ttu-id="174e6-112">ReadWriteSelfForUser、TeamsAppInstallation、TeamsAppInstallation TeamsAppInstallation</span><span class="sxs-lookup"><span data-stu-id="174e6-112">TeamsAppInstallation.ReadWriteSelfForUser, TeamsAppInstallation.ReadWriteForUser, TeamsAppInstallation.ReadWrite</span></span> |
|<span data-ttu-id="174e6-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="174e6-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="174e6-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="174e6-114">Not supported.</span></span>    |
|<span data-ttu-id="174e6-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="174e6-115">Application</span></span> | <span data-ttu-id="174e6-116">TeamsAppInstallation、TeamsAppInstallation、all、TeamsAppInstallation、All</span><span class="sxs-lookup"><span data-stu-id="174e6-116">TeamsAppInstallation.ReadWriteSelfForUser.All, TeamsAppInstallation.ReadWriteForUser.All, TeamsAppInstallation.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="174e6-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="174e6-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /users/{id}/teamwork/installedApps/{id}/upgrade
```

## <a name="request-headers"></a><span data-ttu-id="174e6-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="174e6-118">Request headers</span></span>

| <span data-ttu-id="174e6-119">标头</span><span class="sxs-lookup"><span data-stu-id="174e6-119">Header</span></span>       | <span data-ttu-id="174e6-120">值</span><span class="sxs-lookup"><span data-stu-id="174e6-120">Value</span></span> |
|:---------------|:--------|
| <span data-ttu-id="174e6-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="174e6-121">Authorization</span></span>  | <span data-ttu-id="174e6-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="174e6-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="174e6-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="174e6-124">Request body</span></span>

<span data-ttu-id="174e6-125">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="174e6-125">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="174e6-126">响应</span><span class="sxs-lookup"><span data-stu-id="174e6-126">Response</span></span>

<span data-ttu-id="174e6-p103">如果成功，此方法返回 `204 No Content` 响应代码。它不在响应正文中返回任何内容。</span><span class="sxs-lookup"><span data-stu-id="174e6-p103">If successful, this method returns a `204 No Content` response code. It does not return anything in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="174e6-129">示例</span><span class="sxs-lookup"><span data-stu-id="174e6-129">Example</span></span>

### <a name="request"></a><span data-ttu-id="174e6-130">请求</span><span class="sxs-lookup"><span data-stu-id="174e6-130">Request</span></span>

<span data-ttu-id="174e6-131">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="174e6-131">The following is an example of the request.</span></span>


<!-- {
  "blockType": "request",
  "name": "user_upgrade_teamsApp"
}-->

```http
POST /users/5b649834-7412-4cce-9e69-176e95a394f5/teamwork/installedApps/NWI2NDk4MzQtNzQxMi00Y2NlLTllNjktMTc2ZTk1YTM5NGY1IyNhNmI2MzM2NS0zMWE0LTRmNDMtOTJlYy03MTBiNzE1NTdhZjk/upgrade
```

### <a name="response"></a><span data-ttu-id="174e6-132">响应</span><span class="sxs-lookup"><span data-stu-id="174e6-132">Response</span></span>

<span data-ttu-id="174e6-133">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="174e6-133">The following is an example of the response.</span></span>

<!-- {
  "blockType": "response",
  "name": "user_upgrade_teamsApp",
  "truncated": true
} -->

```http
HTTP/1.1 204 No Content
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Upgrade teamsApp for user",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
