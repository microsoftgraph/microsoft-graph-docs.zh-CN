---
title: passwordCredential 资源类型
description: 包含与应用程序或服务主体关联的密码凭据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: f565e847cee968d07bc76399bbbcf8aeaf3d94f6
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50721521"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="3f5ae-103">passwordCredential 资源类型</span><span class="sxs-lookup"><span data-stu-id="3f5ae-103">passwordCredential resource type</span></span>

<span data-ttu-id="3f5ae-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3f5ae-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="3f5ae-105">表示与应用程序或服务主体关联的密码凭据。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-105">Represents a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="3f5ae-106">**应用程序的 passwordCredentials** [属性](application.md)</span><span class="sxs-lookup"><span data-stu-id="3f5ae-106">The **passwordCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md) entitites--> <span data-ttu-id="3f5ae-107">entity 是 **passwordCredential 对象** 的集合。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-107">entity is a collection of **passwordCredential** objects.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="3f5ae-108">不支持使用 POST 或 PATCH 设置 **passwordCredential。**</span><span class="sxs-lookup"><span data-stu-id="3f5ae-108">Using POST or PATCH to set **passwordCredential** is not supported.</span></span> <span data-ttu-id="3f5ae-109">使用 addPassword 和 removePassword 方法更新应用程序或 servicePrincipal 的密码：</span><span class="sxs-lookup"><span data-stu-id="3f5ae-109">Use the addPassword and removePassword methods to update the password for an application or a servicePrincipal:</span></span>
>
> - [<span data-ttu-id="3f5ae-110">application： addPassword</span><span class="sxs-lookup"><span data-stu-id="3f5ae-110">application: addPassword</span></span>](../api/application-addpassword.md)
> - [<span data-ttu-id="3f5ae-111">application： removePassword</span><span class="sxs-lookup"><span data-stu-id="3f5ae-111">application: removePassword</span></span>](../api/application-removepassword.md)
> - [<span data-ttu-id="3f5ae-112">servicePrincipal：addPassword</span><span class="sxs-lookup"><span data-stu-id="3f5ae-112">servicePrincipal: addPassword</span></span>](../api/serviceprincipal-addpassword.md)
> - [<span data-ttu-id="3f5ae-113">servicePrincipal：removePassword</span><span class="sxs-lookup"><span data-stu-id="3f5ae-113">servicePrincipal: removePassword</span></span>](../api/serviceprincipal-removepassword.md)

## <a name="properties"></a><span data-ttu-id="3f5ae-114">属性</span><span class="sxs-lookup"><span data-stu-id="3f5ae-114">Properties</span></span>
| <span data-ttu-id="3f5ae-115">属性</span><span class="sxs-lookup"><span data-stu-id="3f5ae-115">Property</span></span>     | <span data-ttu-id="3f5ae-116">类型</span><span class="sxs-lookup"><span data-stu-id="3f5ae-116">Type</span></span>   |<span data-ttu-id="3f5ae-117">说明</span><span class="sxs-lookup"><span data-stu-id="3f5ae-117">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="3f5ae-118">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="3f5ae-118">customKeyIdentifier</span></span> | <span data-ttu-id="3f5ae-119">Binary</span><span class="sxs-lookup"><span data-stu-id="3f5ae-119">Binary</span></span> | <span data-ttu-id="3f5ae-120">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-120">Do not use.</span></span> |
| <span data-ttu-id="3f5ae-121">displayName</span><span class="sxs-lookup"><span data-stu-id="3f5ae-121">displayName</span></span> | <span data-ttu-id="3f5ae-122">字符串</span><span class="sxs-lookup"><span data-stu-id="3f5ae-122">String</span></span> | <span data-ttu-id="3f5ae-123">密码的友好名称。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-123">Friendly name for the password.</span></span> <span data-ttu-id="3f5ae-124">可选。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-124">Optional.</span></span> |
| <span data-ttu-id="3f5ae-125">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3f5ae-125">endDateTime</span></span> | <span data-ttu-id="3f5ae-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f5ae-126">DateTimeOffset</span></span> | <span data-ttu-id="3f5ae-127">密码过期的日期和时间使用 ISO 8601 格式表示，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-127">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3f5ae-128">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-128">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="3f5ae-129">可选。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-129">Optional.</span></span> |
| <span data-ttu-id="3f5ae-130">hint</span><span class="sxs-lookup"><span data-stu-id="3f5ae-130">hint</span></span> | <span data-ttu-id="3f5ae-131">字符串</span><span class="sxs-lookup"><span data-stu-id="3f5ae-131">String</span></span> | <span data-ttu-id="3f5ae-132">包含密码的前三个字符。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-132">Contains the first three characters of the password.</span></span> <span data-ttu-id="3f5ae-133">只读。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-133">Read-only.</span></span> |
| <span data-ttu-id="3f5ae-134">keyId</span><span class="sxs-lookup"><span data-stu-id="3f5ae-134">keyId</span></span> | <span data-ttu-id="3f5ae-135">Guid</span><span class="sxs-lookup"><span data-stu-id="3f5ae-135">Guid</span></span> | <span data-ttu-id="3f5ae-136">密码的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-136">The unique identifier for the password.</span></span> |
| <span data-ttu-id="3f5ae-137">secretText</span><span class="sxs-lookup"><span data-stu-id="3f5ae-137">secretText</span></span> | <span data-ttu-id="3f5ae-138">字符串</span><span class="sxs-lookup"><span data-stu-id="3f5ae-138">String</span></span> | <span data-ttu-id="3f5ae-139">只读;包含 Azure AD 生成的长度为 16-64 个字符的强密码。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-139">Read-only; Contains the strong passwords generated by Azure AD that are 16-64 characters in length.</span></span> <span data-ttu-id="3f5ae-140">生成的密码值仅在初始 POST 请求 [addPassword 期间返回](../api/application-addpassword.md)。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-140">The generated password value is only returned during the initial POST request to [addPassword](../api/application-addpassword.md).</span></span> <span data-ttu-id="3f5ae-141">将来无法检索此密码。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-141">There is no way to retrieve this password in the future.</span></span> |
| <span data-ttu-id="3f5ae-142">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3f5ae-142">startDateTime</span></span> | <span data-ttu-id="3f5ae-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3f5ae-143">DateTimeOffset</span></span> | <span data-ttu-id="3f5ae-144">密码生效的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-144">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="3f5ae-145">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-145">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3f5ae-146">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-146">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`.</span></span> <span data-ttu-id="3f5ae-147">可选。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-147">Optional.</span></span> |

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


## <a name="json-representation"></a><span data-ttu-id="3f5ae-148">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3f5ae-148">JSON representation</span></span>

<span data-ttu-id="3f5ae-149">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3f5ae-149">The following is a JSON representation of the resource.</span></span>

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

