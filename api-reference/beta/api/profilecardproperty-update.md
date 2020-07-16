---
title: 更新 profileCardProperty
description: 更新 profileCardProperty 对象的属性。
localization_priority: Normal
author: kevinbellinger
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 122b8c0007067dafd2f7326cffc1b4e3b1697890
ms.sourcegitcommit: f3dda172d95ef1eda8f6dd9e3ffdc7d3c0744c0a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 07/14/2020
ms.locfileid: "45123843"
---
# <a name="update-profilecardproperty"></a><span data-ttu-id="b38c9-103">更新 profileCardProperty</span><span class="sxs-lookup"><span data-stu-id="b38c9-103">Update profileCardProperty</span></span>

<span data-ttu-id="b38c9-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="b38c9-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b38c9-105">更新[profileCardProperty](../resources/profilecardproperty.md)对象的属性（由其**directoryPropertyName**属性标识）。</span><span class="sxs-lookup"><span data-stu-id="b38c9-105">Update the properties of a [profileCardProperty](../resources/profilecardproperty.md) object, identified by its **directoryPropertyName** property.</span></span>

## <a name="permissions"></a><span data-ttu-id="b38c9-106">权限</span><span class="sxs-lookup"><span data-stu-id="b38c9-106">Permissions</span></span>

<span data-ttu-id="b38c9-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="b38c9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="b38c9-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="b38c9-109">Permission type</span></span>                        | <span data-ttu-id="b38c9-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="b38c9-110">Permissions (from least to most privileged)</span></span> |
|:---------------------------------------|:--------------------------------------------|
| <span data-ttu-id="b38c9-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="b38c9-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="b38c9-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="b38c9-112">User.ReadWrite, User.ReadWrite.All</span></span>          |
| <span data-ttu-id="b38c9-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="b38c9-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="b38c9-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="b38c9-114">Not supported.</span></span>                              |
| <span data-ttu-id="b38c9-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="b38c9-115">Application</span></span>                            | <span data-ttu-id="b38c9-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="b38c9-116">Not supported.</span></span>                              |

><span data-ttu-id="b38c9-117">**注意：** 若要对此操作使用委派权限，则需要已登录用户拥有租户管理员或全局管理员角色。</span><span class="sxs-lookup"><span data-stu-id="b38c9-117">**Note:** Using delegated permissions for this operation requires the signed-in user to have a tenant administrator or global administrator role.</span></span>

## <a name="http-request"></a><span data-ttu-id="b38c9-118">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="b38c9-118">HTTP request</span></span>

<!-- { "blockType": "ignored" } -->

```http
PATCH https://graph.microsoft.com/beta/organization/{organizationId}/settings/profileCardProperties/{id}
```

## <a name="request-headers"></a><span data-ttu-id="b38c9-119">请求标头</span><span class="sxs-lookup"><span data-stu-id="b38c9-119">Request headers</span></span>

| <span data-ttu-id="b38c9-120">名称</span><span class="sxs-lookup"><span data-stu-id="b38c9-120">Name</span></span>       | <span data-ttu-id="b38c9-121">说明</span><span class="sxs-lookup"><span data-stu-id="b38c9-121">Description</span></span>|
|:-----------|:-----------|
| <span data-ttu-id="b38c9-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="b38c9-122">Authorization</span></span> | <span data-ttu-id="b38c9-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="b38c9-p102">Bearer {token}. Required.</span></span> |
| <span data-ttu-id="b38c9-125">Content-Type</span><span class="sxs-lookup"><span data-stu-id="b38c9-125">Content-Type</span></span>  | <span data-ttu-id="b38c9-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="b38c9-p103">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="b38c9-128">请求正文</span><span class="sxs-lookup"><span data-stu-id="b38c9-128">Request body</span></span>

<span data-ttu-id="b38c9-129">在请求正文中，提供应更新的相关字段的值。</span><span class="sxs-lookup"><span data-stu-id="b38c9-129">In the request body, supply the values for relevant fields that should be updated.</span></span> <span data-ttu-id="b38c9-130">请求正文中不包括的现有属性将保留其以前的值，或根据对其他属性值的更改重新计算。</span><span class="sxs-lookup"><span data-stu-id="b38c9-130">Existing properties that are not included in the request body will maintain their previous values or be recalculated based on changes to other property values.</span></span> <span data-ttu-id="b38c9-131">为了获得最佳性能，请勿加入尚未更改的现有值。</span><span class="sxs-lookup"><span data-stu-id="b38c9-131">For best performance, don't include existing values that haven't changed.</span></span>

| <span data-ttu-id="b38c9-132">属性</span><span class="sxs-lookup"><span data-stu-id="b38c9-132">Property</span></span>     | <span data-ttu-id="b38c9-133">类型</span><span class="sxs-lookup"><span data-stu-id="b38c9-133">Type</span></span>        | <span data-ttu-id="b38c9-134">说明</span><span class="sxs-lookup"><span data-stu-id="b38c9-134">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b38c9-135">批注</span><span class="sxs-lookup"><span data-stu-id="b38c9-135">annotations</span></span>|<span data-ttu-id="b38c9-136">profileCardAnnotation 集合</span><span class="sxs-lookup"><span data-stu-id="b38c9-136">profileCardAnnotation collection</span></span>| <span data-ttu-id="b38c9-137">包含管理员已选择指定的任何可选或本地化标签。</span><span class="sxs-lookup"><span data-stu-id="b38c9-137">Contains any alternative or localized labels an administrator has chosen to specify.</span></span>|
|<span data-ttu-id="b38c9-138">directoryPropertyName</span><span class="sxs-lookup"><span data-stu-id="b38c9-138">directoryPropertyName</span></span>|<span data-ttu-id="b38c9-139">String</span><span class="sxs-lookup"><span data-stu-id="b38c9-139">String</span></span>|<span data-ttu-id="b38c9-140">包含用于在配置文件卡片上呈现的目录属性的名称。</span><span class="sxs-lookup"><span data-stu-id="b38c9-140">Contains the name of the directory property which is intended to surface on the profile card.</span></span> |

## <a name="response"></a><span data-ttu-id="b38c9-141">响应</span><span class="sxs-lookup"><span data-stu-id="b38c9-141">Response</span></span>

<span data-ttu-id="b38c9-142">如果成功，此方法 `200 OK` 在响应正文中返回响应代码和更新的[profileCardProperty](../resources/profilecardproperty.md)对象。</span><span class="sxs-lookup"><span data-stu-id="b38c9-142">If successful, this method returns a `200 OK` response code and an updated [profileCardProperty](../resources/profilecardproperty.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="b38c9-143">示例</span><span class="sxs-lookup"><span data-stu-id="b38c9-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="b38c9-144">请求</span><span class="sxs-lookup"><span data-stu-id="b38c9-144">Request</span></span>

<span data-ttu-id="b38c9-145">下面的示例为区域设置 "无 NB" 添加本地化的标签 "Kostnads Senter"。</span><span class="sxs-lookup"><span data-stu-id="b38c9-145">The following example adds a localized label "Kostnads Senter" for the locale "no-NB".</span></span>

# <a name="http"></a>[<span data-ttu-id="b38c9-146">HTTP</span><span class="sxs-lookup"><span data-stu-id="b38c9-146">HTTP</span></span>](#tab/http)
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
# <a name="javascript"></a>[<span data-ttu-id="b38c9-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="b38c9-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-profilecardproperty-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="b38c9-148">响应</span><span class="sxs-lookup"><span data-stu-id="b38c9-148">Response</span></span>

<span data-ttu-id="b38c9-149">下面展示了示例响应。</span><span class="sxs-lookup"><span data-stu-id="b38c9-149">The following is an example of the response.</span></span>

> <span data-ttu-id="b38c9-p105">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。所有属性都将通过实际调用返回。</span><span class="sxs-lookup"><span data-stu-id="b38c9-p105">**Note:** The response object shown here might be shortened for readability. All the properties will be returned from an actual call.</span></span>

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
