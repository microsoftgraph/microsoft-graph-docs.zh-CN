---
title: 添加应用程序密码
description: 向应用程序添加强密码。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ee2000daba1f003705979ceb04e78ed920ea9281
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/31/2019
ms.locfileid: "34655157"
---
# <a name="add-application-password"></a><span data-ttu-id="1a909-103">添加应用程序密码</span><span class="sxs-lookup"><span data-stu-id="1a909-103">Add application password</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="1a909-104">向应用程序添加强密码。</span><span class="sxs-lookup"><span data-stu-id="1a909-104">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="1a909-105">权限</span><span class="sxs-lookup"><span data-stu-id="1a909-105">Permissions</span></span>
<span data-ttu-id="1a909-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1a909-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1a909-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="1a909-108">Permission type</span></span>      | <span data-ttu-id="1a909-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1a909-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="1a909-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1a909-110">Delegated (work or school account)</span></span> | <span data-ttu-id="1a909-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="1a909-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="1a909-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1a909-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1a909-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="1a909-113">Not supported.</span></span>    |
|<span data-ttu-id="1a909-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="1a909-114">Application</span></span> | <span data-ttu-id="1a909-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="1a909-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="1a909-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1a909-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="1a909-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="1a909-117">Request headers</span></span>
| <span data-ttu-id="1a909-118">名称</span><span class="sxs-lookup"><span data-stu-id="1a909-118">Name</span></span>       | <span data-ttu-id="1a909-119">类型</span><span class="sxs-lookup"><span data-stu-id="1a909-119">Type</span></span> | <span data-ttu-id="1a909-120">说明</span><span class="sxs-lookup"><span data-stu-id="1a909-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="1a909-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="1a909-121">Authorization</span></span>  | <span data-ttu-id="1a909-122">string</span><span class="sxs-lookup"><span data-stu-id="1a909-122">string</span></span>  | <span data-ttu-id="1a909-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="1a909-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="1a909-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="1a909-125">Request body</span></span>
<span data-ttu-id="1a909-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="1a909-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="1a909-127">响应</span><span class="sxs-lookup"><span data-stu-id="1a909-127">Response</span></span>

<span data-ttu-id="1a909-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和 password 对象。</span><span class="sxs-lookup"><span data-stu-id="1a909-128">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="1a909-129">Azure AD 生成通过`secretText`属性返回的强密码。</span><span class="sxs-lookup"><span data-stu-id="1a909-129">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="1a909-130">将来无法检索此密码。</span><span class="sxs-lookup"><span data-stu-id="1a909-130">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="1a909-131">示例</span><span class="sxs-lookup"><span data-stu-id="1a909-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1a909-132">请求</span><span class="sxs-lookup"><span data-stu-id="1a909-132">Request</span></span>
<span data-ttu-id="1a909-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="1a909-133">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="1a909-134">响应</span><span class="sxs-lookup"><span data-stu-id="1a909-134">Response</span></span>
<span data-ttu-id="1a909-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="1a909-135">Here is an example of the response.</span></span>

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
