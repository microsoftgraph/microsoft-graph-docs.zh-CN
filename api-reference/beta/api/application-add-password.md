---
title: 添加应用程序密码
description: 向应用程序中的强密码。
author: lleonard-msft
localization_priority: Normal
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 565fbab9ff2cde34bcccbe760692df9d3c0d1a14
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/12/2019
ms.locfileid: "27966760"
---
# <a name="add-application-password"></a><span data-ttu-id="fe72e-103">添加应用程序密码</span><span class="sxs-lookup"><span data-stu-id="fe72e-103">Add application password</span></span>

> <span data-ttu-id="fe72e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="fe72e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="fe72e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="fe72e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="fe72e-106">向应用程序中的强密码。</span><span class="sxs-lookup"><span data-stu-id="fe72e-106">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="fe72e-107">权限</span><span class="sxs-lookup"><span data-stu-id="fe72e-107">Permissions</span></span>
<span data-ttu-id="fe72e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="fe72e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="fe72e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="fe72e-110">Permission type</span></span>      | <span data-ttu-id="fe72e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="fe72e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="fe72e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="fe72e-112">Delegated (work or school account)</span></span> | <span data-ttu-id="fe72e-113">Directory.Read.All、Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="fe72e-113">Directory.Read.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="fe72e-114">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="fe72e-114">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="fe72e-115">不支持。</span><span class="sxs-lookup"><span data-stu-id="fe72e-115">Not supported.</span></span>    |
|<span data-ttu-id="fe72e-116">应用程序</span><span class="sxs-lookup"><span data-stu-id="fe72e-116">Application</span></span> | <span data-ttu-id="fe72e-117">Application.ReadWrite.OwnedBy，Application.ReadWrite.All，Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="fe72e-117">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.Read.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="fe72e-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="fe72e-118">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="fe72e-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="fe72e-119">Request headers</span></span>
| <span data-ttu-id="fe72e-120">名称</span><span class="sxs-lookup"><span data-stu-id="fe72e-120">Name</span></span>       | <span data-ttu-id="fe72e-121">类型</span><span class="sxs-lookup"><span data-stu-id="fe72e-121">Type</span></span> | <span data-ttu-id="fe72e-122">说明</span><span class="sxs-lookup"><span data-stu-id="fe72e-122">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="fe72e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="fe72e-123">Authorization</span></span>  | <span data-ttu-id="fe72e-124">string</span><span class="sxs-lookup"><span data-stu-id="fe72e-124">string</span></span>  | <span data-ttu-id="fe72e-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="fe72e-p103">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="fe72e-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="fe72e-127">Request body</span></span>
<span data-ttu-id="fe72e-128">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="fe72e-128">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="fe72e-129">响应</span><span class="sxs-lookup"><span data-stu-id="fe72e-129">Response</span></span>

<span data-ttu-id="fe72e-130">如果成功，此方法返回`200 OK`响应正文中的响应代码和密码对象。</span><span class="sxs-lookup"><span data-stu-id="fe72e-130">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="fe72e-131">Azure AD 将生成一个强密码通过返回的`secretText`属性。</span><span class="sxs-lookup"><span data-stu-id="fe72e-131">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="fe72e-132">没有方法，以便将来检索此密码。</span><span class="sxs-lookup"><span data-stu-id="fe72e-132">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="fe72e-133">示例</span><span class="sxs-lookup"><span data-stu-id="fe72e-133">Example</span></span>
##### <a name="request"></a><span data-ttu-id="fe72e-134">请求</span><span class="sxs-lookup"><span data-stu-id="fe72e-134">Request</span></span>
<span data-ttu-id="fe72e-135">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="fe72e-135">Here is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="fe72e-136">响应</span><span class="sxs-lookup"><span data-stu-id="fe72e-136">Response</span></span>
<span data-ttu-id="fe72e-137">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="fe72e-137">Here is an example of the response.</span></span>

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
