---
title: passwordCredential 资源类型
description: 包含与应用程序或服务主体相关联的密码凭据。 ServicePrincipal 实体和 application 实体的**passwordCredentials**属性是**passwordCredential**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 9d7b1013d572f98f10634ac6470367fd44ffbb66
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37938854"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="07a2f-104">passwordCredential 资源类型</span><span class="sxs-lookup"><span data-stu-id="07a2f-104">passwordCredential resource type</span></span>

<span data-ttu-id="07a2f-105">表示与应用程序或服务主体相关联的密码凭据。</span><span class="sxs-lookup"><span data-stu-id="07a2f-105">Represents a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="07a2f-106">[应用程序](application.md)的**passwordCredentials**属性</span><span class="sxs-lookup"><span data-stu-id="07a2f-106">The **passwordCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md) entitites--> <span data-ttu-id="07a2f-107">entity 是**passwordCredential**对象的集合。</span><span class="sxs-lookup"><span data-stu-id="07a2f-107">entity is a collection of **passwordCredential** objects.</span></span>

> <span data-ttu-id="07a2f-108">注意：不支持使用修补程序更新 passwordCredentials。</span><span class="sxs-lookup"><span data-stu-id="07a2f-108">Note: Using PATCH to update passwordCredentials is not supported.</span></span> <span data-ttu-id="07a2f-109">使用 addPassword 和 removePassword 方法更新应用程序的密码</span><span class="sxs-lookup"><span data-stu-id="07a2f-109">Use use the addPassword and removePassword methods to update the password for an application</span></span> <!--or a servicePrincipal--><span data-ttu-id="07a2f-110">.</span><span class="sxs-lookup"><span data-stu-id="07a2f-110"></span></span>
>
> - <span data-ttu-id="07a2f-111">应用程序[addPassword](../api/application-addpassword.md)</span><span class="sxs-lookup"><span data-stu-id="07a2f-111">application - [addPassword](../api/application-addpassword.md)</span></span>
> - <span data-ttu-id="07a2f-112">应用程序[removePassword](../api/application-removepassword.md)</span><span class="sxs-lookup"><span data-stu-id="07a2f-112">application - [removePassword](../api/application-removepassword.md)</span></span>
<!--
> - servicePrincipal - [addPassword](../api/serviceprincipal-addpassword.md)
> - servicePrincipal - [removePassword](../api/serviceprincipal-removepassword.md)
-->

## <a name="properties"></a><span data-ttu-id="07a2f-113">属性</span><span class="sxs-lookup"><span data-stu-id="07a2f-113">Properties</span></span>
| <span data-ttu-id="07a2f-114">属性</span><span class="sxs-lookup"><span data-stu-id="07a2f-114">Property</span></span>     | <span data-ttu-id="07a2f-115">类型</span><span class="sxs-lookup"><span data-stu-id="07a2f-115">Type</span></span>   |<span data-ttu-id="07a2f-116">描述</span><span class="sxs-lookup"><span data-stu-id="07a2f-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="07a2f-117">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="07a2f-117">customKeyIdentifier</span></span> | <span data-ttu-id="07a2f-118">Binary</span><span class="sxs-lookup"><span data-stu-id="07a2f-118">Binary</span></span> | <span data-ttu-id="07a2f-119">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="07a2f-119">Do not use.</span></span> |
| <span data-ttu-id="07a2f-120">displayName</span><span class="sxs-lookup"><span data-stu-id="07a2f-120">displayName</span></span> | <span data-ttu-id="07a2f-121">String</span><span class="sxs-lookup"><span data-stu-id="07a2f-121">String</span></span> | <span data-ttu-id="07a2f-122">密码的友好名称。</span><span class="sxs-lookup"><span data-stu-id="07a2f-122">Friendly name for the password.</span></span> <span data-ttu-id="07a2f-123">可选。</span><span class="sxs-lookup"><span data-stu-id="07a2f-123">Optional.</span></span> |
| <span data-ttu-id="07a2f-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="07a2f-124">endDateTime</span></span> | <span data-ttu-id="07a2f-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07a2f-125">DateTimeOffset</span></span> | <span data-ttu-id="07a2f-126">密码过期的日期和时间，使用 ISO 8601 格式表示，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="07a2f-126">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="07a2f-127">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="07a2f-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="07a2f-128">可选。</span><span class="sxs-lookup"><span data-stu-id="07a2f-128">Optional.</span></span> |
| <span data-ttu-id="07a2f-129">提示</span><span class="sxs-lookup"><span data-stu-id="07a2f-129">hint</span></span> | <span data-ttu-id="07a2f-130">String</span><span class="sxs-lookup"><span data-stu-id="07a2f-130">String</span></span> | <span data-ttu-id="07a2f-131">包含密码的前三个字符。</span><span class="sxs-lookup"><span data-stu-id="07a2f-131">Contains the first three characters of the password.</span></span> <span data-ttu-id="07a2f-132">只读。</span><span class="sxs-lookup"><span data-stu-id="07a2f-132">Read-only.</span></span> |
| <span data-ttu-id="07a2f-133">keyId</span><span class="sxs-lookup"><span data-stu-id="07a2f-133">keyId</span></span> | <span data-ttu-id="07a2f-134">Guid</span><span class="sxs-lookup"><span data-stu-id="07a2f-134">Guid</span></span> | <span data-ttu-id="07a2f-135">密码的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="07a2f-135">The unique identifier for the password.</span></span> |
| <span data-ttu-id="07a2f-136">secretText</span><span class="sxs-lookup"><span data-stu-id="07a2f-136">secretText</span></span> | <span data-ttu-id="07a2f-137">String</span><span class="sxs-lookup"><span data-stu-id="07a2f-137">String</span></span> | <span data-ttu-id="07a2f-138">只读;包含由 Azure AD 生成的强密码，其长度为16-64 个字符。</span><span class="sxs-lookup"><span data-stu-id="07a2f-138">Read-only; Contains the strong passwords generated by Azure AD that are 16-64 characters in length.</span></span> <span data-ttu-id="07a2f-139">生成的密码值仅在初始 POST 请求过程中返回到[addPassword](../api/application-addpassword.md)。</span><span class="sxs-lookup"><span data-stu-id="07a2f-139">The generated password value is only returned during the initial POST request to [addPassword](../api/application-addpassword.md).</span></span> <span data-ttu-id="07a2f-140">将来无法检索此密码。</span><span class="sxs-lookup"><span data-stu-id="07a2f-140">There is no way to retrieve this password in the future.</span></span> |
| <span data-ttu-id="07a2f-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="07a2f-141">startDateTime</span></span> | <span data-ttu-id="07a2f-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="07a2f-142">DateTimeOffset</span></span> | <span data-ttu-id="07a2f-143">密码生效的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="07a2f-143">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="07a2f-144">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="07a2f-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="07a2f-145">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="07a2f-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="07a2f-146">可选。</span><span class="sxs-lookup"><span data-stu-id="07a2f-146">Optional.</span></span> |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


## <a name="json-representation"></a><span data-ttu-id="07a2f-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="07a2f-147">JSON representation</span></span>

<span data-ttu-id="07a2f-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="07a2f-148">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential",
  "baseType": null
}-->

```json
{
  "customKeyIdentifier": "Binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "hint": "String",
  "keyId": "Guid",
  "secretText": "String",
  "startDateTime": "String (timestamp)"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
