---
title: 创建 connectorGroup
description: 使用此 API 创建新的 connectorGroup。
localization_priority: Normal
ms.openlocfilehash: 233a80366c89b8cba31bd24e5d69b3a83fc20d1c
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455791"
---
# <a name="create-connectorgroup"></a><span data-ttu-id="590be-103">创建 connectorGroup</span><span class="sxs-lookup"><span data-stu-id="590be-103">Create connectorGroup</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="590be-104">使用此 API 创建新的 connectorGroup。</span><span class="sxs-lookup"><span data-stu-id="590be-104">Use this API to create a new connectorGroup.</span></span>
## <a name="permissions"></a><span data-ttu-id="590be-105">权限</span><span class="sxs-lookup"><span data-stu-id="590be-105">Permissions</span></span>
<span data-ttu-id="590be-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="590be-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="590be-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="590be-108">Permission type</span></span>      | <span data-ttu-id="590be-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="590be-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="590be-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="590be-110">Delegated (work or school account)</span></span> | <span data-ttu-id="590be-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="590be-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="590be-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="590be-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="590be-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="590be-113">Not supported.</span></span>    |
|<span data-ttu-id="590be-114">Application</span><span class="sxs-lookup"><span data-stu-id="590be-114">Application</span></span> | <span data-ttu-id="590be-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="590be-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="590be-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="590be-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /connectorGroups

```
## <a name="request-headers"></a><span data-ttu-id="590be-117">请求标头</span><span class="sxs-lookup"><span data-stu-id="590be-117">Request headers</span></span>
| <span data-ttu-id="590be-118">名称</span><span class="sxs-lookup"><span data-stu-id="590be-118">Name</span></span>       | <span data-ttu-id="590be-119">说明</span><span class="sxs-lookup"><span data-stu-id="590be-119">Description</span></span>|
|:---------------|:----------|
| <span data-ttu-id="590be-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="590be-120">Authorization</span></span>  | <span data-ttu-id="590be-121">负载.</span><span class="sxs-lookup"><span data-stu-id="590be-121">Bearer.</span></span> <span data-ttu-id="590be-122">Requried</span><span class="sxs-lookup"><span data-stu-id="590be-122">Requried</span></span>|

## <a name="request-body"></a><span data-ttu-id="590be-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="590be-123">Request body</span></span>
<span data-ttu-id="590be-124">在请求正文中, 提供[connectorGroup](../resources/connectorgroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="590be-124">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>

## <a name="response"></a><span data-ttu-id="590be-125">响应</span><span class="sxs-lookup"><span data-stu-id="590be-125">Response</span></span>

<span data-ttu-id="590be-126">如果成功, 此方法在`201 Created`响应正文中返回响应代码和[connectorGroup](../resources/connectorgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="590be-126">If successful, this method returns `201 Created` response code and [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="590be-127">示例</span><span class="sxs-lookup"><span data-stu-id="590be-127">Example</span></span>
##### <a name="request"></a><span data-ttu-id="590be-128">请求</span><span class="sxs-lookup"><span data-stu-id="590be-128">Request</span></span>
<span data-ttu-id="590be-129">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="590be-129">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "create_connectorgroup_from_connectorgroups"
}-->
```http
POST https://graph.microsoft.com/{ver}/connectorGroups
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": false
}
```
<span data-ttu-id="590be-130">在请求正文中, 提供[connectorGroup](../resources/connectorgroup.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="590be-130">In the request body, supply a JSON representation of [connectorGroup](../resources/connectorgroup.md) object.</span></span>
##### <a name="response"></a><span data-ttu-id="590be-131">响应</span><span class="sxs-lookup"><span data-stu-id="590be-131">Response</span></span>
<span data-ttu-id="590be-p103">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="590be-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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
    "Error: /api-reference/beta/api/connectorgroup-post-connectorgroups.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
