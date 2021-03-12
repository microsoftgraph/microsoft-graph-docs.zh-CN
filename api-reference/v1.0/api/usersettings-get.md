---
title: 获取设置
description: 阅读用户和组织设置对象。
author: jpettere
localization_priority: Priority
ms.prod: users
doc_type: apiPageType
ms.openlocfilehash: 9aa36e3762faddb0f9cc0f9f419c497f2ce3aa82
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721256"
---
# <a name="get-settings"></a><span data-ttu-id="483ce-103">获取设置</span><span class="sxs-lookup"><span data-stu-id="483ce-103">Get settings</span></span>

<span data-ttu-id="483ce-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="483ce-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="483ce-105">读取用户和组织 [userSettings](../resources/usersettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="483ce-105">Read the user and organization [userSettings](../resources/usersettings.md) object.</span></span>
<span data-ttu-id="483ce-106">若要了解如何更新 [userSettings](../resources/usersettings.md) 对象的属性，请参阅[更新用户设置](usersettings-update.md)。</span><span class="sxs-lookup"><span data-stu-id="483ce-106">To learn how to update the properties of the [userSettings](../resources/usersettings.md) object, see [update user settings](usersettings-update.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="483ce-107">权限</span><span class="sxs-lookup"><span data-stu-id="483ce-107">Permissions</span></span>

<span data-ttu-id="483ce-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="483ce-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="483ce-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="483ce-110">Permission type</span></span>      | <span data-ttu-id="483ce-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="483ce-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="483ce-112">委托（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="483ce-112">Delegated (work or school account)</span></span> | <span data-ttu-id="483ce-113">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="483ce-113">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="483ce-114">委托（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="483ce-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="483ce-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="483ce-115">Not supported.</span></span>    |
|<span data-ttu-id="483ce-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="483ce-116">Application</span></span> | <span data-ttu-id="483ce-117">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="483ce-117">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="483ce-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="483ce-118">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="483ce-119">具有“用户ID”或“userPrincipalName”的请求只能由用户或具有 User.ReadWrite.All 权限的用户访问。</span><span class="sxs-lookup"><span data-stu-id="483ce-119">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="483ce-120">若要了解详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="483ce-120">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="483ce-121">请求正文</span><span class="sxs-lookup"><span data-stu-id="483ce-121">Request body</span></span>

<span data-ttu-id="483ce-122">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="483ce-122">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="483ce-123">响应</span><span class="sxs-lookup"><span data-stu-id="483ce-123">Response</span></span>

<span data-ttu-id="483ce-124">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和 [userSettings](../resources/usersettings.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="483ce-124">If successful, this method returns a `200 OK` response code and [userSettings](../resources/usersettings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="483ce-125">示例</span><span class="sxs-lookup"><span data-stu-id="483ce-125">Example</span></span>

##### <a name="request"></a><span data-ttu-id="483ce-126">请求</span><span class="sxs-lookup"><span data-stu-id="483ce-126">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a><span data-ttu-id="483ce-127">响应</span><span class="sxs-lookup"><span data-stu-id="483ce-127">Response</span></span>

<span data-ttu-id="483ce-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="483ce-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```


