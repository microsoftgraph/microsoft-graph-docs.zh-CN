---
title: 创建备注
description: 创建新的 notes 对象。
author: kevinbellinger
localization_priority: Normal
ms.prod: people
doc_type: apiPageType
ms.openlocfilehash: 139de864b9ddec90336e56e122da5f6bf6922952
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48034385"
---
# <a name="create-personannotation"></a><span data-ttu-id="183eb-103">创建 personAnnotation</span><span class="sxs-lookup"><span data-stu-id="183eb-103">Create personAnnotation</span></span>
<span data-ttu-id="183eb-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="183eb-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="183eb-105">在用户的[配置文件](../resources/profile.md)中创建新的[personAnnotation](../resources/personannotation.md)对象。</span><span class="sxs-lookup"><span data-stu-id="183eb-105">Create a new [personAnnotation](../resources/personannotation.md) object in a user's [profile](../resources/profile.md).</span></span>

## <a name="permissions"></a><span data-ttu-id="183eb-106">权限</span><span class="sxs-lookup"><span data-stu-id="183eb-106">Permissions</span></span>

<span data-ttu-id="183eb-p101">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="183eb-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="183eb-109">权限类型</span><span class="sxs-lookup"><span data-stu-id="183eb-109">Permission type</span></span>                        | <span data-ttu-id="183eb-110">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="183eb-110">Permissions (from least to most privileged)</span></span>                                      |
|:---------------------------------------|:---------------------------------------------------------------------------------|
| <span data-ttu-id="183eb-111">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="183eb-111">Delegated (work or school account)</span></span>     | <span data-ttu-id="183eb-112">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="183eb-112">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="183eb-113">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="183eb-113">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="183eb-114">所有用户读写。</span><span class="sxs-lookup"><span data-stu-id="183eb-114">User.ReadWrite, User.ReadWrite.All</span></span> |
| <span data-ttu-id="183eb-115">应用程序</span><span class="sxs-lookup"><span data-stu-id="183eb-115">Application</span></span>                            | <span data-ttu-id="183eb-116">User.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="183eb-116">User.ReadWrite.All</span></span>                            |

## <a name="http-request"></a><span data-ttu-id="183eb-117">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="183eb-117">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /me/profile/notes
POST /users/{id | userPrincipalName}/profile/notes
```

## <a name="request-headers"></a><span data-ttu-id="183eb-118">请求标头</span><span class="sxs-lookup"><span data-stu-id="183eb-118">Request headers</span></span>
|<span data-ttu-id="183eb-119">名称</span><span class="sxs-lookup"><span data-stu-id="183eb-119">Name</span></span>|<span data-ttu-id="183eb-120">说明</span><span class="sxs-lookup"><span data-stu-id="183eb-120">Description</span></span>|
|:---|:---|
|<span data-ttu-id="183eb-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="183eb-121">Authorization</span></span>|<span data-ttu-id="183eb-p102">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="183eb-p102">Bearer {token}. Required.</span></span>|
|<span data-ttu-id="183eb-124">Content-Type</span><span class="sxs-lookup"><span data-stu-id="183eb-124">Content-Type</span></span>|<span data-ttu-id="183eb-p103">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="183eb-p103">application/json. Required.</span></span>|

## <a name="request-body"></a><span data-ttu-id="183eb-127">请求正文</span><span class="sxs-lookup"><span data-stu-id="183eb-127">Request body</span></span>
<span data-ttu-id="183eb-128">在请求正文中，提供 [personAnnotation](../resources/personannotation.md) 对象的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="183eb-128">In the request body, supply a JSON representation of the [personAnnotation](../resources/personannotation.md) object.</span></span>

<span data-ttu-id="183eb-129">下表显示了可以在用户[配置文件](../resources/profile.md)中的新[personAnnotation](../resources/personannotation.md)对象内设置的属性。</span><span class="sxs-lookup"><span data-stu-id="183eb-129">The following table shows the properties that are possible to set within a new [personAnnotation](../resources/personannotation.md) object in a user's [profile](../resources/profile.md).</span></span>

|<span data-ttu-id="183eb-130">属性</span><span class="sxs-lookup"><span data-stu-id="183eb-130">Property</span></span>|<span data-ttu-id="183eb-131">类型</span><span class="sxs-lookup"><span data-stu-id="183eb-131">Type</span></span>|<span data-ttu-id="183eb-132">说明</span><span class="sxs-lookup"><span data-stu-id="183eb-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="183eb-133">allowedAudiences</span><span class="sxs-lookup"><span data-stu-id="183eb-133">allowedAudiences</span></span>|<span data-ttu-id="183eb-134">String</span><span class="sxs-lookup"><span data-stu-id="183eb-134">String</span></span>|<span data-ttu-id="183eb-135">能够查看实体中包含的值的访问群体。</span><span class="sxs-lookup"><span data-stu-id="183eb-135">The audiences that are able to see the values contained within the entity.</span></span> <span data-ttu-id="183eb-136">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="183eb-136">Inherited from [itemFacet](../resources/itemfacet.md).</span></span> <span data-ttu-id="183eb-137">可取值为：`me`、`family`、`contacts`、`groupMembers`、`organization`、`federatedOrganizations`、`everyone`、`unknownFutureValue`。</span><span class="sxs-lookup"><span data-stu-id="183eb-137">Possible values are: `me`, `family`, `contacts`, `groupMembers`, `organization`, `federatedOrganizations`, `everyone`, `unknownFutureValue`.</span></span>|
|<span data-ttu-id="183eb-138">介绍</span><span class="sxs-lookup"><span data-stu-id="183eb-138">detail</span></span>|[<span data-ttu-id="183eb-139">itemBody</span><span class="sxs-lookup"><span data-stu-id="183eb-139">itemBody</span></span>](../resources/itembody.md)|<span data-ttu-id="183eb-140">包含注释本身的详细信息。</span><span class="sxs-lookup"><span data-stu-id="183eb-140">Contains the detail of the note itself.</span></span>|
|<span data-ttu-id="183eb-141">displayName</span><span class="sxs-lookup"><span data-stu-id="183eb-141">displayName</span></span>|<span data-ttu-id="183eb-142">String</span><span class="sxs-lookup"><span data-stu-id="183eb-142">String</span></span>|<span data-ttu-id="183eb-143">包含注解的友好名称。</span><span class="sxs-lookup"><span data-stu-id="183eb-143">Contains a friendly name for the note.</span></span>|
|<span data-ttu-id="183eb-144">推导</span><span class="sxs-lookup"><span data-stu-id="183eb-144">inference</span></span>|[<span data-ttu-id="183eb-145">inferenceData</span><span class="sxs-lookup"><span data-stu-id="183eb-145">inferenceData</span></span>](../resources/inferencedata.md)|<span data-ttu-id="183eb-146">如果实体是由创建或修改应用程序推断的，则包含推理详细信息。</span><span class="sxs-lookup"><span data-stu-id="183eb-146">Contains inference detail if the entity is inferred by the creating or modifying application.</span></span> <span data-ttu-id="183eb-147">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="183eb-147">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|
|<span data-ttu-id="183eb-148">source</span><span class="sxs-lookup"><span data-stu-id="183eb-148">source</span></span>|[<span data-ttu-id="183eb-149">personDataSource</span><span class="sxs-lookup"><span data-stu-id="183eb-149">personDataSource</span></span>](../resources/persondatasource.md)|<span data-ttu-id="183eb-150">值的来源，如果从另一个服务同步。</span><span class="sxs-lookup"><span data-stu-id="183eb-150">Where the values originated if synced from another service.</span></span> <span data-ttu-id="183eb-151">继承自 [itemFacet](../resources/itemfacet.md)。</span><span class="sxs-lookup"><span data-stu-id="183eb-151">Inherited from [itemFacet](../resources/itemfacet.md).</span></span>|

## <a name="response"></a><span data-ttu-id="183eb-152">响应</span><span class="sxs-lookup"><span data-stu-id="183eb-152">Response</span></span>

<span data-ttu-id="183eb-153">如果成功，此方法 `201 Created` 在响应正文中返回响应代码和 [personAnnotation](../resources/personannotation.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="183eb-153">If successful, this method returns a `201 Created` response code and a [personAnnotation](../resources/personannotation.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="183eb-154">示例</span><span class="sxs-lookup"><span data-stu-id="183eb-154">Examples</span></span>

# <a name="http"></a>[<span data-ttu-id="183eb-155">HTTP</span><span class="sxs-lookup"><span data-stu-id="183eb-155">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "create_personannotation_from_"
}
-->
``` http
POST https://graph.microsoft.com/beta/me/profile/notes
Content-Type: application/json
Content-length: 413

{
  "detail": {
    "contentType": "text",
    "content": "I am originally from Australia, but grew up in Moscow, Russia."
  },
  "displayName": "About Me"
}
```
# <a name="c"></a>[<span data-ttu-id="183eb-156">C#</span><span class="sxs-lookup"><span data-stu-id="183eb-156">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/create-personannotation-from--csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="183eb-157">JavaScript</span><span class="sxs-lookup"><span data-stu-id="183eb-157">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/create-personannotation-from--javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="183eb-158">Objective-C</span><span class="sxs-lookup"><span data-stu-id="183eb-158">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/create-personannotation-from--objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="183eb-159">响应</span><span class="sxs-lookup"><span data-stu-id="183eb-159">Response</span></span>
<span data-ttu-id="183eb-160">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="183eb-160">**Note:** The response object shown here might be shortened for readability.</span></span>
<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.personAnnotation"
}
-->
``` http
HTTP/1.1 201 Created
Content-Type: application/json

{
  "id": "0fb4c1e3-c1e3-0fb4-e3c1-b40fe3c1b40f",
  "allowedAudiences": "organization",
  "inference": null,
  "createdDateTime": "2020-07-06T06:34:12.2294868Z",
  "createdBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "lastModifiedDateTime": "2020-07-06T06:34:12.2294868Z",
  "lastModifiedBy": {
    "application": null,
    "device": null,
    "user": {
      "displayName": "Innocenty Popov",
      "id": "db789417-4ccb-41d1-a0a9-47b01a09ea49"
    }
  },
  "detail": {
    "contentType": "text",
    "content": "I am originally from Australia, but grew up in Moscow, Russia."
  },
  "displayName": "About Me"
}
```


