---
title: 更新程序
description: 在 Azure AD 中访问审阅功能，则请更新现有程序对象。
localization_priority: Normal
ms.openlocfilehash: 75562aac5a7b3f3aaef0c8a1251d32a7728813aa
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29529920"
---
# <a name="update-program"></a><span data-ttu-id="70ba1-103">更新程序</span><span class="sxs-lookup"><span data-stu-id="70ba1-103">Update program</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="70ba1-104">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，更新现有[程序](../resources/program.md)对象。</span><span class="sxs-lookup"><span data-stu-id="70ba1-104">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="70ba1-105">权限</span><span class="sxs-lookup"><span data-stu-id="70ba1-105">Permissions</span></span>
<span data-ttu-id="70ba1-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="70ba1-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70ba1-108">权限类型</span><span class="sxs-lookup"><span data-stu-id="70ba1-108">Permission type</span></span>                        | <span data-ttu-id="70ba1-109">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="70ba1-109">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="70ba1-110">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="70ba1-110">Delegated (work or school account)</span></span>     | <span data-ttu-id="70ba1-111">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="70ba1-111"></span></span>  <span data-ttu-id="70ba1-112">登录的用户还必须在目录角色中允许这些程序更新。</span><span class="sxs-lookup"><span data-stu-id="70ba1-112">The signed in user must also be in a directory role which permits them to update a program.</span></span> |
|<span data-ttu-id="70ba1-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="70ba1-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="70ba1-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="70ba1-114">Not supported.</span></span> |
|<span data-ttu-id="70ba1-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="70ba1-115">Application</span></span>                            | <span data-ttu-id="70ba1-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="70ba1-116">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="70ba1-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="70ba1-117">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="70ba1-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="70ba1-118">Request headers</span></span>
| <span data-ttu-id="70ba1-119">名称</span><span class="sxs-lookup"><span data-stu-id="70ba1-119">Name</span></span>         | <span data-ttu-id="70ba1-120">类型</span><span class="sxs-lookup"><span data-stu-id="70ba1-120">Type</span></span>        | <span data-ttu-id="70ba1-121">说明</span><span class="sxs-lookup"><span data-stu-id="70ba1-121">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="70ba1-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="70ba1-122">Authorization</span></span> | <span data-ttu-id="70ba1-123">string</span><span class="sxs-lookup"><span data-stu-id="70ba1-123">string</span></span> | <span data-ttu-id="70ba1-124">持有者令牌</span><span class="sxs-lookup"><span data-stu-id="70ba1-124">Bearer \{token\}.</span></span> <span data-ttu-id="70ba1-125">必需。</span><span class="sxs-lookup"><span data-stu-id="70ba1-125">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="70ba1-126">请求正文</span><span class="sxs-lookup"><span data-stu-id="70ba1-126">Request body</span></span>
<span data-ttu-id="70ba1-127">在请求正文中，提供[程序](../resources/program.md)的对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70ba1-127">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="70ba1-128">下表显示程序更新时可以提供的属性。</span><span class="sxs-lookup"><span data-stu-id="70ba1-128">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="70ba1-129">属性</span><span class="sxs-lookup"><span data-stu-id="70ba1-129">Property</span></span>     | <span data-ttu-id="70ba1-130">类型</span><span class="sxs-lookup"><span data-stu-id="70ba1-130">Type</span></span>        | <span data-ttu-id="70ba1-131">说明</span><span class="sxs-lookup"><span data-stu-id="70ba1-131">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="70ba1-132">程序的名称。</span><span class="sxs-lookup"><span data-stu-id="70ba1-132">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="70ba1-133">该程序的描述。</span><span class="sxs-lookup"><span data-stu-id="70ba1-133">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="70ba1-134">响应</span><span class="sxs-lookup"><span data-stu-id="70ba1-134">Response</span></span>
<span data-ttu-id="70ba1-135">如果成功，此方法返回`204, Accepted`响应正文中的响应代码和[程序](../resources/program.md)对象。</span><span class="sxs-lookup"><span data-stu-id="70ba1-135">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70ba1-136">示例</span><span class="sxs-lookup"><span data-stu-id="70ba1-136">Example</span></span>
##### <a name="request"></a><span data-ttu-id="70ba1-137">请求</span><span class="sxs-lookup"><span data-stu-id="70ba1-137">Request</span></span>
<span data-ttu-id="70ba1-138">在请求正文中，提供[程序](../resources/program.md)对象参数，以更改的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="70ba1-138">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>

<!-- {
  "blockType": "request",
  "name": "update_program"
}-->
```http
PATCH https://graph.microsoft.com/beta/programs('7e59d237-2fb0-4e5d-b7bb-d4f9f9129213')
Content-type: application/json

{
    "displayName": "testprogram3 new name"
}
```

##### <a name="response"></a><span data-ttu-id="70ba1-139">响应</span><span class="sxs-lookup"><span data-stu-id="70ba1-139">Response</span></span>
><span data-ttu-id="70ba1-p104">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="70ba1-p104">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 204 Accepted
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3 new name",
    "description": "test description"
}
```

## <a name="see-also"></a><span data-ttu-id="70ba1-142">另请参阅</span><span class="sxs-lookup"><span data-stu-id="70ba1-142">See also</span></span>

| <span data-ttu-id="70ba1-143">方法</span><span class="sxs-lookup"><span data-stu-id="70ba1-143">Method</span></span>           | <span data-ttu-id="70ba1-144">返回类型</span><span class="sxs-lookup"><span data-stu-id="70ba1-144">Return Type</span></span>    |<span data-ttu-id="70ba1-145">说明</span><span class="sxs-lookup"><span data-stu-id="70ba1-145">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="70ba1-146">对程序的列表 programControls</span><span class="sxs-lookup"><span data-stu-id="70ba1-146">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="70ba1-147">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="70ba1-147">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="70ba1-148">获取一个程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="70ba1-148">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="70ba1-149">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="70ba1-149">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="70ba1-150">programControl</span><span class="sxs-lookup"><span data-stu-id="70ba1-150">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="70ba1-151">添加到程序 programControl。</span><span class="sxs-lookup"><span data-stu-id="70ba1-151">Add a programControl to a program.</span></span>|

<!--
{
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/program-update.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
