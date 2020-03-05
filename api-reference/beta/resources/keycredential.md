---
title: keyCredential 资源类型
description: 包含与应用程序或服务主体相关联的密钥凭据。 Application 和 servicePrincipal 实体的**keyCredentials**属性是**keyCredential**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 507ea4283ae34e0148d84cd8f76036880a255e98
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42523028"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="c4b03-104">keyCredential 资源类型</span><span class="sxs-lookup"><span data-stu-id="c4b03-104">keyCredential resource type</span></span>

<span data-ttu-id="c4b03-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="c4b03-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c4b03-106">包含与应用程序或服务主体相关联的密钥凭据。</span><span class="sxs-lookup"><span data-stu-id="c4b03-106">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="c4b03-107">[Application](application.md)和[ServicePrincipal](serviceprincipal.md)实体的**keyCredentials**属性是**keyCredential**的集合。</span><span class="sxs-lookup"><span data-stu-id="c4b03-107">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="c4b03-108">属性</span><span class="sxs-lookup"><span data-stu-id="c4b03-108">Properties</span></span>
| <span data-ttu-id="c4b03-109">属性</span><span class="sxs-lookup"><span data-stu-id="c4b03-109">Property</span></span>     | <span data-ttu-id="c4b03-110">类型</span><span class="sxs-lookup"><span data-stu-id="c4b03-110">Type</span></span>   |<span data-ttu-id="c4b03-111">说明</span><span class="sxs-lookup"><span data-stu-id="c4b03-111">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c4b03-112">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="c4b03-112">customKeyIdentifier</span></span>|<span data-ttu-id="c4b03-113">Binary</span><span class="sxs-lookup"><span data-stu-id="c4b03-113">Binary</span></span>| <span data-ttu-id="c4b03-114">自定义密钥标识符</span><span class="sxs-lookup"><span data-stu-id="c4b03-114">Custom key identifier</span></span> |
| <span data-ttu-id="c4b03-115">displayName</span><span class="sxs-lookup"><span data-stu-id="c4b03-115">displayName</span></span> | <span data-ttu-id="c4b03-116">String</span><span class="sxs-lookup"><span data-stu-id="c4b03-116">String</span></span> | <span data-ttu-id="c4b03-117">密钥的友好名称。</span><span class="sxs-lookup"><span data-stu-id="c4b03-117">Friendly name for the key.</span></span> <span data-ttu-id="c4b03-118">可选。</span><span class="sxs-lookup"><span data-stu-id="c4b03-118">Optional.</span></span> |
|<span data-ttu-id="c4b03-119">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c4b03-119">endDateTime</span></span>|<span data-ttu-id="c4b03-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4b03-120">DateTimeOffset</span></span>|<span data-ttu-id="c4b03-121">凭据到期的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="c4b03-121">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c4b03-122">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c4b03-122">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c4b03-123">keyId</span><span class="sxs-lookup"><span data-stu-id="c4b03-123">keyId</span></span>|<span data-ttu-id="c4b03-124">Guid</span><span class="sxs-lookup"><span data-stu-id="c4b03-124">Guid</span></span>|<span data-ttu-id="c4b03-125">键的唯一标识符（GUID）。</span><span class="sxs-lookup"><span data-stu-id="c4b03-125">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="c4b03-126">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c4b03-126">startDateTime</span></span>|<span data-ttu-id="c4b03-127">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c4b03-127">DateTimeOffset</span></span>|<span data-ttu-id="c4b03-128">凭据生效的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="c4b03-128">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c4b03-129">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c4b03-129">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c4b03-130">type</span><span class="sxs-lookup"><span data-stu-id="c4b03-130">type</span></span>|<span data-ttu-id="c4b03-131">String</span><span class="sxs-lookup"><span data-stu-id="c4b03-131">String</span></span>|<span data-ttu-id="c4b03-132">密钥凭据的类型;例如，"对称"。</span><span class="sxs-lookup"><span data-stu-id="c4b03-132">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="c4b03-133">使用率</span><span class="sxs-lookup"><span data-stu-id="c4b03-133">usage</span></span>|<span data-ttu-id="c4b03-134">String</span><span class="sxs-lookup"><span data-stu-id="c4b03-134">String</span></span>|<span data-ttu-id="c4b03-135">一个描述可对其使用密钥的用途的字符串;例如，"Verify"。</span><span class="sxs-lookup"><span data-stu-id="c4b03-135">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="c4b03-136">key</span><span class="sxs-lookup"><span data-stu-id="c4b03-136">key</span></span>|<span data-ttu-id="c4b03-137">二进制</span><span class="sxs-lookup"><span data-stu-id="c4b03-137">Binary</span></span>| <span data-ttu-id="c4b03-138">密钥凭据的值。</span><span class="sxs-lookup"><span data-stu-id="c4b03-138">Value for the key credential.</span></span> <span data-ttu-id="c4b03-139">应为 base 64 编码值。</span><span class="sxs-lookup"><span data-stu-id="c4b03-139">Should be a base 64 encoded value.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c4b03-140">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c4b03-140">JSON representation</span></span>

<span data-ttu-id="c4b03-141">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c4b03-141">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "displayName": "String",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
