---
title: 获取设置
description: 阅读用户和组织设置对象。
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 0663f9581eb34be5c26c8666887c7c3bee7cffc1
ms.sourcegitcommit: 71b5a96f14984a76c386934b648f730baa1b2357
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/27/2021
ms.locfileid: "52031422"
---
# <a name="get-settings"></a><span data-ttu-id="fbade-103">获取设置</span><span class="sxs-lookup"><span data-stu-id="fbade-103">Get settings</span></span>

<span data-ttu-id="fbade-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="fbade-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="fbade-105">读取用户和组织 [userSettings](../resources/usersettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fbade-105">Read the user and organization [userSettings](../resources/usersettings.md) object.</span></span>
<span data-ttu-id="fbade-106">若要了解如何更新 [userSettings](../resources/usersettings.md) 对象的属性，请参阅[更新用户设置](usersettings-update.md)。</span><span class="sxs-lookup"><span data-stu-id="fbade-106">To learn how to update the properties of the [userSettings](../resources/usersettings.md) object, see [update user settings](usersettings-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="fbade-107">权限</span><span class="sxs-lookup"><span data-stu-id="fbade-107">Permissions</span></span>

<span data-ttu-id="fbade-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fbade-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fbade-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fbade-110">Permission type</span></span>      | <span data-ttu-id="fbade-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fbade-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fbade-112">委托（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fbade-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fbade-113">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbade-113">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="fbade-114">委托（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fbade-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fbade-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fbade-115">Not supported.</span></span>    |
|<span data-ttu-id="fbade-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fbade-116">Application</span></span> | <span data-ttu-id="fbade-117">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="fbade-117">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fbade-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fbade-118">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="fbade-119">具有“用户ID”或“userPrincipalName”的请求只能由用户或具有 User.ReadWrite.All 权限的用户访问。</span><span class="sxs-lookup"><span data-stu-id="fbade-119">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="fbade-120">若要了解详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fbade-120">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="fbade-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="fbade-121">Request body</span></span>

<span data-ttu-id="fbade-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fbade-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fbade-123">响应</span><span class="sxs-lookup"><span data-stu-id="fbade-123">Response</span></span>

<span data-ttu-id="fbade-124">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [userSettings](../resources/usersettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="fbade-124">If successful, this method returns a `200 OK` response code and [userSettings](../resources/usersettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="fbade-125">示例</span><span class="sxs-lookup"><span data-stu-id="fbade-125">Example</span></span>

##### <a name="request"></a><span data-ttu-id="fbade-126">请求</span><span class="sxs-lookup"><span data-stu-id="fbade-126">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a><span data-ttu-id="fbade-127">响应</span><span class="sxs-lookup"><span data-stu-id="fbade-127">Response</span></span>

<span data-ttu-id="fbade-128">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fbade-128">Here is an example of the response.</span></span> <span data-ttu-id="fbade-129">注意：为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="fbade-129">Note: The response object shown here might be shortened for readability.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```


