---
title: 创建程序
description: Azure AD 中访问审阅功能，创建一个新的程序对象。
ms.openlocfilehash: 1ac3fa1f0b555fc92449adf0e57217d0a7d50375
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27047484"
---
# <a name="create-program"></a><span data-ttu-id="1c19e-103">创建程序</span><span class="sxs-lookup"><span data-stu-id="1c19e-103">Create program</span></span>

> <span data-ttu-id="1c19e-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="1c19e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="1c19e-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="1c19e-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="1c19e-106">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中创建新的[程序](../resources/program.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1c19e-106">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [program](../resources/program.md) object.</span></span>
## <a name="permissions"></a><span data-ttu-id="1c19e-107">权限</span><span class="sxs-lookup"><span data-stu-id="1c19e-107">Permissions</span></span>
<span data-ttu-id="1c19e-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="1c19e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="1c19e-110">权限类型</span><span class="sxs-lookup"><span data-stu-id="1c19e-110">Permission type</span></span>                        | <span data-ttu-id="1c19e-111">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="1c19e-111">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="1c19e-112">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="1c19e-112">Delegated (work or school account)</span></span>     | <span data-ttu-id="1c19e-113">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="1c19e-113"></span></span>  <span data-ttu-id="1c19e-114">登录的用户还必须在目录角色中允许他们创建的程序。</span><span class="sxs-lookup"><span data-stu-id="1c19e-114">The signed in user must also be in a directory role which permits them to create a program.</span></span> |
|<span data-ttu-id="1c19e-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="1c19e-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="1c19e-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c19e-116">Not supported.</span></span> |
|<span data-ttu-id="1c19e-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="1c19e-117">Application</span></span>                            | <span data-ttu-id="1c19e-118">不支持。</span><span class="sxs-lookup"><span data-stu-id="1c19e-118">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="1c19e-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="1c19e-119">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programs
```
## <a name="request-headers"></a><span data-ttu-id="1c19e-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="1c19e-120">Request headers</span></span>
| <span data-ttu-id="1c19e-121">名称</span><span class="sxs-lookup"><span data-stu-id="1c19e-121">Name</span></span>         | <span data-ttu-id="1c19e-122">类型</span><span class="sxs-lookup"><span data-stu-id="1c19e-122">Type</span></span>        | <span data-ttu-id="1c19e-123">说明</span><span class="sxs-lookup"><span data-stu-id="1c19e-123">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="1c19e-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="1c19e-124">Authorization</span></span> | <span data-ttu-id="1c19e-125">string</span><span class="sxs-lookup"><span data-stu-id="1c19e-125">string</span></span> | <span data-ttu-id="1c19e-126">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="1c19e-126">Bearer \{token\}.</span></span> <span data-ttu-id="1c19e-127">必需。</span><span class="sxs-lookup"><span data-stu-id="1c19e-127">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="1c19e-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="1c19e-128">Request body</span></span>
<span data-ttu-id="1c19e-129">在请求正文中，提供[程序](../resources/program.md)的对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c19e-129">In the request body, supply a JSON representation of a [program](../resources/program.md) object.</span></span>

<span data-ttu-id="1c19e-130">下表显示时创建程序所需的属性。</span><span class="sxs-lookup"><span data-stu-id="1c19e-130">The following table shows the properties that are required when you create a program.</span></span>

| <span data-ttu-id="1c19e-131">属性</span><span class="sxs-lookup"><span data-stu-id="1c19e-131">Property</span></span>     | <span data-ttu-id="1c19e-132">类型</span><span class="sxs-lookup"><span data-stu-id="1c19e-132">Type</span></span>        | <span data-ttu-id="1c19e-133">说明</span><span class="sxs-lookup"><span data-stu-id="1c19e-133">Description</span></span> |
|:-------------|:------------|:------------|
| `displayName`               |`String`                              |  <span data-ttu-id="1c19e-134">程序的名称。</span><span class="sxs-lookup"><span data-stu-id="1c19e-134">The name of the program.</span></span>                   |
| `description`               |`String`                              |  <span data-ttu-id="1c19e-135">该程序的描述。</span><span class="sxs-lookup"><span data-stu-id="1c19e-135">The description of the program.</span></span>           |


## <a name="response"></a><span data-ttu-id="1c19e-136">响应</span><span class="sxs-lookup"><span data-stu-id="1c19e-136">Response</span></span>
<span data-ttu-id="1c19e-137">如果成功，此方法返回`201, Created`响应正文中的响应代码和[程序](../resources/program.md)对象。</span><span class="sxs-lookup"><span data-stu-id="1c19e-137">If successful, this method returns a `201, Created` response code and [program](../resources/program.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1c19e-138">示例</span><span class="sxs-lookup"><span data-stu-id="1c19e-138">Example</span></span>
##### <a name="request"></a><span data-ttu-id="1c19e-139">请求</span><span class="sxs-lookup"><span data-stu-id="1c19e-139">Request</span></span>
<span data-ttu-id="1c19e-140">在请求正文中，提供[程序](../resources/program.md)的对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="1c19e-140">In the request body, supply a JSON representation of the [program](../resources/program.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_program_from_programs"
}-->
```http
POST https://graph.microsoft.com/beta/programs
Content-type: application/json

{
    "displayName": "testprogram3",
    "description": "test description"
}
```

##### <a name="response"></a><span data-ttu-id="1c19e-141">响应</span><span class="sxs-lookup"><span data-stu-id="1c19e-141">Response</span></span>
><span data-ttu-id="1c19e-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="1c19e-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.program"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
    "id": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "displayName": "testprogram3",
    "description": "test description"
}
```

## <a name="see-also"></a><span data-ttu-id="1c19e-144">另请参阅</span><span class="sxs-lookup"><span data-stu-id="1c19e-144">See also</span></span>

| <span data-ttu-id="1c19e-145">方法</span><span class="sxs-lookup"><span data-stu-id="1c19e-145">Method</span></span>           | <span data-ttu-id="1c19e-146">返回类型</span><span class="sxs-lookup"><span data-stu-id="1c19e-146">Return Type</span></span>    |<span data-ttu-id="1c19e-147">说明</span><span class="sxs-lookup"><span data-stu-id="1c19e-147">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="1c19e-148">列表程序</span><span class="sxs-lookup"><span data-stu-id="1c19e-148">List programs</span></span>](program-list.md) | <span data-ttu-id="1c19e-149">[程序](../resources/program.md)集</span><span class="sxs-lookup"><span data-stu-id="1c19e-149">[program](../resources/program.md) collection</span></span>|  <span data-ttu-id="1c19e-150">获取所有的程序的集合。</span><span class="sxs-lookup"><span data-stu-id="1c19e-150">Get a collection of all the programs.</span></span>|
|[<span data-ttu-id="1c19e-151">对程序的列表 programControls</span><span class="sxs-lookup"><span data-stu-id="1c19e-151">List programControls of a program</span></span>](program-listcontrols.md) |     <span data-ttu-id="1c19e-152">[programControl](../resources/programcontrol.md)集合</span><span class="sxs-lookup"><span data-stu-id="1c19e-152">[programControl](../resources/programcontrol.md) collection</span></span>|    <span data-ttu-id="1c19e-153">获取一个程序的控件的集合。</span><span class="sxs-lookup"><span data-stu-id="1c19e-153">Get a collection of the controls of a program.</span></span>|
|[<span data-ttu-id="1c19e-154">更新程序</span><span class="sxs-lookup"><span data-stu-id="1c19e-154">Update program</span></span>](program-update.md) |  [<span data-ttu-id="1c19e-155">程序</span><span class="sxs-lookup"><span data-stu-id="1c19e-155">program</span></span>](../resources/program.md)| <span data-ttu-id="1c19e-156">更新程序。</span><span class="sxs-lookup"><span data-stu-id="1c19e-156">Update a program.</span></span>|
|[<span data-ttu-id="1c19e-157">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="1c19e-157">Create programControl</span></span>](programcontrol-create.md) |        [<span data-ttu-id="1c19e-158">programControl</span><span class="sxs-lookup"><span data-stu-id="1c19e-158">programControl</span></span>](../resources/programcontrol.md)    |   <span data-ttu-id="1c19e-159">添加到程序 programControl。</span><span class="sxs-lookup"><span data-stu-id="1c19e-159">Add a programControl to a program.</span></span>|

<!-- {
  "type": "#page.annotation",
  "description": "Create program",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
