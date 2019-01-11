---
title: 更新程序
description: 在 Azure AD 中访问审阅功能，则请更新现有程序对象。
localization_priority: Normal
ms.openlocfilehash: a9abe10a2a672984d14f1da821b7ae6244cbdf39
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27840332"
---
# <a name="update-program"></a><span data-ttu-id="469f5-103">更新程序</span><span class="sxs-lookup"><span data-stu-id="469f5-103">Update program</span></span>

> <span data-ttu-id="469f5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="469f5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="469f5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="469f5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="469f5-106">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中，更新现有[程序](../resources/program.md)对象。</span><span class="sxs-lookup"><span data-stu-id="469f5-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, update an existing [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="469f5-107">权限</span><span class="sxs-lookup"><span data-stu-id="469f5-107">Permissions</span></span>
<span data-ttu-id="469f5-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="469f5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="469f5-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="469f5-110">Permission type</span></span>                        | <span data-ttu-id="469f5-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="469f5-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="469f5-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="469f5-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="469f5-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="469f5-113"></span></span>  <span data-ttu-id="469f5-114">登录的用户还必须在目录角色中允许这些程序更新。</span><span class="sxs-lookup"><span data-stu-id="469f5-114">The signed in user must also be in a directory role which permits them to update a program.</span></span> |
|<span data-ttu-id="469f5-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="469f5-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="469f5-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="469f5-116">Not supported.</span></span> |
|<span data-ttu-id="469f5-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="469f5-117">Application</span></span>                            | <span data-ttu-id="469f5-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="469f5-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="469f5-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="469f5-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /programs('{programId}')
```
## <a name="request-headers"></a><span data-ttu-id="469f5-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="469f5-120">Request headers</span></span>
| <span data-ttu-id="469f5-121">名称</span><span class="sxs-lookup"><span data-stu-id="469f5-121">Name</span></span>         | <span data-ttu-id="469f5-122">类型</span><span class="sxs-lookup"><span data-stu-id="469f5-122">Type</span></span>        | <span data-ttu-id="469f5-123">说明</span><span class="sxs-lookup"><span data-stu-id="469f5-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="469f5-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="469f5-124">Authorization</span></span> | <span data-ttu-id="469f5-125">string</span><span class="sxs-lookup"><span data-stu-id="469f5-125">string</span></span> | <span data-ttu-id="469f5-126">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="469f5-126">Bearer \{token\}.</span></span> <span data-ttu-id="469f5-127">必填。</span><span class="sxs-lookup"><span data-stu-id="469f5-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="469f5-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="469f5-128">Request body</span></span>
<span data-ttu-id="469f5-129">在请求正文中，提供[程序](../resources/program.md)的对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="469f5-129">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="469f5-130">下表显示程序更新时可以提供的属性。</span><span class="sxs-lookup"><span data-stu-id="469f5-130">The following table shows the properties that can be supplied when you update a program.</span></span>

| <span data-ttu-id="469f5-131">属性</span><span class="sxs-lookup"><span data-stu-id="469f5-131">Property</span></span>     | <span data-ttu-id="469f5-132">类型</span><span class="sxs-lookup"><span data-stu-id="469f5-132">Type</span></span>        | <span data-ttu-id="469f5-133">Description</span><span class="sxs-lookup"><span data-stu-id="469f5-133">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="469f5-134">程序的名称。</span><span class="sxs-lookup"><span data-stu-id="469f5-134">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="469f5-135">该程序的描述。</span><span class="sxs-lookup"><span data-stu-id="469f5-135">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="469f5-136">响应</span><span class="sxs-lookup"><span data-stu-id="469f5-136">Response</span></span>
<span data-ttu-id="469f5-137">如果成功，此方法返回`204, Accepted`响应正文中的响应代码和[程序](../resources/program.md)对象。</span><span class="sxs-lookup"><span data-stu-id="469f5-137">If successful, this method returns a `204, Accepted` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="469f5-138">示例</span><span class="sxs-lookup"><span data-stu-id="469f5-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="469f5-139">请求</span><span class="sxs-lookup"><span data-stu-id="469f5-139">Request</span></span>
<span data-ttu-id="469f5-140">在请求正文中，提供[程序](../resources/program.md)对象参数，以更改的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="469f5-140">In the request body, supply a JSON representation of the [program](../resources/program.md) object parameters to change.</span></span>

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

##### <a name="response"></a><span data-ttu-id="469f5-141">响应</span><span class="sxs-lookup"><span data-stu-id="469f5-141">Response</span></span>
><span data-ttu-id="469f5-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="469f5-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="469f5-144">另请参阅</span><span class="sxs-lookup"><span data-stu-id="469f5-144">See also</span></span>

| <span data-ttu-id="469f5-145">方法</span><span class="sxs-lookup"><span data-stu-id="469f5-145">Method</span></span>           | <span data-ttu-id="469f5-146">返回类型</span><span class="sxs-lookup"><span data-stu-id="469f5-146">Return Type</span></span>    |<span data-ttu-id="469f5-147">说明</span><span class="sxs-lookup"><span data-stu-id="469f5-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="469f5-148">对程序的列表 programControls</span><span class="sxs-lookup"><span data-stu-id="469f5-148">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="469f5-149">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="469f5-149">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="469f5-150">获取一个程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="469f5-150">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="469f5-151">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="469f5-151">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="469f5-152">programControl</span><span class="sxs-lookup"><span data-stu-id="469f5-152">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="469f5-153">添加到程序 programControl。</span><span class="sxs-lookup"><span data-stu-id="469f5-153">Add a programControl to a program.</span></span>|

<!-- {
  "type": "#page.annotation",
  "description": "Update program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
