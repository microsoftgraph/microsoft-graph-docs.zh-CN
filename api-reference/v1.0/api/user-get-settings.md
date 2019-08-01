---
title: 获取设置
description: 阅读用户和组织设置对象。
author: dkershaw10
localization_priority: Priority
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 64ecf4c4f44cf59bf3c6344edda7510a6997d813
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/31/2019
ms.locfileid: "36027074"
---
# <a name="get-settings"></a><span data-ttu-id="c9a44-103">获取设置</span><span class="sxs-lookup"><span data-stu-id="c9a44-103">Get settings</span></span>

<span data-ttu-id="c9a44-104">阅读用户和组织[设置](../resources/user-settings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c9a44-104">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="c9a44-105">若要了解如何更新[设置](../resources/user-settings.md)对象的属性，请参阅[更新用户设置](user-update-settings.md)。</span><span class="sxs-lookup"><span data-stu-id="c9a44-105">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="c9a44-106">权限</span><span class="sxs-lookup"><span data-stu-id="c9a44-106">Permissions</span></span>

<span data-ttu-id="c9a44-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9a44-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c9a44-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="c9a44-109">Permission type</span></span>      | <span data-ttu-id="c9a44-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c9a44-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c9a44-111">委托（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c9a44-111">Delegated (work or school account)</span></span> | <span data-ttu-id="c9a44-112">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9a44-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="c9a44-113">委托（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c9a44-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c9a44-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="c9a44-114">Not supported.</span></span>    |
|<span data-ttu-id="c9a44-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="c9a44-115">Application</span></span> | <span data-ttu-id="c9a44-116">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c9a44-116">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c9a44-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c9a44-117">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="c9a44-118">具有“用户ID”或“userPrincipalName”的请求只能由用户或具有 User.ReadWrite.All 权限的用户访问。</span><span class="sxs-lookup"><span data-stu-id="c9a44-118">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="c9a44-119">若要了解详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c9a44-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="c9a44-120">请求正文</span><span class="sxs-lookup"><span data-stu-id="c9a44-120">Request body</span></span>

<span data-ttu-id="c9a44-121">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="c9a44-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="c9a44-122">响应</span><span class="sxs-lookup"><span data-stu-id="c9a44-122">Response</span></span>

<span data-ttu-id="c9a44-123">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和[用户设置](../resources/user-settings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c9a44-123">If successful, this method returns a `200 OK` response code and [user settings](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c9a44-124">示例</span><span class="sxs-lookup"><span data-stu-id="c9a44-124">Example</span></span>

##### <a name="request"></a><span data-ttu-id="c9a44-125">请求</span><span class="sxs-lookup"><span data-stu-id="c9a44-125">Request</span></span>

```http
GET https://graph.microsoft.com/v1.0/me/settings
```

##### <a name="response"></a><span data-ttu-id="c9a44-126">响应</span><span class="sxs-lookup"><span data-stu-id="c9a44-126">Response</span></span>

<span data-ttu-id="c9a44-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c9a44-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```

