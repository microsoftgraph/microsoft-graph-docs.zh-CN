---
title: 创建应用程序
description: 使用此 API 新建应用程序。
localization_priority: Normal
doc_type: apiPageType
ms.prod: ''
author: ''
ms.openlocfilehash: 018288444be3c2851e71117e1710a08947fa6104
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42437355"
---
# <a name="create-application"></a><span data-ttu-id="ea7ce-103">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="ea7ce-103">Create application</span></span>

<span data-ttu-id="ea7ce-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="ea7ce-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ea7ce-105">使用此 API 新建应用程序。</span><span class="sxs-lookup"><span data-stu-id="ea7ce-105">Use this API to create a new application.</span></span>
## <a name="permissions"></a><span data-ttu-id="ea7ce-106">权限</span><span class="sxs-lookup"><span data-stu-id="ea7ce-106">Permissions</span></span>
<span data-ttu-id="ea7ce-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ea7ce-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ea7ce-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="ea7ce-109">Permission type</span></span>      | <span data-ttu-id="ea7ce-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ea7ce-110">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ea7ce-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ea7ce-111">Delegated (work or school account)</span></span> | <span data-ttu-id="ea7ce-112">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ea7ce-112">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ea7ce-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ea7ce-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ea7ce-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="ea7ce-114">Not supported.</span></span>    |
|<span data-ttu-id="ea7ce-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="ea7ce-115">Application</span></span> | <span data-ttu-id="ea7ce-116">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ea7ce-116">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ea7ce-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ea7ce-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/applications

```
## <a name="request-headers"></a><span data-ttu-id="ea7ce-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="ea7ce-118">Request headers</span></span>
| <span data-ttu-id="ea7ce-119">名称</span><span class="sxs-lookup"><span data-stu-id="ea7ce-119">Name</span></span>       | <span data-ttu-id="ea7ce-120">说明</span><span class="sxs-lookup"><span data-stu-id="ea7ce-120">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="ea7ce-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="ea7ce-121">Authorization</span></span>  | <span data-ttu-id="ea7ce-122">负载.</span><span class="sxs-lookup"><span data-stu-id="ea7ce-122">Bearer.</span></span> <span data-ttu-id="ea7ce-123">必需</span><span class="sxs-lookup"><span data-stu-id="ea7ce-123">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="ea7ce-124">请求正文</span><span class="sxs-lookup"><span data-stu-id="ea7ce-124">Request body</span></span>
<span data-ttu-id="ea7ce-125">在请求正文中，提供 [application](../resources/application.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea7ce-125">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="ea7ce-126">响应</span><span class="sxs-lookup"><span data-stu-id="ea7ce-126">Response</span></span>

<span data-ttu-id="ea7ce-127">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [application](../resources/application.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="ea7ce-127">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ea7ce-128">示例</span><span class="sxs-lookup"><span data-stu-id="ea7ce-128">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ea7ce-129">请求</span><span class="sxs-lookup"><span data-stu-id="ea7ce-129">Request</span></span>
<span data-ttu-id="ea7ce-130">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ea7ce-130">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_application_from_connectorgroup"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups/{id}/applications
Content-type: application/json
Content-length: 329

{
  "@odata.id": "https://graph.microsoft.com/{ver}/applications/{id}"
}
```
<span data-ttu-id="ea7ce-131">在请求正文中，提供 [application](../resources/application.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ea7ce-131">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="ea7ce-132">响应</span><span class="sxs-lookup"><span data-stu-id="ea7ce-132">Response</span></span>
<span data-ttu-id="ea7ce-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ea7ce-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
