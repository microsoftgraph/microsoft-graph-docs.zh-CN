---
title: 创建 programControl
description: Azure AD 中访问审阅功能，创建一个新的 programControl 对象。  这会链接到程序访问审阅。
localization_priority: Normal
ms.openlocfilehash: 89e31994ea91dba68e2f4563c64eeab53dd4db93
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29511112"
---
# <a name="create-programcontrol"></a><span data-ttu-id="7cc49-104">创建 programControl</span><span class="sxs-lookup"><span data-stu-id="7cc49-104">Create programControl</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7cc49-105">在 Azure AD[访问审阅](../resources/accessreviews-root.md)功能中创建新的[programControl](../resources/programcontrol.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7cc49-105">In the Azure AD [access reviews](../resources/accessreviews-root.md) feature, create a new [programControl](../resources/programcontrol.md) object.</span></span>  <span data-ttu-id="7cc49-106">这会链接到程序访问审阅。</span><span class="sxs-lookup"><span data-stu-id="7cc49-106">This links an access review to a program.</span></span>

<span data-ttu-id="7cc49-107">进行此请求之前, 将呼叫者必须具有之前</span><span class="sxs-lookup"><span data-stu-id="7cc49-107">Prior to making this request, the caller must have previously</span></span>

 - <span data-ttu-id="7cc49-108">[创建一个程序](program-create.md)或[检索程序](program-list.md)，以使数值`programId`要包含在请求中，</span><span class="sxs-lookup"><span data-stu-id="7cc49-108">[created a program](program-create.md) or [retrieved a program](program-list.md), to have the value of `programId` to include in the request,</span></span>
 - <span data-ttu-id="7cc49-109">[创建访问审阅](accessreview-create.md)或[检索访问审阅](accessreview-get.md)，具有的值`controlId`要包含在请求中，和</span><span class="sxs-lookup"><span data-stu-id="7cc49-109">[created an access review](accessreview-create.md) or [retrieved an access review](accessreview-get.md), to have the value of `controlId` to include in the request, and</span></span>
 - <span data-ttu-id="7cc49-110">[检索的程序控件类型的列表](programcontroltype-list.md)，以使数值`controlTypeId`要包含在请求中。</span><span class="sxs-lookup"><span data-stu-id="7cc49-110">[retrieved the list of program control types](programcontroltype-list.md), to have the value of `controlTypeId` to include in the request.</span></span>


## <a name="permissions"></a><span data-ttu-id="7cc49-111">权限</span><span class="sxs-lookup"><span data-stu-id="7cc49-111">Permissions</span></span>
<span data-ttu-id="7cc49-p103">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="7cc49-p103">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7cc49-114">权限类型</span><span class="sxs-lookup"><span data-stu-id="7cc49-114">Permission type</span></span>                        | <span data-ttu-id="7cc49-115">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="7cc49-115">Permissions (from least to most privileged)</span></span>              |
|:--------------------------------------|:---------------------------------------------------------|
|<span data-ttu-id="7cc49-116">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="7cc49-116">Delegated (work or school account)</span></span>     | <span data-ttu-id="7cc49-117">`ProgramControl.ReadWrite.All`.</span><span class="sxs-lookup"><span data-stu-id="7cc49-117"></span></span>  <span data-ttu-id="7cc49-118">登录的用户必须同时是允许他们创建 programControl 目录角色中。</span><span class="sxs-lookup"><span data-stu-id="7cc49-118">The signed in user must also be in a directory role which permits them to create a programControl.</span></span> |
|<span data-ttu-id="7cc49-119">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="7cc49-119">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="7cc49-120">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cc49-120">Not supported.</span></span> |
|<span data-ttu-id="7cc49-121">应用程序</span><span class="sxs-lookup"><span data-stu-id="7cc49-121">Application</span></span>                            | <span data-ttu-id="7cc49-122">不支持。</span><span class="sxs-lookup"><span data-stu-id="7cc49-122">Not supported.</span></span> |

## <a name="http-request"></a><span data-ttu-id="7cc49-123">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="7cc49-123">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
POST /programControls
```
## <a name="request-headers"></a><span data-ttu-id="7cc49-124">请求标头</span><span class="sxs-lookup"><span data-stu-id="7cc49-124">Request headers</span></span>
| <span data-ttu-id="7cc49-125">名称</span><span class="sxs-lookup"><span data-stu-id="7cc49-125">Name</span></span>         | <span data-ttu-id="7cc49-126">类型</span><span class="sxs-lookup"><span data-stu-id="7cc49-126">Type</span></span>        | <span data-ttu-id="7cc49-127">说明</span><span class="sxs-lookup"><span data-stu-id="7cc49-127">Description</span></span> |
|:-------------|:------------|:------------|
| <span data-ttu-id="7cc49-128">Authorization</span><span class="sxs-lookup"><span data-stu-id="7cc49-128">Authorization</span></span> | <span data-ttu-id="7cc49-129">string</span><span class="sxs-lookup"><span data-stu-id="7cc49-129">string</span></span> | <span data-ttu-id="7cc49-130">持有者令牌</span><span class="sxs-lookup"><span data-stu-id="7cc49-130">Bearer \{token\}.</span></span> <span data-ttu-id="7cc49-131">必需。</span><span class="sxs-lookup"><span data-stu-id="7cc49-131">Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="7cc49-132">请求正文</span><span class="sxs-lookup"><span data-stu-id="7cc49-132">Request body</span></span>
<span data-ttu-id="7cc49-133">在请求正文中，提供[programControl](../resources/programcontrol.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7cc49-133">In the request body, supply a JSON representation of a [programControl](../resources/programcontrol.md) object.</span></span>

<span data-ttu-id="7cc49-134">下表显示时创建一个程序控件所需的属性。</span><span class="sxs-lookup"><span data-stu-id="7cc49-134">The following table shows the properties that are required when you create a program control.</span></span>

| <span data-ttu-id="7cc49-135">属性</span><span class="sxs-lookup"><span data-stu-id="7cc49-135">Property</span></span>     | <span data-ttu-id="7cc49-136">类型</span><span class="sxs-lookup"><span data-stu-id="7cc49-136">Type</span></span>        | <span data-ttu-id="7cc49-137">说明</span><span class="sxs-lookup"><span data-stu-id="7cc49-137">Description</span></span> |
|:-------------|:------------|:------------|
| `programId`              |`String`                | <span data-ttu-id="7cc49-138">程序 programId 此控件将变得的一部分。</span><span class="sxs-lookup"><span data-stu-id="7cc49-138">The programId of the program this control is going to become a part of.</span></span>                             |
| `controlId`              |`String`                | <span data-ttu-id="7cc49-139">控件的 controlId，尤其要指出的访问的标识符查看。</span><span class="sxs-lookup"><span data-stu-id="7cc49-139">The controlId of the control, in particular the identifier of an access review.</span></span>                                                |
| `controlTypeId`          |`String`                | <span data-ttu-id="7cc49-140">ProgramControlType 标识的程序控件的类型-例如，将链接到来宾访问控制审阅。</span><span class="sxs-lookup"><span data-stu-id="7cc49-140">The programControlType identifies the type of program control - for example, a control linking to guest access reviews.</span></span> |

## <a name="response"></a><span data-ttu-id="7cc49-141">响应</span><span class="sxs-lookup"><span data-stu-id="7cc49-141">Response</span></span>
<span data-ttu-id="7cc49-142">如果成功，此方法返回`201, Created`响应代码和响应正文中的[programControl](../resources/programcontrol.md)对象。</span><span class="sxs-lookup"><span data-stu-id="7cc49-142">If successful, this method returns a `201, Created` response code and a [programControl](../resources/programcontrol.md) object in the response body.</span></span>


## <a name="example"></a><span data-ttu-id="7cc49-143">示例</span><span class="sxs-lookup"><span data-stu-id="7cc49-143">Example</span></span>
##### <a name="request"></a><span data-ttu-id="7cc49-144">请求</span><span class="sxs-lookup"><span data-stu-id="7cc49-144">Request</span></span>
<span data-ttu-id="7cc49-145">在请求正文中，提供[programControl](../resources/programcontrol.md)对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7cc49-145">In the request body, supply a JSON representation of the [programControl](../resources/programcontrol.md) object.</span></span>

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

##### <a name="response"></a><span data-ttu-id="7cc49-146">响应</span><span class="sxs-lookup"><span data-stu-id="7cc49-146">Response</span></span>
><span data-ttu-id="7cc49-p106">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="7cc49-p106">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>
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

## <a name="see-also"></a><span data-ttu-id="7cc49-149">另请参阅</span><span class="sxs-lookup"><span data-stu-id="7cc49-149">See also</span></span>

| <span data-ttu-id="7cc49-150">方法</span><span class="sxs-lookup"><span data-stu-id="7cc49-150">Method</span></span>           | <span data-ttu-id="7cc49-151">返回类型</span><span class="sxs-lookup"><span data-stu-id="7cc49-151">Return Type</span></span>    |<span data-ttu-id="7cc49-152">说明</span><span class="sxs-lookup"><span data-stu-id="7cc49-152">Description</span></span>|
|:---------------|:--------|:----------|
|[<span data-ttu-id="7cc49-153">列表 programControlTypes</span><span class="sxs-lookup"><span data-stu-id="7cc49-153">List programControlTypes</span></span>](../api/programcontroltype-list.md) | <span data-ttu-id="7cc49-154">[programControlType](../resources/programcontroltype.md)集合</span><span class="sxs-lookup"><span data-stu-id="7cc49-154">[programControlType](../resources/programcontroltype.md) collection</span></span>| <span data-ttu-id="7cc49-155">列出程序控件类型。</span><span class="sxs-lookup"><span data-stu-id="7cc49-155">List program control types.</span></span> |


<!--
{
  "type": "#page.annotation",
  "description": "Create programControl",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/api/programcontrol-create.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
