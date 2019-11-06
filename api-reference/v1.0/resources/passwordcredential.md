---
title: passwordCredential 资源类型
description: 包含与应用程序或服务主体相关联的密码凭据。 ServicePrincipal 实体和 application 实体的**passwordCredentials**属性是**passwordCredential**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 4aebabc02ec673534d789542af33d74d6ede4eea
ms.sourcegitcommit: 60dfb2ad9ef17f2918c4ee34ebb74f63e32ce2d3
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/05/2019
ms.locfileid: "37998628"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="aeb5a-104">passwordCredential 资源类型</span><span class="sxs-lookup"><span data-stu-id="aeb5a-104">passwordCredential resource type</span></span>

<span data-ttu-id="aeb5a-105">表示与应用程序或服务主体相关联的密码凭据。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-105">Represents a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="aeb5a-106">[应用程序](application.md)的**passwordCredentials**属性</span><span class="sxs-lookup"><span data-stu-id="aeb5a-106">The **passwordCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md) entitites--> <span data-ttu-id="aeb5a-107">entity 是**passwordCredential**对象的集合。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-107">entity is a collection of **passwordCredential** objects.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="aeb5a-108">不支持使用 POST 或 PATCH 设置**passwordCredential** 。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-108">Using POST or PATCH to set **passwordCredential** is not supported.</span></span> <span data-ttu-id="aeb5a-109">使用 addPassword 和 removePassword 方法更新应用程序的密码</span><span class="sxs-lookup"><span data-stu-id="aeb5a-109">Use the addPassword and removePassword methods to update the password for an application</span></span><!--or a servicePrincipal--><span data-ttu-id="aeb5a-110">:</span><span class="sxs-lookup"><span data-stu-id="aeb5a-110"></span></span>
>
> - [<span data-ttu-id="aeb5a-111">应用程序： addPassword</span><span class="sxs-lookup"><span data-stu-id="aeb5a-111">application: addPassword</span></span>](../api/application-addpassword.md)
> - [<span data-ttu-id="aeb5a-112">应用程序： removePassword</span><span class="sxs-lookup"><span data-stu-id="aeb5a-112">application: removePassword</span></span>](../api/application-removepassword.md)
<!--
> - [servicePrincipal: addPassword](../api/serviceprincipal-addpassword.md)
> - [servicePrincipal: removePassword](../api/serviceprincipal-removepassword.md)
-->

## <a name="properties"></a><span data-ttu-id="aeb5a-113">属性</span><span class="sxs-lookup"><span data-stu-id="aeb5a-113">Properties</span></span>
| <span data-ttu-id="aeb5a-114">属性</span><span class="sxs-lookup"><span data-stu-id="aeb5a-114">Property</span></span>     | <span data-ttu-id="aeb5a-115">类型</span><span class="sxs-lookup"><span data-stu-id="aeb5a-115">Type</span></span>   |<span data-ttu-id="aeb5a-116">说明</span><span class="sxs-lookup"><span data-stu-id="aeb5a-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="aeb5a-117">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="aeb5a-117">customKeyIdentifier</span></span> | <span data-ttu-id="aeb5a-118">Binary</span><span class="sxs-lookup"><span data-stu-id="aeb5a-118">Binary</span></span> | <span data-ttu-id="aeb5a-119">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-119">Do not use.</span></span> |
| <span data-ttu-id="aeb5a-120">displayName</span><span class="sxs-lookup"><span data-stu-id="aeb5a-120">displayName</span></span> | <span data-ttu-id="aeb5a-121">String</span><span class="sxs-lookup"><span data-stu-id="aeb5a-121">String</span></span> | <span data-ttu-id="aeb5a-122">密码的友好名称。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-122">Friendly name for the password.</span></span> <span data-ttu-id="aeb5a-123">可选。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-123">Optional.</span></span> |
| <span data-ttu-id="aeb5a-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="aeb5a-124">endDateTime</span></span> | <span data-ttu-id="aeb5a-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aeb5a-125">DateTimeOffset</span></span> | <span data-ttu-id="aeb5a-126">密码过期的日期和时间，使用 ISO 8601 格式表示，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-126">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aeb5a-127">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="aeb5a-128">可选。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-128">Optional.</span></span> |
| <span data-ttu-id="aeb5a-129">提示</span><span class="sxs-lookup"><span data-stu-id="aeb5a-129">hint</span></span> | <span data-ttu-id="aeb5a-130">String</span><span class="sxs-lookup"><span data-stu-id="aeb5a-130">String</span></span> | <span data-ttu-id="aeb5a-131">包含密码的前三个字符。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-131">Contains the first three characters of the password.</span></span> <span data-ttu-id="aeb5a-132">只读。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-132">Read-only.</span></span> |
| <span data-ttu-id="aeb5a-133">keyId</span><span class="sxs-lookup"><span data-stu-id="aeb5a-133">keyId</span></span> | <span data-ttu-id="aeb5a-134">Guid</span><span class="sxs-lookup"><span data-stu-id="aeb5a-134">Guid</span></span> | <span data-ttu-id="aeb5a-135">密码的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-135">The unique identifier for the password.</span></span> |
| <span data-ttu-id="aeb5a-136">secretText</span><span class="sxs-lookup"><span data-stu-id="aeb5a-136">secretText</span></span> | <span data-ttu-id="aeb5a-137">String</span><span class="sxs-lookup"><span data-stu-id="aeb5a-137">String</span></span> | <span data-ttu-id="aeb5a-138">只读;包含由 Azure AD 生成的强密码，其长度为16-64 个字符。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-138">Read-only; Contains the strong passwords generated by Azure AD that are 16-64 characters in length.</span></span> <span data-ttu-id="aeb5a-139">生成的密码值仅在初始 POST 请求过程中返回到[addPassword](../api/application-addpassword.md)。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-139">The generated password value is only returned during the initial POST request to [addPassword](../api/application-addpassword.md).</span></span> <span data-ttu-id="aeb5a-140">将来无法检索此密码。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-140">There is no way to retrieve this password in the future.</span></span> |
| <span data-ttu-id="aeb5a-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="aeb5a-141">startDateTime</span></span> | <span data-ttu-id="aeb5a-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="aeb5a-142">DateTimeOffset</span></span> | <span data-ttu-id="aeb5a-143">密码生效的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-143">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="aeb5a-144">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="aeb5a-145">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="aeb5a-146">可选。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-146">Optional.</span></span> |

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


## <a name="json-representation"></a><span data-ttu-id="aeb5a-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="aeb5a-147">JSON representation</span></span>

<span data-ttu-id="aeb5a-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="aeb5a-148">The following is a JSON representation of the resource.</span></span>

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
