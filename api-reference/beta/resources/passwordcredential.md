---
title: passwordCredential 资源类型
description: 包含与应用程序或服务主体相关联的密码凭据。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: 25b2070a7a665bf6893ad870a7a3111ae9eba80f
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998214"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="bf564-103">passwordCredential 资源类型</span><span class="sxs-lookup"><span data-stu-id="bf564-103">passwordCredential resource type</span></span>

<span data-ttu-id="bf564-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="bf564-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="bf564-105">表示与应用程序或服务主体相关联的密码凭据。</span><span class="sxs-lookup"><span data-stu-id="bf564-105">Represents a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="bf564-106">[Application](application.md)和[ServicePrincipal](serviceprincipal.md) entitites 的**passwordCredentials**属性是**passwordCredential**对象的集合。</span><span class="sxs-lookup"><span data-stu-id="bf564-106">The **passwordCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entitites is a collection of **passwordCredential** objects.</span></span>

> [!IMPORTANT]
> <span data-ttu-id="bf564-107">不支持使用 POST 或 PATCH 设置 **passwordCredential** 。</span><span class="sxs-lookup"><span data-stu-id="bf564-107">Using POST or PATCH to set **passwordCredential** is not supported.</span></span> <span data-ttu-id="bf564-108">使用 addPassword 和 removePassword 方法更新应用程序或 servicePrincipal 的密码：</span><span class="sxs-lookup"><span data-stu-id="bf564-108">Use the addPassword and removePassword methods to update the password for an application or a servicePrincipal:</span></span>
>
> - [<span data-ttu-id="bf564-109">应用程序： addPassword</span><span class="sxs-lookup"><span data-stu-id="bf564-109">application: addPassword</span></span>](../api/application-addpassword.md)
> - [<span data-ttu-id="bf564-110">应用程序： removePassword</span><span class="sxs-lookup"><span data-stu-id="bf564-110">application: removePassword</span></span>](../api/application-removepassword.md)
> - [<span data-ttu-id="bf564-111">servicePrincipal： addPassword</span><span class="sxs-lookup"><span data-stu-id="bf564-111">servicePrincipal: addPassword</span></span>](../api/serviceprincipal-addpassword.md)
> - [<span data-ttu-id="bf564-112">servicePrincipal： removePassword</span><span class="sxs-lookup"><span data-stu-id="bf564-112">servicePrincipal: removePassword</span></span>](../api/serviceprincipal-removepassword.md)


## <a name="properties"></a><span data-ttu-id="bf564-113">属性</span><span class="sxs-lookup"><span data-stu-id="bf564-113">Properties</span></span>
| <span data-ttu-id="bf564-114">属性</span><span class="sxs-lookup"><span data-stu-id="bf564-114">Property</span></span>     | <span data-ttu-id="bf564-115">类型</span><span class="sxs-lookup"><span data-stu-id="bf564-115">Type</span></span>   |<span data-ttu-id="bf564-116">说明</span><span class="sxs-lookup"><span data-stu-id="bf564-116">Description</span></span>|
|:---------------|:--------|:----------|
| <span data-ttu-id="bf564-117">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="bf564-117">customKeyIdentifier</span></span> | <span data-ttu-id="bf564-118">Binary</span><span class="sxs-lookup"><span data-stu-id="bf564-118">Binary</span></span> | <span data-ttu-id="bf564-119">请勿使用。</span><span class="sxs-lookup"><span data-stu-id="bf564-119">Do not use.</span></span> |
| <span data-ttu-id="bf564-120">displayName</span><span class="sxs-lookup"><span data-stu-id="bf564-120">displayName</span></span> | <span data-ttu-id="bf564-121">String</span><span class="sxs-lookup"><span data-stu-id="bf564-121">String</span></span> | <span data-ttu-id="bf564-122">密码的友好名称。</span><span class="sxs-lookup"><span data-stu-id="bf564-122">Friendly name for the password.</span></span> <span data-ttu-id="bf564-123">可选。</span><span class="sxs-lookup"><span data-stu-id="bf564-123">Optional.</span></span> |
| <span data-ttu-id="bf564-124">endDateTime</span><span class="sxs-lookup"><span data-stu-id="bf564-124">endDateTime</span></span> | <span data-ttu-id="bf564-125">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf564-125">DateTimeOffset</span></span> | <span data-ttu-id="bf564-126">密码过期的日期和时间，使用 ISO 8601 格式表示，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="bf564-126">The date and time at which the password expires represented using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bf564-127">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="bf564-127">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="bf564-128">可选。</span><span class="sxs-lookup"><span data-stu-id="bf564-128">Optional.</span></span> |
| <span data-ttu-id="bf564-129">提示</span><span class="sxs-lookup"><span data-stu-id="bf564-129">hint</span></span> | <span data-ttu-id="bf564-130">String</span><span class="sxs-lookup"><span data-stu-id="bf564-130">String</span></span> | <span data-ttu-id="bf564-131">包含密码的前三个字符。</span><span class="sxs-lookup"><span data-stu-id="bf564-131">Contains the first three characters of the password.</span></span> <span data-ttu-id="bf564-132">只读。</span><span class="sxs-lookup"><span data-stu-id="bf564-132">Read-only.</span></span> |
| <span data-ttu-id="bf564-133">keyId</span><span class="sxs-lookup"><span data-stu-id="bf564-133">keyId</span></span> | <span data-ttu-id="bf564-134">Guid</span><span class="sxs-lookup"><span data-stu-id="bf564-134">Guid</span></span> | <span data-ttu-id="bf564-135">密码的唯一标识符。</span><span class="sxs-lookup"><span data-stu-id="bf564-135">The unique identifier for the password.</span></span> |
| <span data-ttu-id="bf564-136">secretText</span><span class="sxs-lookup"><span data-stu-id="bf564-136">secretText</span></span> | <span data-ttu-id="bf564-137">String</span><span class="sxs-lookup"><span data-stu-id="bf564-137">String</span></span> | <span data-ttu-id="bf564-138">只读;包含由 Azure AD 生成的强密码，其长度为16-64 个字符。</span><span class="sxs-lookup"><span data-stu-id="bf564-138">Read-only; Contains the strong passwords generated by Azure AD that are 16-64 characters in length.</span></span> <span data-ttu-id="bf564-139">生成的密码值仅在初始 POST 请求过程中返回到 [addPassword](../api/application-addpassword.md)。</span><span class="sxs-lookup"><span data-stu-id="bf564-139">The generated password value is only returned during the initial POST request to [addPassword](../api/application-addpassword.md).</span></span> <span data-ttu-id="bf564-140">将来无法检索此密码。</span><span class="sxs-lookup"><span data-stu-id="bf564-140">There is no way to retrieve this password in the future.</span></span> |
| <span data-ttu-id="bf564-141">startDateTime</span><span class="sxs-lookup"><span data-stu-id="bf564-141">startDateTime</span></span> | <span data-ttu-id="bf564-142">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="bf564-142">DateTimeOffset</span></span> | <span data-ttu-id="bf564-143">密码生效的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="bf564-143">The date and time at which the password becomes valid.</span></span> <span data-ttu-id="bf564-144">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="bf564-144">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="bf564-145">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="bf564-145">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="bf564-146">可选。</span><span class="sxs-lookup"><span data-stu-id="bf564-146">Optional.</span></span> |

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


## <a name="json-representation"></a><span data-ttu-id="bf564-147">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="bf564-147">JSON representation</span></span>

<span data-ttu-id="bf564-148">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="bf564-148">The following is a JSON representation of the resource.</span></span>

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


