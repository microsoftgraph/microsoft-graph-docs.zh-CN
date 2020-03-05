---
title: 添加应用程序密码
description: 向应用程序添加强密码。
author: davidmu1
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 980f2bdc9d43d5d8e854c92a016d9c40b68d3745
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42441569"
---
# <a name="add-application-password"></a><span data-ttu-id="ddf7d-103">添加应用程序密码</span><span class="sxs-lookup"><span data-stu-id="ddf7d-103">Add application password</span></span>

<span data-ttu-id="ddf7d-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ddf7d-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ddf7d-105">向应用程序添加强密码。</span><span class="sxs-lookup"><span data-stu-id="ddf7d-105">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="ddf7d-106">权限</span><span class="sxs-lookup"><span data-stu-id="ddf7d-106">Permissions</span></span>
<span data-ttu-id="ddf7d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ddf7d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ddf7d-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ddf7d-109">Permission type</span></span>      | <span data-ttu-id="ddf7d-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ddf7d-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ddf7d-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ddf7d-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ddf7d-112">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ddf7d-112">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ddf7d-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ddf7d-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ddf7d-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ddf7d-114">Not supported.</span></span>    |
|<span data-ttu-id="ddf7d-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ddf7d-115">Application</span></span> | <span data-ttu-id="ddf7d-116">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="ddf7d-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ddf7d-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ddf7d-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="ddf7d-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ddf7d-118">Request headers</span></span>
| <span data-ttu-id="ddf7d-119">名称</span><span class="sxs-lookup"><span data-stu-id="ddf7d-119">Name</span></span>       | <span data-ttu-id="ddf7d-120">类型</span><span class="sxs-lookup"><span data-stu-id="ddf7d-120">Type</span></span> | <span data-ttu-id="ddf7d-121">说明</span><span class="sxs-lookup"><span data-stu-id="ddf7d-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="ddf7d-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ddf7d-122">Authorization</span></span>  | <span data-ttu-id="ddf7d-123">string</span><span class="sxs-lookup"><span data-stu-id="ddf7d-123">string</span></span>  | <span data-ttu-id="ddf7d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="ddf7d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="ddf7d-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="ddf7d-126">Request body</span></span>
<span data-ttu-id="ddf7d-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="ddf7d-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="ddf7d-128">响应</span><span class="sxs-lookup"><span data-stu-id="ddf7d-128">Response</span></span>

<span data-ttu-id="ddf7d-129">如果成功，此方法在响应`200 OK`正文中返回响应代码和 password 对象。</span><span class="sxs-lookup"><span data-stu-id="ddf7d-129">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="ddf7d-130">Azure AD 生成通过`secretText`属性返回的强密码。</span><span class="sxs-lookup"><span data-stu-id="ddf7d-130">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="ddf7d-131">将来无法检索此密码。</span><span class="sxs-lookup"><span data-stu-id="ddf7d-131">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="ddf7d-132">示例</span><span class="sxs-lookup"><span data-stu-id="ddf7d-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ddf7d-133">请求</span><span class="sxs-lookup"><span data-stu-id="ddf7d-133">Request</span></span>
<span data-ttu-id="ddf7d-134">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ddf7d-134">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="ddf7d-135">响应</span><span class="sxs-lookup"><span data-stu-id="ddf7d-135">Response</span></span>
<span data-ttu-id="ddf7d-136">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="ddf7d-136">Here is an example of the response.</span></span>

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
