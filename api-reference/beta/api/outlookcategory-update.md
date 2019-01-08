---
title: 更新 Outlook 类别
description: '更新指定 outlookCategory 对象的可写属性 **color**。 不能修改的**displayName**属性 '
ms.openlocfilehash: 741536a659add633da21b27e00006a6782a8beb7
ms.sourcegitcommit: 37591c2299c80e7675cd2b5f781e1eeeba628a60
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/08/2019
ms.locfileid: "27748533"
---
# <a name="update-outlook-category"></a><span data-ttu-id="0d591-104">更新 Outlook 类别</span><span class="sxs-lookup"><span data-stu-id="0d591-104">Update Outlook category</span></span>

> <span data-ttu-id="0d591-105">**重要说明**： 在 Microsoft Graph 中的 /beta 版本下的 Api 在预览，并会受到更改。</span><span class="sxs-lookup"><span data-stu-id="0d591-105">**Important**: APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="0d591-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="0d591-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="0d591-107">更新指定 [outlookCategory](../resources/outlookcategory.md) 对象的可写属性 **color**。</span><span class="sxs-lookup"><span data-stu-id="0d591-107">Update the writable property, **color**, of the specified [outlookCategory](../resources/outlookcategory.md) object.</span></span> <span data-ttu-id="0d591-108">创建类别后，不能修改 **displayName** 属性。</span><span class="sxs-lookup"><span data-stu-id="0d591-108">You cannot modify the **displayName** property once you have created the category.</span></span>

## <a name="permissions"></a><span data-ttu-id="0d591-109">权限</span><span class="sxs-lookup"><span data-stu-id="0d591-109">Permissions</span></span>
<span data-ttu-id="0d591-p104">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="0d591-p104">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="0d591-112">权限类型</span><span class="sxs-lookup"><span data-stu-id="0d591-112">Permission type</span></span>      | <span data-ttu-id="0d591-113">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="0d591-113">Permissions (from least to most privileged)</span></span>              |
|:--------------------|:---------------------------------------------------------|
|<span data-ttu-id="0d591-114">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="0d591-114">Delegated (work or school account)</span></span> | <span data-ttu-id="0d591-115">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d591-115">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="0d591-116">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="0d591-116">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="0d591-117">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d591-117">MailboxSettings.ReadWrite</span></span>    |
|<span data-ttu-id="0d591-118">应用程序</span><span class="sxs-lookup"><span data-stu-id="0d591-118">Application</span></span> | <span data-ttu-id="0d591-119">MailboxSettings.ReadWrite</span><span class="sxs-lookup"><span data-stu-id="0d591-119">MailboxSettings.ReadWrite</span></span> |

## <a name="http-request"></a><span data-ttu-id="0d591-120">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="0d591-120">HTTP request</span></span>
<!-- { "blockType": "ignored" } -->
```http
PATCH /me/outlook/masterCategories/{id}
PATCH /users/{id|userPrincipalName}/outlook/masterCategories/{id}
```

## <a name="request-headers"></a><span data-ttu-id="0d591-121">请求标头</span><span class="sxs-lookup"><span data-stu-id="0d591-121">Request headers</span></span>
| <span data-ttu-id="0d591-122">名称</span><span class="sxs-lookup"><span data-stu-id="0d591-122">Name</span></span>      |<span data-ttu-id="0d591-123">说明</span><span class="sxs-lookup"><span data-stu-id="0d591-123">Description</span></span>|
|:----------|:----------|
| <span data-ttu-id="0d591-124">Authorization</span><span class="sxs-lookup"><span data-stu-id="0d591-124">Authorization</span></span>  | <span data-ttu-id="0d591-p105">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="0d591-p105">Bearer {token}. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="0d591-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="0d591-127">Request body</span></span>
<span data-ttu-id="0d591-p106">在请求正文中，提供应更新的相关字段的值。请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。为了获得最佳性能，不应包括尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="0d591-p106">In the request body, supply the values for relevant fields that should be updated. Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values. For best performance you shouldn't include existing values that haven't changed.</span></span>

| <span data-ttu-id="0d591-131">属性</span><span class="sxs-lookup"><span data-stu-id="0d591-131">Property</span></span>     | <span data-ttu-id="0d591-132">类型</span><span class="sxs-lookup"><span data-stu-id="0d591-132">Type</span></span>   |<span data-ttu-id="0d591-133">说明</span><span class="sxs-lookup"><span data-stu-id="0d591-133">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="0d591-134">color</span><span class="sxs-lookup"><span data-stu-id="0d591-134">color</span></span>|<span data-ttu-id="0d591-135">String</span><span class="sxs-lookup"><span data-stu-id="0d591-135">String</span></span>|<span data-ttu-id="0d591-136">预先设定的颜色常数，它表示类别的特征，并映射到 25 种预定义颜色中的一种。</span><span class="sxs-lookup"><span data-stu-id="0d591-136">A pre-set color constant that characterizes a category, and that is mapped to one of 25 predefined colors.</span></span> |

## <a name="response"></a><span data-ttu-id="0d591-137">响应</span><span class="sxs-lookup"><span data-stu-id="0d591-137">Response</span></span>

<span data-ttu-id="0d591-138">如果成功，此方法在响应正文中返回 `200 OK` 响应代码和更新的 [outlookCategory](../resources/outlookcategory.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="0d591-138">If successful, this method returns a `200 OK` response code and updated [outlookCategory](../resources/outlookcategory.md) object in the response body.</span></span>
## <a name="example"></a><span data-ttu-id="0d591-139">示例</span><span class="sxs-lookup"><span data-stu-id="0d591-139">Example</span></span>
##### <a name="request"></a><span data-ttu-id="0d591-140">请求</span><span class="sxs-lookup"><span data-stu-id="0d591-140">Request</span></span>
<span data-ttu-id="0d591-141">下面是一个请求示例。</span><span class="sxs-lookup"><span data-stu-id="0d591-141">Here is an example of the request.</span></span>
<!-- {
  "blockType": "request",
  "name": "update_outlookcategory"
}-->
```http
PATCH https://graph.microsoft.com/beta/me/outlook/masterCategories('bac262b7-485d-4739-b436-e31467d64fac')
Content-type: application/json
Content-length: 30

{
  "color":"preset15"
}
```
##### <a name="response"></a><span data-ttu-id="0d591-142">响应</span><span class="sxs-lookup"><span data-stu-id="0d591-142">Response</span></span>
<span data-ttu-id="0d591-p107">下面是一个响应示例。注意：为了简单起见，可能会将此处所示的响应对象截断。将从实际调用中返回所有属性。</span><span class="sxs-lookup"><span data-stu-id="0d591-p107">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.outlookCategory"
} -->
```http
HTTP/1.1 200 OK
Content-type: application/json
Content-length: 251

{
  "@odata.context":"https://graph.microsoft.com/beta/$metadata#users('8ae6f565-0d7f-4ead-853e-7db94c912a1f')/outlook/masterCategories/$entity",
  "id":"bac262b7-485d-4739-b436-e31467d64fac",
  "displayName":"Project expenses",
  "color":"preset15"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update outlookCategory",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->