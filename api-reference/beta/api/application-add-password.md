---
title: 添加应用程序密码
description: 向应用程序添加强密码。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: dc1e0ebb215ef478c9eedbb44a0d328f35693972
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33322654"
---
# <a name="add-application-password"></a><span data-ttu-id="0ea4d-103">添加应用程序密码</span><span class="sxs-lookup"><span data-stu-id="0ea4d-103">Add application password</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="0ea4d-104">向应用程序添加强密码。</span><span class="sxs-lookup"><span data-stu-id="0ea4d-104">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="0ea4d-105">权限</span><span class="sxs-lookup"><span data-stu-id="0ea4d-105">Permissions</span></span>
<span data-ttu-id="0ea4d-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0ea4d-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0ea4d-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="0ea4d-108">Permission type</span></span>      | <span data-ttu-id="0ea4d-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0ea4d-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0ea4d-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0ea4d-110">Delegated (work or school account)</span></span> | <span data-ttu-id="0ea4d-111">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="0ea4d-111">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="0ea4d-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0ea4d-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0ea4d-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="0ea4d-113">Not supported.</span></span>    |
|<span data-ttu-id="0ea4d-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="0ea4d-114">Application</span></span> | <span data-ttu-id="0ea4d-115">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="0ea4d-115">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="0ea4d-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0ea4d-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="0ea4d-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="0ea4d-117">Request headers</span></span>
| <span data-ttu-id="0ea4d-118">名称</span><span class="sxs-lookup"><span data-stu-id="0ea4d-118">Name</span></span>       | <span data-ttu-id="0ea4d-119">类型</span><span class="sxs-lookup"><span data-stu-id="0ea4d-119">Type</span></span> | <span data-ttu-id="0ea4d-120">说明</span><span class="sxs-lookup"><span data-stu-id="0ea4d-120">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="0ea4d-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="0ea4d-121">Authorization</span></span>  | <span data-ttu-id="0ea4d-122">string</span><span class="sxs-lookup"><span data-stu-id="0ea4d-122">string</span></span>  | <span data-ttu-id="0ea4d-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0ea4d-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="0ea4d-125">请求正文</span><span class="sxs-lookup"><span data-stu-id="0ea4d-125">Request body</span></span>
<span data-ttu-id="0ea4d-126">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="0ea4d-126">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="0ea4d-127">响应</span><span class="sxs-lookup"><span data-stu-id="0ea4d-127">Response</span></span>

<span data-ttu-id="0ea4d-128">如果成功, 此方法在响应`200 OK`正文中返回响应代码和 password 对象。</span><span class="sxs-lookup"><span data-stu-id="0ea4d-128">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="0ea4d-129">Azure AD 生成通过`secretText`属性返回的强密码。</span><span class="sxs-lookup"><span data-stu-id="0ea4d-129">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="0ea4d-130">将来无法检索此密码。</span><span class="sxs-lookup"><span data-stu-id="0ea4d-130">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="0ea4d-131">示例</span><span class="sxs-lookup"><span data-stu-id="0ea4d-131">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0ea4d-132">请求</span><span class="sxs-lookup"><span data-stu-id="0ea4d-132">Request</span></span>
<span data-ttu-id="0ea4d-133">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0ea4d-133">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="0ea4d-134">响应</span><span class="sxs-lookup"><span data-stu-id="0ea4d-134">Response</span></span>
<span data-ttu-id="0ea4d-135">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="0ea4d-135">Here is an example of the response.</span></span>

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
