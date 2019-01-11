---
title: 获取设置
description: 读取用户和组织设置对象。
author: dkershaw10
localization_priority: Priority
ms.openlocfilehash: ace7c43b27860832968572628838484bc8c91c84
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27815489"
---
# <a name="get-settings"></a><span data-ttu-id="a08c5-103">获取设置</span><span class="sxs-lookup"><span data-stu-id="a08c5-103">Get settings</span></span>

<span data-ttu-id="a08c5-104">读取用户和组织[设置](../resources/user-settings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a08c5-104">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="a08c5-105">若要了解如何更新[设置](../resources/user-settings.md)对象的属性，请参阅[更新用户设置](user-update-settings.md)。</span><span class="sxs-lookup"><span data-stu-id="a08c5-105">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="a08c5-106">权限</span><span class="sxs-lookup"><span data-stu-id="a08c5-106">Permissions</span></span>

<span data-ttu-id="a08c5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a08c5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="a08c5-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="a08c5-109">Permission type</span></span>      | <span data-ttu-id="a08c5-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="a08c5-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="a08c5-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="a08c5-111">Delegated (work or school account)</span></span> | <span data-ttu-id="a08c5-112">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a08c5-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="a08c5-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="a08c5-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="a08c5-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="a08c5-114">Not supported.</span></span>    |
|<span data-ttu-id="a08c5-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="a08c5-115">Application</span></span> | <span data-ttu-id="a08c5-116">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a08c5-116">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="a08c5-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="a08c5-117">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="a08c5-118">请求用户 id 或者 userPrincipalName 才可以访问由用户或由具有 User.ReadWrite.All 权限的用户。</span><span class="sxs-lookup"><span data-stu-id="a08c5-118">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="a08c5-119">若要了解详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="a08c5-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="a08c5-120">请求正文</span><span class="sxs-lookup"><span data-stu-id="a08c5-120">Request body</span></span>

<span data-ttu-id="a08c5-121">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="a08c5-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="a08c5-122">响应</span><span class="sxs-lookup"><span data-stu-id="a08c5-122">Response</span></span>

<span data-ttu-id="a08c5-123">如果成功，此方法返回`200 OK`响应正文中的响应代码和[用户设置](../resources/user-settings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="a08c5-123">If successful, this method returns a `200 OK` response code and [user settings](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a08c5-124">示例</span><span class="sxs-lookup"><span data-stu-id="a08c5-124">Example</span></span>

##### <a name="request"></a><span data-ttu-id="a08c5-125">请求</span><span class="sxs-lookup"><span data-stu-id="a08c5-125">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a><span data-ttu-id="a08c5-126">响应</span><span class="sxs-lookup"><span data-stu-id="a08c5-126">Response</span></span>

<span data-ttu-id="a08c5-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="a08c5-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

