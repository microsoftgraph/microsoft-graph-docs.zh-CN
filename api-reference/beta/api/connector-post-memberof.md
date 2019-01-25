---
title: 添加到 connectorGroup 连接器
description: 使用此 API 添加到新 connectorGroup 连接符。
localization_priority: Normal
ms.openlocfilehash: 097f24233ec1c540885d67b60a4b471ff1c64f65
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29514626"
---
# <a name="add-connector-to-connectorgroup"></a><span data-ttu-id="c69b2-103">添加到 connectorGroup 连接器</span><span class="sxs-lookup"><span data-stu-id="c69b2-103">Add Connector to connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c69b2-104">使用此 API 添加到新 connectorGroup 连接符。</span><span class="sxs-lookup"><span data-stu-id="c69b2-104">Use this API to add a connector to a new connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="c69b2-105">权限</span><span class="sxs-lookup"><span data-stu-id="c69b2-105">Permissions</span></span>
<span data-ttu-id="c69b2-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="c69b2-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="c69b2-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="c69b2-108">Permission type</span></span>      | <span data-ttu-id="c69b2-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="c69b2-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="c69b2-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="c69b2-110">Delegated (work or school account)</span></span> | <span data-ttu-id="c69b2-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="c69b2-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="c69b2-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="c69b2-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="c69b2-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="c69b2-113">Not supported.</span></span>    |
|<span data-ttu-id="c69b2-114">应用程序</span><span class="sxs-lookup"><span data-stu-id="c69b2-114">Application</span></span> | <span data-ttu-id="c69b2-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="c69b2-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="c69b2-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="c69b2-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectors/{id}/memberOf

```
## <a name="request-headers"></a><span data-ttu-id="c69b2-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="c69b2-117">Request headers</span></span>
| <span data-ttu-id="c69b2-118">名称</span><span class="sxs-lookup"><span data-stu-id="c69b2-118">Name</span></span>       | <span data-ttu-id="c69b2-119">说明</span><span class="sxs-lookup"><span data-stu-id="c69b2-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="c69b2-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="c69b2-120">Authorization</span></span>  | <span data-ttu-id="c69b2-121">Bearer </span><span class="sxs-lookup"><span data-stu-id="c69b2-121">Bearer.</span></span> <span data-ttu-id="c69b2-122">必需</span><span class="sxs-lookup"><span data-stu-id="c69b2-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="c69b2-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="c69b2-123">Request body</span></span>
<span data-ttu-id="c69b2-124">在请求正文中，提供[connectorGroup](../resources/connectorgroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c69b2-124">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="c69b2-125">响应</span><span class="sxs-lookup"><span data-stu-id="c69b2-125">Response</span></span>

<span data-ttu-id="c69b2-126">如果成功，此方法返回`201 Created`响应正文中的响应代码和[connectorGroup](../resources/connectorgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="c69b2-126">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="c69b2-127">示例</span><span class="sxs-lookup"><span data-stu-id="c69b2-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="c69b2-128">请求</span><span class="sxs-lookup"><span data-stu-id="c69b2-128">Request</span></span>
<span data-ttu-id="c69b2-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="c69b2-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connectorgroup_from_connector"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectors/{id}/memberOf
Content-type: application/json
Content-length: 99

{
  "@odata.id": "https://graph.microsoft.com/{ver}/connectorGroups/{id}"
}
```
<span data-ttu-id="c69b2-130">在请求正文中，提供[connectorGroup](../resources/connectorgroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c69b2-130">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="c69b2-131">响应</span><span class="sxs-lookup"><span data-stu-id="c69b2-131">Response</span></span>
<span data-ttu-id="c69b2-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="c69b2-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Create connectorGroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/connector-post-memberof.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
