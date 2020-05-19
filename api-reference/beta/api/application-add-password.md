---
title: 添加应用程序密码
description: 向应用程序添加强密码。
author: sureshja
localization_priority: Normal
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 944c0a2e30a7202ad85510be84ef8b426059f4b6
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44289395"
---
# <a name="add-application-password"></a><span data-ttu-id="2e561-103">添加应用程序密码</span><span class="sxs-lookup"><span data-stu-id="2e561-103">Add application password</span></span>

<span data-ttu-id="2e561-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e561-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e561-105">向应用程序添加强密码。</span><span class="sxs-lookup"><span data-stu-id="2e561-105">Adds a strong password to an application.</span></span>

## <a name="permissions"></a><span data-ttu-id="2e561-106">权限</span><span class="sxs-lookup"><span data-stu-id="2e561-106">Permissions</span></span>
<span data-ttu-id="2e561-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="2e561-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="2e561-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="2e561-109">Permission type</span></span>      | <span data-ttu-id="2e561-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="2e561-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="2e561-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="2e561-111">Delegated (work or school account)</span></span> | <span data-ttu-id="2e561-112">所有的 Directory.accessasuser.all，all，all，All</span><span class="sxs-lookup"><span data-stu-id="2e561-112">Application.ReadWrite.All, Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="2e561-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="2e561-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="2e561-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="2e561-114">Not supported.</span></span>    |
|<span data-ttu-id="2e561-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="2e561-115">Application</span></span> | <span data-ttu-id="2e561-116">Application.readwrite.ownedby、所有的 readwrite、全部、读写。</span><span class="sxs-lookup"><span data-stu-id="2e561-116">Application.ReadWrite.OwnedBy, Application.ReadWrite.All, Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="2e561-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="2e561-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /applications/{id}/addPassword
```

## <a name="request-headers"></a><span data-ttu-id="2e561-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="2e561-118">Request headers</span></span>
| <span data-ttu-id="2e561-119">名称</span><span class="sxs-lookup"><span data-stu-id="2e561-119">Name</span></span>       | <span data-ttu-id="2e561-120">类型</span><span class="sxs-lookup"><span data-stu-id="2e561-120">Type</span></span> | <span data-ttu-id="2e561-121">说明</span><span class="sxs-lookup"><span data-stu-id="2e561-121">Description</span></span>|
|:-----------|:------|:----------|
| <span data-ttu-id="2e561-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="2e561-122">Authorization</span></span>  | <span data-ttu-id="2e561-123">string</span><span class="sxs-lookup"><span data-stu-id="2e561-123">string</span></span>  | <span data-ttu-id="2e561-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="2e561-p102">Bearer {token}. Required.</span></span>  |

## <a name="request-body"></a><span data-ttu-id="2e561-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="2e561-126">Request body</span></span>
<span data-ttu-id="2e561-127">请勿提供此方法的请求正文。</span><span class="sxs-lookup"><span data-stu-id="2e561-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="2e561-128">响应</span><span class="sxs-lookup"><span data-stu-id="2e561-128">Response</span></span>

<span data-ttu-id="2e561-129">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和 password 对象。</span><span class="sxs-lookup"><span data-stu-id="2e561-129">If successful, this method returns a `200 OK` response code and password object in the response body.</span></span> <span data-ttu-id="2e561-130">Azure AD 生成通过属性返回的强密码 `secretText` 。</span><span class="sxs-lookup"><span data-stu-id="2e561-130">Azure AD generates a strong password which is returned via the `secretText` property.</span></span> <span data-ttu-id="2e561-131">将来无法检索此密码。</span><span class="sxs-lookup"><span data-stu-id="2e561-131">There is no way to retrieve this password in the future.</span></span>

## <a name="example"></a><span data-ttu-id="2e561-132">示例</span><span class="sxs-lookup"><span data-stu-id="2e561-132">Example</span></span>
##### <a name="request"></a><span data-ttu-id="2e561-133">请求</span><span class="sxs-lookup"><span data-stu-id="2e561-133">Request</span></span>
<span data-ttu-id="2e561-134">下面展示了示例请求。</span><span class="sxs-lookup"><span data-stu-id="2e561-134">The following is an example of the request.</span></span>

```http
POST https://graph.microsoft.com/beta/applications/{id}/addPassword
```
##### <a name="response"></a><span data-ttu-id="2e561-135">响应</span><span class="sxs-lookup"><span data-stu-id="2e561-135">Response</span></span>
<span data-ttu-id="2e561-136">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="2e561-136">The following is an example of the response.</span></span>

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
