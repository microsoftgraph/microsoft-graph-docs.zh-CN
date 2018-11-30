---
title: 获取设置
description: 读取用户和组织设置对象。
ms.openlocfilehash: dc0f5e23f1c00291af90a1e2f685d947046b925f
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27046816"
---
# <a name="get-settings"></a><span data-ttu-id="7faae-103">获取设置</span><span class="sxs-lookup"><span data-stu-id="7faae-103">Get settings</span></span>

> <span data-ttu-id="7faae-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="7faae-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="7faae-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="7faae-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="7faae-106">读取用户和组织[设置](../resources/user-settings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7faae-106">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="7faae-107">若要了解如何更新[设置](../resources/user-settings.md)对象的属性，请参阅[更新用户设置](user-update-settings.md)。</span><span class="sxs-lookup"><span data-stu-id="7faae-107">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="7faae-108">权限</span><span class="sxs-lookup"><span data-stu-id="7faae-108">Permissions</span></span>

<span data-ttu-id="7faae-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7faae-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7faae-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="7faae-111">Permission type</span></span>      | <span data-ttu-id="7faae-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7faae-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="7faae-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7faae-113">Delegated (work or school account)</span></span> | <span data-ttu-id="7faae-114">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7faae-114">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="7faae-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7faae-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7faae-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="7faae-116">Not supported.</span></span>    |
|<span data-ttu-id="7faae-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="7faae-117">Application</span></span> | <span data-ttu-id="7faae-118">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7faae-118">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="7faae-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7faae-119">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="7faae-120">请求用户 id 或者 userPrincipalName 才可以访问由用户或由具有 User.ReadWrite.All 权限的用户。</span><span class="sxs-lookup"><span data-stu-id="7faae-120">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="7faae-121">若要了解详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7faae-121">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="7faae-122">请求正文</span><span class="sxs-lookup"><span data-stu-id="7faae-122">Request body</span></span>

<span data-ttu-id="7faae-123">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="7faae-123">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="7faae-124">响应</span><span class="sxs-lookup"><span data-stu-id="7faae-124">Response</span></span>

<span data-ttu-id="7faae-125">如果成功，此方法返回`200 OK`响应正文中的响应代码和[用户设置](../resources/user-settings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7faae-125">If successful, this method returns a `200 OK` response code and [user settings](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7faae-126">示例</span><span class="sxs-lookup"><span data-stu-id="7faae-126">Example</span></span>

##### <a name="request"></a><span data-ttu-id="7faae-127">请求</span><span class="sxs-lookup"><span data-stu-id="7faae-127">Request</span></span>

```http
GET https://graph.microsoft.com/beta/me/settings
```

##### <a name="response"></a><span data-ttu-id="7faae-128">响应</span><span class="sxs-lookup"><span data-stu-id="7faae-128">Response</span></span>

<span data-ttu-id="7faae-p105">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="7faae-p105">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```
