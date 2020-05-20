---
title: 创建 serviceprincipal
description: 创建新的 serviceprincipal 对象。
author: davidmu1
localization_priority: Priority
doc_type: apiPageType
ms.prod: microsoft-identity-platform
ms.openlocfilehash: 439f7c4e41d665eaaa7ce41b2b4372fdd9016388
ms.sourcegitcommit: 87966dcd42a0111c5c9987fcae0a491c92022938
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 05/19/2020
ms.locfileid: "44291095"
---
# <a name="create-serviceprincipal"></a><span data-ttu-id="407fb-103">创建 servicePrincipal</span><span class="sxs-lookup"><span data-stu-id="407fb-103">Create servicePrincipal</span></span>

<span data-ttu-id="407fb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="407fb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="407fb-105">创建新的[servicePrincipal](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="407fb-105">Create a new [servicePrincipal](../resources/serviceprincipal.md) object.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="407fb-106">不支持在创建 servicePrincipals 时添加[**passwordCredential**](../resources/passwordcredential.md) 。</span><span class="sxs-lookup"><span data-stu-id="407fb-106">Adding [**passwordCredential**](../resources/passwordcredential.md) when creating servicePrincipals is not supported.</span></span> <span data-ttu-id="407fb-107">使用[addPassword](serviceprincipal-addpassword.md)方法可添加 servicePrincipal 的密码。</span><span class="sxs-lookup"><span data-stu-id="407fb-107">Use the [addPassword](serviceprincipal-addpassword.md) method to add passwords for a servicePrincipal.</span></span>

## <a name="permissions"></a><span data-ttu-id="407fb-108">Permissions</span><span class="sxs-lookup"><span data-stu-id="407fb-108">Permissions</span></span>
<span data-ttu-id="407fb-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="407fb-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>


|<span data-ttu-id="407fb-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="407fb-111">Permission type</span></span>      | <span data-ttu-id="407fb-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="407fb-112">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="407fb-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="407fb-113">Delegated (work or school account)</span></span> | <span data-ttu-id="407fb-114">Directory.accessasuser.all 的所有应用程序。</span><span class="sxs-lookup"><span data-stu-id="407fb-114">Application.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="407fb-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="407fb-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="407fb-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="407fb-116">Not supported.</span></span>    |
|<span data-ttu-id="407fb-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="407fb-117">Application</span></span> | <span data-ttu-id="407fb-118">Application.ReadWrite.OwnedBy、Application.ReadWrite.All、Directory.Read.All</span><span class="sxs-lookup"><span data-stu-id="407fb-118">Application.ReadWrite.OwnedBy, Application.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="407fb-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="407fb-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /serviceprincipals
```

## <a name="request-headers"></a><span data-ttu-id="407fb-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="407fb-120">Request headers</span></span>
| <span data-ttu-id="407fb-121">名称</span><span class="sxs-lookup"><span data-stu-id="407fb-121">Name</span></span>       | <span data-ttu-id="407fb-122">说明</span><span class="sxs-lookup"><span data-stu-id="407fb-122">Description</span></span>|
|:-----------|:----------|
| <span data-ttu-id="407fb-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="407fb-123">Authorization</span></span> | <span data-ttu-id="407fb-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="407fb-p103">Bearer {token}. Required.</span></span>  |
| <span data-ttu-id="407fb-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="407fb-126">Content-Type</span></span> | <span data-ttu-id="407fb-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="407fb-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="407fb-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="407fb-129">Request body</span></span>
<span data-ttu-id="407fb-130">在请求正文中，提供[serviceprincipal](../resources/serviceprincipal.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="407fb-130">In the request body, supply a JSON representation of a [serviceprincipal](../resources/serviceprincipal.md) object.</span></span> <span data-ttu-id="407fb-131">请求正文必须包含**appId**。</span><span class="sxs-lookup"><span data-stu-id="407fb-131">The request body must contain  **appId**.</span></span>

## <a name="response"></a><span data-ttu-id="407fb-132">响应</span><span class="sxs-lookup"><span data-stu-id="407fb-132">Response</span></span>

<span data-ttu-id="407fb-133">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和[serviceprincipal](../resources/serviceprincipal.md)对象。</span><span class="sxs-lookup"><span data-stu-id="407fb-133">If successful, this method returns a `201 Created` response code and a [serviceprincipal](../resources/serviceprincipal.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="407fb-134">示例</span><span class="sxs-lookup"><span data-stu-id="407fb-134">Examples</span></span>
### <a name="request"></a><span data-ttu-id="407fb-135">请求</span><span class="sxs-lookup"><span data-stu-id="407fb-135">Request</span></span>
<span data-ttu-id="407fb-136">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="407fb-136">Here is an example of the request.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_serviceprincipal_from_serviceprincipals"
}-->
```http
POST https://graph.microsoft.com/v1.0/serviceprincipals
Content-type: application/json

{
  "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
}
```

### <a name="response"></a><span data-ttu-id="407fb-137">响应</span><span class="sxs-lookup"><span data-stu-id="407fb-137">Response</span></span>
<span data-ttu-id="407fb-138">下面是一个响应示例。</span><span class="sxs-lookup"><span data-stu-id="407fb-138">Here is an example of the response.</span></span> 

> <span data-ttu-id="407fb-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="407fb-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.servicePrincipal"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "@odata.context": "https://graph.microsoft.com/v1.0/$metadata#servicePrincipals/$entity",
    "id": "59e617e5-e447-4adc-8b88-00af644d7c92",
    "deletedDateTime": null,
    "accountEnabled": true,
    "appDisplayName": "My App",
    "appId": "65415bb1-9267-4313-bbf5-ae259732ee12",
    "appOwnerOrganizationId": "1bc1c026-2f7b-48a5-98da-afa2fd8bc7bc",
    "appRoleAssignmentRequired": false,
    "displayName": "foo",
    "homepage": null,
    "logoutUrl": null,
    "publisherName": "Contoso",
    "replyUrls": [],
    "servicePrincipalNames": [
        "f1bd758f-4a1a-4b71-aa20-a248a22a8928"
    ],
    "tags": [],
    "addIns": [],
    "appRoles": [],
    "info": {
        "termsOfServiceUrl": null,
        "supportUrl": null,
        "privacyStatementUrl": null,
        "marketingUrl": null,
        "logoUrl": null
    },
    "keyCredentials": [],
    "oauth2PermissionScopes": [],
    "passwordCredentials": []
}
```
