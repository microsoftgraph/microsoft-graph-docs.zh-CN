---
title: 更新 relatedContacts
description: 更新 educationUser 对象的 relatedContact 集合。
author: mmast-msft
ms.author: mmast-msft
localization_priority: Normal
ms.prod: education
doc_type: apiPageType
ms.openlocfilehash: f6217c1ea0859de21fa70c53810e825327d497f2
ms.sourcegitcommit: b736af7020db7311f7d28b301752b5669d7badba
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/25/2021
ms.locfileid: "51200898"
---
# <a name="update-relatedcontacts"></a><span data-ttu-id="89d2a-103">更新 relatedContacts</span><span class="sxs-lookup"><span data-stu-id="89d2a-103">Update relatedContacts</span></span>

<span data-ttu-id="89d2a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="89d2a-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="89d2a-105">更新 [educationUser](../resources/relatedContact.md) 对象的 [relatedContact](../resources/educationuser.md) 集合。</span><span class="sxs-lookup"><span data-stu-id="89d2a-105">Update the [relatedContact](../resources/relatedContact.md) collection of an [educationUser](../resources/educationuser.md) object.</span></span>

> [!NOTE]
> <span data-ttu-id="89d2a-106">更新 **relatedContacts** 将替换整个集合。</span><span class="sxs-lookup"><span data-stu-id="89d2a-106">Updating **relatedContacts** replaces the entire collection.</span></span> <span data-ttu-id="89d2a-107">无法添加、删除或更新单个联系人。</span><span class="sxs-lookup"><span data-stu-id="89d2a-107">It is not possible to add, remove, or update a single contact.</span></span>

## <a name="permissions"></a><span data-ttu-id="89d2a-108">权限</span><span class="sxs-lookup"><span data-stu-id="89d2a-108">Permissions</span></span>

<span data-ttu-id="89d2a-p102">要调用此 API，需要以下权限之一。要了解详细信息，包括如何选择权限的信息，请参阅[权限](/graph/permissions-reference)。</span><span class="sxs-lookup"><span data-stu-id="89d2a-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

| <span data-ttu-id="89d2a-111">权限类型</span><span class="sxs-lookup"><span data-stu-id="89d2a-111">Permission type</span></span>                        | <span data-ttu-id="89d2a-112">权限（从最低特权到最高特权）</span><span class="sxs-lookup"><span data-stu-id="89d2a-112">Permissions (from least to most privileged)</span></span> |
| :------------------------------------- | :------------------------------------------ |
| <span data-ttu-id="89d2a-113">委派（工作或学校帐户）</span><span class="sxs-lookup"><span data-stu-id="89d2a-113">Delegated (work or school account)</span></span>     | <span data-ttu-id="89d2a-114">不支持。</span><span class="sxs-lookup"><span data-stu-id="89d2a-114">Not supported.</span></span>                              |
| <span data-ttu-id="89d2a-115">委派（个人 Microsoft 帐户）</span><span class="sxs-lookup"><span data-stu-id="89d2a-115">Delegated (personal Microsoft account)</span></span> | <span data-ttu-id="89d2a-116">不支持。</span><span class="sxs-lookup"><span data-stu-id="89d2a-116">Not supported.</span></span>                              |
| <span data-ttu-id="89d2a-117">应用程序</span><span class="sxs-lookup"><span data-stu-id="89d2a-117">Application</span></span>                            | <span data-ttu-id="89d2a-118">EduRoster.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="89d2a-118">EduRoster.ReadWrite.All</span></span>                     |

## <a name="http-request"></a><span data-ttu-id="89d2a-119">HTTP 请求</span><span class="sxs-lookup"><span data-stu-id="89d2a-119">HTTP request</span></span>

<!-- {
  "blockType": "ignored"
}
-->

```http
PATCH /education/users/{id}
```

## <a name="request-headers"></a><span data-ttu-id="89d2a-120">请求标头</span><span class="sxs-lookup"><span data-stu-id="89d2a-120">Request headers</span></span>

| <span data-ttu-id="89d2a-121">名称</span><span class="sxs-lookup"><span data-stu-id="89d2a-121">Name</span></span>          | <span data-ttu-id="89d2a-122">说明</span><span class="sxs-lookup"><span data-stu-id="89d2a-122">Description</span></span>                 |
| :------------ | :-------------------------- |
| <span data-ttu-id="89d2a-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="89d2a-123">Authorization</span></span> | <span data-ttu-id="89d2a-p103">Bearer {token}。必需。</span><span class="sxs-lookup"><span data-stu-id="89d2a-p103">Bearer {token}. Required.</span></span>   |
| <span data-ttu-id="89d2a-126">Content-Type</span><span class="sxs-lookup"><span data-stu-id="89d2a-126">Content-Type</span></span>  | <span data-ttu-id="89d2a-p104">application/json. Required.</span><span class="sxs-lookup"><span data-stu-id="89d2a-p104">application/json. Required.</span></span> |

## <a name="request-body"></a><span data-ttu-id="89d2a-129">请求正文</span><span class="sxs-lookup"><span data-stu-id="89d2a-129">Request body</span></span>

<span data-ttu-id="89d2a-130">在请求正文中，提供 [relatedContact](../resources/relatedcontact.md) 集合的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89d2a-130">In the request body, supply a JSON representation of the [relatedContact](../resources/relatedcontact.md) collection.</span></span>

<span data-ttu-id="89d2a-131">下表显示更新 [educationUser](../resources/educationuser.md)时所需的属性。</span><span class="sxs-lookup"><span data-stu-id="89d2a-131">The following table shows the properties that are required when you update the [educationUser](../resources/educationuser.md).</span></span>

| <span data-ttu-id="89d2a-132">属性</span><span class="sxs-lookup"><span data-stu-id="89d2a-132">Property</span></span>        | <span data-ttu-id="89d2a-133">类型</span><span class="sxs-lookup"><span data-stu-id="89d2a-133">Type</span></span>                                                        | <span data-ttu-id="89d2a-134">说明</span><span class="sxs-lookup"><span data-stu-id="89d2a-134">Description</span></span>                                    |
| :-------------- | :---------------------------------------------------------- | :--------------------------------------------- |
| <span data-ttu-id="89d2a-135">relatedContacts</span><span class="sxs-lookup"><span data-stu-id="89d2a-135">relatedContacts</span></span> | <span data-ttu-id="89d2a-136">[relatedContact](../resources/relatedcontact.md) 集合</span><span class="sxs-lookup"><span data-stu-id="89d2a-136">[relatedContact](../resources/relatedcontact.md) collection</span></span> | <span data-ttu-id="89d2a-137">用户的完整相关联系人集</span><span class="sxs-lookup"><span data-stu-id="89d2a-137">The complete set of related contact for a user</span></span> |

> [!IMPORTANT]
> <span data-ttu-id="89d2a-138">此更新必须是一个不同的操作。</span><span class="sxs-lookup"><span data-stu-id="89d2a-138">This update must be a distinct operation.</span></span> <span data-ttu-id="89d2a-139">它不能与其他 [educationUser](../resources/educationuser.md) 属性的更新结合使用。</span><span class="sxs-lookup"><span data-stu-id="89d2a-139">It cannot be combined with updates to other [educationUser](../resources/educationuser.md) properties.</span></span>
> <span data-ttu-id="89d2a-140">例如，更新 **relatedContacts** 和 **displayName** 需要两个不同的请求。</span><span class="sxs-lookup"><span data-stu-id="89d2a-140">For example, updating both **relatedContacts** and **displayName** requires two distinct requests.</span></span>

## <a name="response"></a><span data-ttu-id="89d2a-141">响应</span><span class="sxs-lookup"><span data-stu-id="89d2a-141">Response</span></span>

<span data-ttu-id="89d2a-142">如果成功，此方法在响应正文中返回 响应代码和更新的 `200 OK` [educationUser](../resources/educationuser.md) 对象。</span><span class="sxs-lookup"><span data-stu-id="89d2a-142">If successful, this method returns a `200 OK` response code and an updated [educationUser](../resources/educationuser.md) object in the response body.</span></span>

## <a name="examples"></a><span data-ttu-id="89d2a-143">示例</span><span class="sxs-lookup"><span data-stu-id="89d2a-143">Examples</span></span>

### <a name="request"></a><span data-ttu-id="89d2a-144">请求</span><span class="sxs-lookup"><span data-stu-id="89d2a-144">Request</span></span>


# <a name="http"></a>[<span data-ttu-id="89d2a-145">HTTP</span><span class="sxs-lookup"><span data-stu-id="89d2a-145">HTTP</span></span>](#tab/http)
<!-- {
  "blockType": "request",
  "name": "update_educationuser"
}
-->

```http
PATCH https://graph.microsoft.com/beta/education/users/{educationUserId}
Content-Type: application/json
Content-length: 408

{
  "relatedContacts": [
    {
      "displayName": "Father Time",
      "emailAddress": "father@time.com",
      "mobilePhone": "4251231234",
      "relationship": "guardian",
      "accessConsent": true
    },
    {
      "displayName": "Mother Nature",
      "emailAddress": "mother@nature.co.uk",
      "mobilePhone": "3251231234",
      "relationship": "parent",
      "accessConsent": true
    }
  ]
}
```
# <a name="c"></a>[<span data-ttu-id="89d2a-146">C#</span><span class="sxs-lookup"><span data-stu-id="89d2a-146">C#</span></span>](#tab/csharp)
[!INCLUDE [sample-code](../includes/snippets/csharp/update-educationuser-csharp-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="javascript"></a>[<span data-ttu-id="89d2a-147">JavaScript</span><span class="sxs-lookup"><span data-stu-id="89d2a-147">JavaScript</span></span>](#tab/javascript)
[!INCLUDE [sample-code](../includes/snippets/javascript/update-educationuser-javascript-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="objective-c"></a>[<span data-ttu-id="89d2a-148">Objective-C</span><span class="sxs-lookup"><span data-stu-id="89d2a-148">Objective-C</span></span>](#tab/objc)
[!INCLUDE [sample-code](../includes/snippets/objc/update-educationuser-objc-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

# <a name="java"></a>[<span data-ttu-id="89d2a-149">Java</span><span class="sxs-lookup"><span data-stu-id="89d2a-149">Java</span></span>](#tab/java)
[!INCLUDE [sample-code](../includes/snippets/java/update-educationuser-java-snippets.md)]
[!INCLUDE [sdk-documentation](../includes/snippets/snippets-sdk-documentation-link.md)]

---


### <a name="response"></a><span data-ttu-id="89d2a-150">响应</span><span class="sxs-lookup"><span data-stu-id="89d2a-150">Response</span></span>

<span data-ttu-id="89d2a-151">**注意：** 为了提高可读性，可能缩短了此处显示的响应对象。</span><span class="sxs-lookup"><span data-stu-id="89d2a-151">**Note:** The response object shown here might be shortened for readability.</span></span>

<!-- {
  "blockType": "response",
  "truncated": true,
  "@odata.type": "microsoft.graph.educationUser"
} -->

```http
HTTP/1.1 200 OK
Content-Type: application/json

{
  "id": "4b712dc5-2dc5-4b71-c52d-714bc52d714b",
  "relatedContacts": [
      {
          "displayName": "Father Time",
          "emailAddress": "father@time.com",
          "mobilePhone": "4251231234",
          "relationship": "guardian",
          "accessConsent": true
      },
      {
          "displayName": "Mother Nature",
          "emailAddress": "mother@nature.co.uk",
          "mobilePhone": "3251231234",
          "relationship": "parent",
          "accessConsent": true
      }
  ]
}
```
