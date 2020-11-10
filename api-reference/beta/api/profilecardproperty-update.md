---
title: Update profileCardProperty
description: 更新 profileCardProperty 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 7e7acede752607b34cf8f3cb9378cb0d87983f25
ms.sourcegitcommit: 342516a52b69fcda31442b130eb6bd7e2c8a0066
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/10/2020
ms.locfileid: "48968979"
---
# <a name="update-profilecardproperty"></a><span data-ttu-id="5916c-103">Update profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="5916c-103">Update profileCardProperty</span></span>

<span data-ttu-id="5916c-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="5916c-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="5916c-105">更新 [profileCardProperty](../resources/profilecardproperty.md) 对象的属性（由其 **directoryPropertyName** 属性标识）。</span><span class="sxs-lookup"><span data-stu-id="5916c-105">Update the properties of a [profileCardProperty](../resources/profilecardproperty.md) object, identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="5916c-106">权限</span><span class="sxs-lookup"><span data-stu-id="5916c-106">Permissions</span></span>

<span data-ttu-id="5916c-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="5916c-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="5916c-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="5916c-109">Permission type</span></span>                        | <span data-ttu-id="5916c-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="5916c-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="5916c-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="5916c-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="5916c-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="5916c-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="5916c-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="5916c-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="5916c-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="5916c-114">Not supported.</span></span>                              |
| <span data-ttu-id="5916c-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="5916c-115">Application</span></span>                            | <span data-ttu-id="5916c-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="5916c-116">Not supported.</span></span>                              |

><span data-ttu-id="5916c-117">**注意：** 若要对此操作使用委派权限，则需要已登录用户拥有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="5916c-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="5916c-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="5916c-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="5916c-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="5916c-119">Request headers</span></span>

| <span data-ttu-id="5916c-120">名称</span><span class="sxs-lookup"><span data-stu-id="5916c-120">Name</span></span>       | <span data-ttu-id="5916c-121">说明</span><span class="sxs-lookup"><span data-stu-id="5916c-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="5916c-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="5916c-122">Authorization</span></span> | <span data-ttu-id="5916c-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="5916c-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="5916c-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="5916c-125">Content-Type</span></span>  | <span data-ttu-id="5916c-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="5916c-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="5916c-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="5916c-128">Request body</span></span>

<span data-ttu-id="5916c-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="5916c-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="5916c-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="5916c-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="5916c-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="5916c-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="5916c-132">属性</span><span class="sxs-lookup"><span data-stu-id="5916c-132">Property</span></span>     | <span data-ttu-id="5916c-133">类型</span><span class="sxs-lookup"><span data-stu-id="5916c-133">Type</span></span>        | <span data-ttu-id="5916c-134">说明</span><span class="sxs-lookup"><span data-stu-id="5916c-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="5916c-135">批注</span><span class="sxs-lookup"><span data-stu-id="5916c-135">annotations</span></span>|<span data-ttu-id="5916c-136">profileCardAnnotation 集合</span><span class="sxs-lookup"><span data-stu-id="5916c-136">profileCardAnnotation collection</span></span>| <span data-ttu-id="5916c-137">包含管理员已选择指定的任何可选或本地化标签。</span><span class="sxs-lookup"><span data-stu-id="5916c-137">Contains any alternative or localized labels an administrator has chosen to specify.</span></span>|
|<span data-ttu-id="5916c-138">directoryPropertyName</span><span class="sxs-lookup"><span data-stu-id="5916c-138">directoryPropertyName</span></span>|<span data-ttu-id="5916c-139">String</span><span class="sxs-lookup"><span data-stu-id="5916c-139">String</span></span>|<span data-ttu-id="5916c-140">包含用于在配置文件卡片上呈现的目录属性的名称。</span><span class="sxs-lookup"><span data-stu-id="5916c-140">Contains the name of the directory property which is intended to surface on the profile card.</span></span> |

## <a name="response"></a><span data-ttu-id="5916c-141">响应</span><span class="sxs-lookup"><span data-stu-id="5916c-141">Response</span></span>

<span data-ttu-id="5916c-142">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的 [profileCardProperty](../resources/profilecardproperty.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="5916c-142">If successful, this method returns a `200 OK` response code and an updated [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="5916c-143">示例</span><span class="sxs-lookup"><span data-stu-id="5916c-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="5916c-144">请求</span><span class="sxs-lookup"><span data-stu-id="5916c-144">Request</span></span>

<span data-ttu-id="5916c-145">下面的示例为区域设置 "无 NB" 添加本地化的标签 "Kostnads Senter"。</span><span class="sxs-lookup"><span data-stu-id="5916c-145">The following example adds a localized label "Kostnads Senter" for the locale "no-NB".</span></span>

# <a name="http"></a>[<span data-ttu-id="5916c-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="5916c-146">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_profilecardproperty"
}-->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/CustomAttribute1
Content-type: application/json

{
  "annotations": [
    {
      "localizations": [
        {
          "languageTag": "no-NB",
          "displayName": "Kostnads Senter"
        }
      ]
    }
  ]
}
```
# <a name="javascript"></a>[<span data-ttu-id="5916c-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="5916c-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilecardproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="c"></a>[<span data-ttu-id="5916c-148">C#</span><span class="sxs-lookup"><span data-stu-id="5916c-148">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-profilecardproperty-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="5916c-149">Objective-C</span><span class="sxs-lookup"><span data-stu-id="5916c-149">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-profilecardproperty-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="5916c-150">Java</span><span class="sxs-lookup"><span data-stu-id="5916c-150">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-profilecardproperty-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="5916c-151">响应</span><span class="sxs-lookup"><span data-stu-id="5916c-151">Response</span></span>

<span data-ttu-id="5916c-152">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="5916c-152">The following is an example of the response.</span></span>

> <span data-ttu-id="5916c-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="5916c-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.profileCardProperty"
} -->

```http
HTTP/1.1 200 OK
Content-type: application/json

{
  "directoryPropertyName": "CustomAttribute1",
  "annotations": [
    {
      "displayName": "Cost Center",
      "localizations": [
        {
          "languageTag": "ru-RU",
          "displayName": "центр затрат"
        },
        {
          "languageTag": "no-NB",
          "displayName": "Kostnads Senter"
        }
      ]
    }
  ]
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "Update profilecardproperty",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->


