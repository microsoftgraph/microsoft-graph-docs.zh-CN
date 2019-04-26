---
title: 创建应用程序
description: 使用此 API 新建应用程序。
localization_priority: Normal
ms.openlocfilehash: ee0ecc6db99c0ea92131dbbf0e9c028234925f0a
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33327480"
---
# <a name="create-application"></a><span data-ttu-id="c66ba-103">创建应用程序</span><span class="sxs-lookup"><span data-stu-id="c66ba-103">Create application</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c66ba-104">使用此 API 新建应用程序。</span><span class="sxs-lookup"><span data-stu-id="c66ba-104">Use this API to create a new application.</span></span>
## <a name="permissions"></a><span data-ttu-id="c66ba-105">权限</span><span class="sxs-lookup"><span data-stu-id="c66ba-105">Permissions</span></span>
<span data-ttu-id="c66ba-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c66ba-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c66ba-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c66ba-108">Permission type</span></span>      | <span data-ttu-id="c66ba-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c66ba-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c66ba-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c66ba-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c66ba-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c66ba-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c66ba-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c66ba-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c66ba-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c66ba-113">Not supported.</span></span>    |
|<span data-ttu-id="c66ba-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c66ba-114">Application</span></span> | <span data-ttu-id="c66ba-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c66ba-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c66ba-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c66ba-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups/{id}/applications

```
## <a name="request-headers"></a><span data-ttu-id="c66ba-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c66ba-117">Request headers</span></span>
| <span data-ttu-id="c66ba-118">名称</span><span class="sxs-lookup"><span data-stu-id="c66ba-118">Name</span></span>       | <span data-ttu-id="c66ba-119">说明</span><span class="sxs-lookup"><span data-stu-id="c66ba-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c66ba-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c66ba-120">Authorization</span></span>  | <span data-ttu-id="c66ba-121">负载.</span><span class="sxs-lookup"><span data-stu-id="c66ba-121">Bearer.</span></span> <span data-ttu-id="c66ba-122">必需</span><span class="sxs-lookup"><span data-stu-id="c66ba-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="c66ba-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="c66ba-123">Request body</span></span>
<span data-ttu-id="c66ba-124">在请求正文中，提供 [application](../resources/application.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c66ba-124">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c66ba-125">响应</span><span class="sxs-lookup"><span data-stu-id="c66ba-125">Response</span></span>

<span data-ttu-id="c66ba-126">如果成功，此方法在响应正文中返回 `201 Created` 响应代码和 [application](../resources/application.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="c66ba-126">If successful, this method returns `201 Created` response code and [application](../resources/application.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c66ba-127">示例</span><span class="sxs-lookup"><span data-stu-id="c66ba-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c66ba-128">请求</span><span class="sxs-lookup"><span data-stu-id="c66ba-128">Request</span></span>
<span data-ttu-id="c66ba-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c66ba-129">Here is an example of the request.</span></span>
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
<span data-ttu-id="c66ba-130">在请求正文中，提供 [application](../resources/application.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c66ba-130">In the request body, supply a JSON representation of [application](../resources/application.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c66ba-131">响应</span><span class="sxs-lookup"><span data-stu-id="c66ba-131">Response</span></span>
<span data-ttu-id="c66ba-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c66ba-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
