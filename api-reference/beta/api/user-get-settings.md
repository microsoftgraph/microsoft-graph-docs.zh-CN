---
title: 获取设置
description: 读取用户和组织设置对象。
author: dkershaw10
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 128feebf624350baaea9fee41c411bd46c2b42c5
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29507479"
---
# <a name="get-settings"></a><span data-ttu-id="ea668-103">获取设置</span><span class="sxs-lookup"><span data-stu-id="ea668-103">Get settings</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea668-104">读取用户和组织[设置](../resources/user-settings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ea668-104">Read the user and organization [settings](../resources/user-settings.md) object.</span></span>
<span data-ttu-id="ea668-105">若要了解如何更新[设置](../resources/user-settings.md)对象的属性，请参阅[更新用户设置](user-update-settings.md)。</span><span class="sxs-lookup"><span data-stu-id="ea668-105">To learn how to update the properties of the [settings](../resources/user-settings.md) object, see [update user settings](user-update-settings.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="ea668-106">权限</span><span class="sxs-lookup"><span data-stu-id="ea668-106">Permissions</span></span>

<span data-ttu-id="ea668-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea668-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea668-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea668-109">Permission type</span></span>      | <span data-ttu-id="ea668-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ea668-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea668-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea668-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ea668-112">User.Read.All、User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea668-112">User.Read.All, User.ReadWrite.All</span></span>    |
|<span data-ttu-id="ea668-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea668-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea668-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea668-114">Not supported.</span></span>    |
|<span data-ttu-id="ea668-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea668-115">Application</span></span> | <span data-ttu-id="ea668-116">User.Read.All,User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea668-116">User.Read.All,User.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea668-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea668-117">HTTP request</span></span>

```http
GET /me/settings/
```

<span data-ttu-id="ea668-118">请求用户 id 或者 userPrincipalName 才可以访问由用户或由具有 User.ReadWrite.All 权限的用户。</span><span class="sxs-lookup"><span data-stu-id="ea668-118">Request with a 'user id' or 'userPrincipalName' is only accessible by the user or by a user with the User.ReadWrite.All permissions.</span></span> <span data-ttu-id="ea668-119">若要了解详细信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea668-119">To learn more, see [Permissions](/graph/permissions-reference).</span></span>

```http
GET /users/{id | userPrincipalName}/settings/
```

## <a name="request-body"></a><span data-ttu-id="ea668-120">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea668-120">Request body</span></span>

<span data-ttu-id="ea668-121">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ea668-121">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ea668-122">响应</span><span class="sxs-lookup"><span data-stu-id="ea668-122">Response</span></span>

<span data-ttu-id="ea668-123">如果成功，此方法返回`200 OK`响应正文中的响应代码和[用户设置](../resources/user-settings.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ea668-123">If successful, this method returns a `200 OK` response code and [user settings](../resources/user-settings.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea668-124">示例</span><span class="sxs-lookup"><span data-stu-id="ea668-124">Example</span></span>

##### <a name="request"></a><span data-ttu-id="ea668-125">请求</span><span class="sxs-lookup"><span data-stu-id="ea668-125">Request</span></span>

```http
GET https://graph.microsoft.com/beta/me/settings
```

##### <a name="response"></a><span data-ttu-id="ea668-126">响应</span><span class="sxs-lookup"><span data-stu-id="ea668-126">Response</span></span>

<span data-ttu-id="ea668-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ea668-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 72

{
  "contributionToContentDiscoveryAsOrganizationDisabled": false,
  "contributionToContentDiscoveryDisabled": false
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/user-get-settings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
