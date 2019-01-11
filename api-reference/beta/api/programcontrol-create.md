---
title: 创建 programControl
description: Azure AD 中访问审阅功能，创建一个新的 programControl 对象。  这会链接到程序访问审阅。
localization_priority: Normal
ms.openlocfilehash: 4dfbb76244a41867b8a57faa42f63dc728f59136
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27851532"
---
# <a name="create-programcontrol"></a><span data-ttu-id="20006-104">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="20006-104">Create programControl</span></span>

> <span data-ttu-id="20006-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="20006-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="20006-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="20006-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="20006-107">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中创建新的[programControl](../resources/programcontrol.md)对象。</span><span class="sxs-lookup"><span data-stu-id="20006-107">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="20006-108">这会链接到程序访问审阅。</span><span class="sxs-lookup"><span data-stu-id="20006-108">This links an access review to a program.</span></span>

<span data-ttu-id="20006-109">进行此请求之前, 将呼叫者必须具有之前</span><span class="sxs-lookup"><span data-stu-id="20006-109">Prior to making this request, the caller must have previously</span></span>

 - <span data-ttu-id="20006-110">[创建一个程序](program-create.md)或[检索程序](program-list.md)，以使数值`programId`要包含在请求中，</span><span class="sxs-lookup"><span data-stu-id="20006-110">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
 - <span data-ttu-id="20006-111">[创建访问审阅](accessreview-create.md)或[检索访问审阅](accessreview-get.md)，具有的值`controlId`要包含在请求中，和</span><span class="sxs-lookup"><span data-stu-id="20006-111">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
 - <span data-ttu-id="20006-112">[检索的程序控件类型的列表](programcontroltype-list.md)，以使数值`controlTypeId`要包含在请求中。</span><span class="sxs-lookup"><span data-stu-id="20006-112">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="20006-113">权限</span><span class="sxs-lookup"><span data-stu-id="20006-113">Permissions</span></span>
<span data-ttu-id="20006-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="20006-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="20006-116">权限类型</span><span class="sxs-lookup"><span data-stu-id="20006-116">Permission type</span></span>                        | <span data-ttu-id="20006-117">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="20006-117">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="20006-118">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="20006-118">Delegated (work or school account)</span></span>     | <span data-ttu-id="20006-119">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="20006-119"></span></span>  <span data-ttu-id="20006-120">登录的用户必须同时是允许他们创建 programControl 目录角色中。</span><span class="sxs-lookup"><span data-stu-id="20006-120">The signed in user must also be in a directory role which permits them to create a programControl.</span></span> |
|<span data-ttu-id="20006-121">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="20006-121">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="20006-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="20006-122">Not supported.</span></span> |
|<span data-ttu-id="20006-123">应用程序</span><span class="sxs-lookup"><span data-stu-id="20006-123">Application</span></span>                            | <span data-ttu-id="20006-124">不支持。</span><span class="sxs-lookup"><span data-stu-id="20006-124">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="20006-125">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="20006-125">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="20006-126">请求标头</span><span class="sxs-lookup"><span data-stu-id="20006-126">Request headers</span></span>
| <span data-ttu-id="20006-127">名称</span><span class="sxs-lookup"><span data-stu-id="20006-127">Name</span></span>         | <span data-ttu-id="20006-128">类型</span><span class="sxs-lookup"><span data-stu-id="20006-128">Type</span></span>        | <span data-ttu-id="20006-129">说明</span><span class="sxs-lookup"><span data-stu-id="20006-129">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="20006-130">Authorization</span><span class="sxs-lookup"><span data-stu-id="20006-130">Authorization</span></span> | <span data-ttu-id="20006-131">string</span><span class="sxs-lookup"><span data-stu-id="20006-131">string</span></span> | <span data-ttu-id="20006-132">持有者\{标记\}。</span><span class="sxs-lookup"><span data-stu-id="20006-132">Bearer \{token\}.</span></span> <span data-ttu-id="20006-133">必填。</span><span class="sxs-lookup"><span data-stu-id="20006-133">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="20006-134">请求正文</span><span class="sxs-lookup"><span data-stu-id="20006-134">Request body</span></span>
<span data-ttu-id="20006-135">在请求正文中，提供[programControl](../resources/programcontrol.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20006-135">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="20006-136">下表显示时创建一个程序控件所需的属性。</span><span class="sxs-lookup"><span data-stu-id="20006-136">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="20006-137">属性</span><span class="sxs-lookup"><span data-stu-id="20006-137">Property</span></span>     | <span data-ttu-id="20006-138">类型</span><span class="sxs-lookup"><span data-stu-id="20006-138">Type</span></span>        | <span data-ttu-id="20006-139">Description</span><span class="sxs-lookup"><span data-stu-id="20006-139">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="20006-140">程序 programId 此控件将变得的一部分。</span><span class="sxs-lookup"><span data-stu-id="20006-140">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="20006-141">控件的 controlId，尤其要指出的访问的标识符查看。</span><span class="sxs-lookup"><span data-stu-id="20006-141">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="20006-142">ProgramControlType 标识的程序控件的类型-例如，将链接到来宾访问控制审阅。</span><span class="sxs-lookup"><span data-stu-id="20006-142">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="20006-143">响应</span><span class="sxs-lookup"><span data-stu-id="20006-143">Response</span></span>
<span data-ttu-id="20006-144">如果成功，此方法返回`201, Created`响应代码和响应正文中的[programControl](../resources/programcontrol.md)对象。</span><span class="sxs-lookup"><span data-stu-id="20006-144">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="20006-145">示例</span><span class="sxs-lookup"><span data-stu-id="20006-145">Example</span></span>
##### <a name="request"></a><span data-ttu-id="20006-146">请求</span><span class="sxs-lookup"><span data-stu-id="20006-146">Request</span></span>
<span data-ttu-id="20006-147">在请求正文中，提供[programControl](../resources/programcontrol.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="20006-147">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>

<!-- {
  "blockType": "request",
  "name": "create_programControl_from_programControls"
}-->
```http
POST https://graph.microsoft.com/beta/programControls
Content-type: application/json

{
    "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
    "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
    "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213"
}
```

##### <a name="response"></a><span data-ttu-id="20006-148">响应</span><span class="sxs-lookup"><span data-stu-id="20006-148">Response</span></span>
><span data-ttu-id="20006-p107">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="20006-p107">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.programControl"
} -->
```http
HTTP/1.1 201 Created
Content-type: application/json

{
  "id": "63b2302c-7e62-43b7-aefb-063ba5bdb853",
  "controlId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "programId": "7e59d237-2fb0-4e5d-b7bb-d4f9f9129213",
  "controlTypeId": "6e4f3d20-c5c3-407f-9695-8460952bcc68",
  "displayName": "test",
  "status": "Active",
  "createdDateTime": "2018-05-18T20:26:05.2976279Z"
}
```

## <a name="see-also"></a><span data-ttu-id="20006-151">另请参阅</span><span class="sxs-lookup"><span data-stu-id="20006-151">See also</span></span>

| <span data-ttu-id="20006-152">方法</span><span class="sxs-lookup"><span data-stu-id="20006-152">Method</span></span>           | <span data-ttu-id="20006-153">返回类型</span><span class="sxs-lookup"><span data-stu-id="20006-153">Return Type</span></span>    |<span data-ttu-id="20006-154">说明</span><span class="sxs-lookup"><span data-stu-id="20006-154">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="20006-155">列表 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="20006-155">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="20006-156">[programControlType](../resources/programcontroltype.md)集合</span><span class="sxs-lookup"><span data-stu-id="20006-156">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="20006-157">列出程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="20006-157">List program control types.</span></span> |


<!-- {
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
