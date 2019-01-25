---
title: 添加应用程序密码
description: 向应用程序中的强密码。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 15189ee709b2b369d014f9854bcdbd4dc1b7e9be
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29526821"
---
# <a name="add-application-password"></a><span data-ttu-id="81d3f-103">添加应用程序密码</span><span class="sxs-lookup"><span data-stu-id="81d3f-103">Add application password</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="81d3f-104">向应用程序中的强密码。</span><span class="sxs-lookup"><span data-stu-id="81d3f-104">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="81d3f-105">权限</span><span class="sxs-lookup"><span data-stu-id="81d3f-105">Permissions</span></span>
<span data-ttu-id="81d3f-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="81d3f-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="81d3f-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="81d3f-108">Permission type</span></span>      | <span data-ttu-id="81d3f-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="81d3f-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="81d3f-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="81d3f-110">Delegated (work or school account)</span></span> | <span data-ttu-id="81d3f-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="81d3f-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="81d3f-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="81d3f-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="81d3f-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="81d3f-113">Not supported.</span></span>    |
|<span data-ttu-id="81d3f-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="81d3f-114">Application</span></span> | <span data-ttu-id="81d3f-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="81d3f-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="81d3f-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="81d3f-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="81d3f-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="81d3f-117">Request headers</span></span>
| <span data-ttu-id="81d3f-118">名称</span><span class="sxs-lookup"><span data-stu-id="81d3f-118">Name</span></span>       | <span data-ttu-id="81d3f-119">类型</span><span class="sxs-lookup"><span data-stu-id="81d3f-119">Type</span></span> | <span data-ttu-id="81d3f-120">说明</span><span class="sxs-lookup"><span data-stu-id="81d3f-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="81d3f-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="81d3f-121">Authorization</span></span>  | <span data-ttu-id="81d3f-122">string</span><span class="sxs-lookup"><span data-stu-id="81d3f-122">string</span></span>  | <span data-ttu-id="81d3f-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="81d3f-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="81d3f-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="81d3f-125">Request body</span></span>
<span data-ttu-id="81d3f-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="81d3f-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="81d3f-127">响应</span><span class="sxs-lookup"><span data-stu-id="81d3f-127">Response</span></span>

<span data-ttu-id="81d3f-128">如果成功，此方法返回`200 OK`响应正文中的响应代码和密码对象。</span><span class="sxs-lookup"><span data-stu-id="81d3f-128">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="81d3f-129">Azure AD 将生成一个强密码通过返回的`secretText`属性。</span><span class="sxs-lookup"><span data-stu-id="81d3f-129">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="81d3f-130">没有方法，以便将来检索此密码。</span><span class="sxs-lookup"><span data-stu-id="81d3f-130">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="81d3f-131">示例</span><span class="sxs-lookup"><span data-stu-id="81d3f-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="81d3f-132">请求</span><span class="sxs-lookup"><span data-stu-id="81d3f-132">Request</span></span>
<span data-ttu-id="81d3f-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="81d3f-133">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="81d3f-134">响应</span><span class="sxs-lookup"><span data-stu-id="81d3f-134">Response</span></span>
<span data-ttu-id="81d3f-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="81d3f-135">Here is an example of the response.</span></span>

```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 1044

{
    "customKeyIdentifier": "Binary",
    "endDateTime": "String (timestamp)",
    "keyId": "String (identifier)",
    "startDateTime": "String (timestamp)",
    "secretText": "String",
    "hint": "String"
}
```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/api/application-add-password.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
