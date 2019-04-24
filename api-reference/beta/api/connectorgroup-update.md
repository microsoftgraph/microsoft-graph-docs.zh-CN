---
title: 更新 connectorGroups
description: 更新 connectorgroup 对象的属性。
localization_priority: Normal
ms.openlocfilehash: 9d6feec19552aeeebe51ba0fab07e805c6f4a2bb
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32455763"
---
# <a name="update-connectorgroups"></a><span data-ttu-id="ad309-103">更新 connectorGroups</span><span class="sxs-lookup"><span data-stu-id="ad309-103">Update connectorGroups</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ad309-104">更新 connectorgroup 对象的属性。</span><span class="sxs-lookup"><span data-stu-id="ad309-104">Update the properties of connectorgroup object.</span></span>
## <a name="permissions"></a><span data-ttu-id="ad309-105">权限</span><span class="sxs-lookup"><span data-stu-id="ad309-105">Permissions</span></span>
<span data-ttu-id="ad309-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="ad309-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ad309-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="ad309-108">Permission type</span></span>      | <span data-ttu-id="ad309-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="ad309-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="ad309-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="ad309-110">Delegated (work or school account)</span></span> | <span data-ttu-id="ad309-111">Directory.ReadWrite.All、Directory.AccessAsUser.All</span><span class="sxs-lookup"><span data-stu-id="ad309-111">Directory.ReadWrite.All, Directory.AccessAsUser.All</span></span>    |
|<span data-ttu-id="ad309-112">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="ad309-112">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="ad309-113">不支持。</span><span class="sxs-lookup"><span data-stu-id="ad309-113">Not supported.</span></span>    |
|<span data-ttu-id="ad309-114">Application</span><span class="sxs-lookup"><span data-stu-id="ad309-114">Application</span></span> | <span data-ttu-id="ad309-115">Directory.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ad309-115">Directory.ReadWrite.All</span></span> |

## <a name="http-request"></a><span data-ttu-id="ad309-116">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="ad309-116">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /connectorGroups/{id}
```
## <a name="optional-request-headers"></a><span data-ttu-id="ad309-117">可选的请求标头</span><span class="sxs-lookup"><span data-stu-id="ad309-117">Optional request headers</span></span>
| <span data-ttu-id="ad309-118">名称</span><span class="sxs-lookup"><span data-stu-id="ad309-118">Name</span></span>       | <span data-ttu-id="ad309-119">说明</span><span class="sxs-lookup"><span data-stu-id="ad309-119">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="ad309-120">Authorization</span><span class="sxs-lookup"><span data-stu-id="ad309-120">Authorization</span></span>  | <span data-ttu-id="ad309-121">负载.</span><span class="sxs-lookup"><span data-stu-id="ad309-121">Bearer.</span></span> <span data-ttu-id="ad309-122">必需</span><span class="sxs-lookup"><span data-stu-id="ad309-122">Required</span></span>|

## <a name="request-body"></a><span data-ttu-id="ad309-123">请求正文</span><span class="sxs-lookup"><span data-stu-id="ad309-123">Request body</span></span>
<span data-ttu-id="ad309-p103">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="ad309-p103">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="ad309-127">属性</span><span class="sxs-lookup"><span data-stu-id="ad309-127">Property</span></span>     | <span data-ttu-id="ad309-128">类型</span><span class="sxs-lookup"><span data-stu-id="ad309-128">Type</span></span>   |<span data-ttu-id="ad309-129">描述</span><span class="sxs-lookup"><span data-stu-id="ad309-129">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ad309-130">connectorGroupType</span><span class="sxs-lookup"><span data-stu-id="ad309-130">connectorGroupType</span></span>|<span data-ttu-id="ad309-131">string</span><span class="sxs-lookup"><span data-stu-id="ad309-131">string</span></span>| <span data-ttu-id="ad309-132">可能的值是`applicationProxy`:。</span><span class="sxs-lookup"><span data-stu-id="ad309-132">Possible values are: `applicationProxy`.</span></span>|
|<span data-ttu-id="ad309-133">name</span><span class="sxs-lookup"><span data-stu-id="ad309-133">name</span></span>|<span data-ttu-id="ad309-134">String</span><span class="sxs-lookup"><span data-stu-id="ad309-134">String</span></span>|<span data-ttu-id="ad309-135">connectorGroup 的名称。</span><span class="sxs-lookup"><span data-stu-id="ad309-135">The name of the connectorGroup.</span></span>|

## <a name="response"></a><span data-ttu-id="ad309-136">响应</span><span class="sxs-lookup"><span data-stu-id="ad309-136">Response</span></span>

<span data-ttu-id="ad309-137">如果成功, 此方法在响应`200 OK`正文中返回响应代码和更新的[connectorGroup](../resources/connectorgroup.md)对象。</span><span class="sxs-lookup"><span data-stu-id="ad309-137">If successful, this method returns a `200 OK` response code and updated [connectorGroup](../resources/connectorgroup.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="ad309-138">示例</span><span class="sxs-lookup"><span data-stu-id="ad309-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="ad309-139">请求</span><span class="sxs-lookup"><span data-stu-id="ad309-139">Request</span></span>
<span data-ttu-id="ad309-140">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="ad309-140">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_connectorgroup"
}-->
```http
PATCH https://graph.microsoft.com/{ver}/connectorGroups/{id}
Content-type: application/json
Content-length: 99

{
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
}
```
##### <a name="response"></a><span data-ttu-id="ad309-141">响应</span><span class="sxs-lookup"><span data-stu-id="ad309-141">Response</span></span>
<span data-ttu-id="ad309-p104">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="ad309-p104">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.connectorGroup"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 119

{
  "id": "id-value",
  "name": "name-value",
  "connectorGroupType": "connectorGroupType-value",
  "isDefault": true
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "Update connectorgroup",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/connectorgroup-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
