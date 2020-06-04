---
title: 将应用程序添加到 connectorGroup
description: 使用此 API 将应用程序分配给连接器组
localization_priority: Normal
author: japere
ms.prod: microsoft-identity-platform
doc_type: apiPageType
ms.openlocfilehash: 7843d1fa661bfcaf209fbdfee52f08f96427a37f
ms.sourcegitcommit: b2e216de4a649606c961b3ed2aa3eb8a65f2355c
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 06/04/2020
ms.locfileid: "44555774"
---
# <a name="add-an-application-to-a-connectorgroup"></a><span data-ttu-id="554b3-103">将应用程序添加到 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="554b3-103">Add an application to a connectorGroup</span></span>

<span data-ttu-id="554b3-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="554b3-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="554b3-105">将[应用程序](../resources/application.md)添加到[connectorGroup](../resources/connectorgroup.md)。</span><span class="sxs-lookup"><span data-stu-id="554b3-105">Add an [application](../resources/application.md) to a [connectorGroup](../resources/connectorgroup.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="554b3-106">Permissions</span><span class="sxs-lookup"><span data-stu-id="554b3-106">Permissions</span></span>
<span data-ttu-id="554b3-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="554b3-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="554b3-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="554b3-109">Permission type</span></span>      | <span data-ttu-id="554b3-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="554b3-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="554b3-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="554b3-111">Delegated (work or school account)</span></span> | <span data-ttu-id="554b3-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="554b3-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="554b3-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="554b3-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="554b3-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="554b3-114">Not supported.</span></span>    |
|<span data-ttu-id="554b3-115">Application</span><span class="sxs-lookup"><span data-stu-id="554b3-115">Application</span></span> | <span data-ttu-id="554b3-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="554b3-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="554b3-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="554b3-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications

```
## <a name="request-headers"></a><span data-ttu-id="554b3-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="554b3-118">Request headers</span></span>
| <span data-ttu-id="554b3-119">名称</span><span class="sxs-lookup"><span data-stu-id="554b3-119">Name</span></span>       | <span data-ttu-id="554b3-120">说明</span><span class="sxs-lookup"><span data-stu-id="554b3-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="554b3-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="554b3-121">Authorization</span></span>  | <span data-ttu-id="554b3-122">负载.</span><span class="sxs-lookup"><span data-stu-id="554b3-122">Bearer.</span></span> <span data-ttu-id="554b3-123">必需</span><span class="sxs-lookup"><span data-stu-id="554b3-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="554b3-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="554b3-124">Request body</span></span>
<span data-ttu-id="554b3-125">在请求正文中，提供 [application](../resources/application.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="554b3-125">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="554b3-126">响应</span><span class="sxs-lookup"><span data-stu-id="554b3-126">Response</span></span>

<span data-ttu-id="554b3-127">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [application](../resources/application.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="554b3-127">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="554b3-128">示例</span><span class="sxs-lookup"><span data-stu-id="554b3-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="554b3-129">请求</span><span class="sxs-lookup"><span data-stu-id="554b3-129">Request</span></span>
<span data-ttu-id="554b3-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="554b3-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_application_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/beta/onPremisesPublishingProfiles/applicationProxy/connectorGroups/{id}/applications
Content-type: application/json
Content-length: 329

{
  "@odata.id": "https://graph.microsoft.com/beta/applications/{id}"
}
```
<span data-ttu-id="554b3-131">在请求正文中，提供 [application](../resources/application.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="554b3-131">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="554b3-132">响应</span><span class="sxs-lookup"><span data-stu-id="554b3-132">Response</span></span>
<span data-ttu-id="554b3-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="554b3-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.application"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 355

{
  "appId": "appId-value",
  "onPremisesPublishing": {
    "externalUrl": "externalUrl-value",
    "internalUrl": "internalUrl-value",
    "externalAuthenticationType": "externalAuthenticationType-value",
    "customDomainCertificate": "customDomainCertificate-value",
    "isTranslateHostHeaderEnabled": true,
    "isOnPremPublishingEnabled": true
  }
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create application",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
