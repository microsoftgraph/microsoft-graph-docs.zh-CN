---
title: keyCredential 资源类型
description: 包含与应用程序或服务主体相关联的密钥凭据。 Application 和 servicePrincipal 实体的**keyCredentials**属性是**keyCredential**的集合。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 346ff30ad0479d2b25dc57d09a67cc4ddd5f83bc
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939626"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="c291c-104">keyCredential 资源类型</span><span class="sxs-lookup"><span data-stu-id="c291c-104">keyCredential resource type</span></span>

<span data-ttu-id="c291c-105">包含与应用程序关联的密钥凭据</span><span class="sxs-lookup"><span data-stu-id="c291c-105">Contains a key credential associated with an application</span></span> <!--or a service principal--><span data-ttu-id="c291c-106">.</span><span class="sxs-lookup"><span data-stu-id="c291c-106"></span></span> <span data-ttu-id="c291c-107">[应用程序](application.md)的**keyCredentials**属性</span><span class="sxs-lookup"><span data-stu-id="c291c-107">The **keyCredentials** property of the [application](application.md)</span></span> <!--and [servicePrincipal](serviceprincipal.md)--> <span data-ttu-id="c291c-108">实体是**keyCredential**的集合。</span><span class="sxs-lookup"><span data-stu-id="c291c-108">entity is a collection of **keyCredential**.</span></span>

## <a name="properties"></a><span data-ttu-id="c291c-109">属性</span><span class="sxs-lookup"><span data-stu-id="c291c-109">Properties</span></span>
| <span data-ttu-id="c291c-110">属性</span><span class="sxs-lookup"><span data-stu-id="c291c-110">Property</span></span>     | <span data-ttu-id="c291c-111">类型</span><span class="sxs-lookup"><span data-stu-id="c291c-111">Type</span></span>   |<span data-ttu-id="c291c-112">描述</span><span class="sxs-lookup"><span data-stu-id="c291c-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c291c-113">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="c291c-113">customKeyIdentifier</span></span>|<span data-ttu-id="c291c-114">Binary</span><span class="sxs-lookup"><span data-stu-id="c291c-114">Binary</span></span>| <span data-ttu-id="c291c-115">自定义密钥标识符</span><span class="sxs-lookup"><span data-stu-id="c291c-115">Custom key identifier</span></span> |
| <span data-ttu-id="c291c-116">displayName</span><span class="sxs-lookup"><span data-stu-id="c291c-116">displayName</span></span> | <span data-ttu-id="c291c-117">String</span><span class="sxs-lookup"><span data-stu-id="c291c-117">String</span></span> | <span data-ttu-id="c291c-118">密钥的友好名称。</span><span class="sxs-lookup"><span data-stu-id="c291c-118">Friendly name for the key.</span></span> <span data-ttu-id="c291c-119">可选。</span><span class="sxs-lookup"><span data-stu-id="c291c-119">Optional.</span></span> |
|<span data-ttu-id="c291c-120">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c291c-120">endDateTime</span></span>|<span data-ttu-id="c291c-121">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c291c-121">DateTimeOffset</span></span>|<span data-ttu-id="c291c-122">凭据到期的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="c291c-122">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c291c-123">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c291c-123">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c291c-124">keyId</span><span class="sxs-lookup"><span data-stu-id="c291c-124">keyId</span></span>|<span data-ttu-id="c291c-125">Guid</span><span class="sxs-lookup"><span data-stu-id="c291c-125">Guid</span></span>|<span data-ttu-id="c291c-126">键的唯一标识符（GUID）。</span><span class="sxs-lookup"><span data-stu-id="c291c-126">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="c291c-127">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c291c-127">startDateTime</span></span>|<span data-ttu-id="c291c-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c291c-128">DateTimeOffset</span></span>|<span data-ttu-id="c291c-129">凭据生效的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="c291c-129">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c291c-130">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c291c-130">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c291c-131">type</span><span class="sxs-lookup"><span data-stu-id="c291c-131">type</span></span>|<span data-ttu-id="c291c-132">String</span><span class="sxs-lookup"><span data-stu-id="c291c-132">String</span></span>|<span data-ttu-id="c291c-133">密钥凭据的类型;例如，"对称"。</span><span class="sxs-lookup"><span data-stu-id="c291c-133">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="c291c-134">使用率</span><span class="sxs-lookup"><span data-stu-id="c291c-134">usage</span></span>|<span data-ttu-id="c291c-135">String</span><span class="sxs-lookup"><span data-stu-id="c291c-135">String</span></span>|<span data-ttu-id="c291c-136">一个描述可对其使用密钥的用途的字符串;例如，"Verify"。</span><span class="sxs-lookup"><span data-stu-id="c291c-136">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="c291c-137">key</span><span class="sxs-lookup"><span data-stu-id="c291c-137">key</span></span>|<span data-ttu-id="c291c-138">二进制</span><span class="sxs-lookup"><span data-stu-id="c291c-138">Binary</span></span>| <span data-ttu-id="c291c-139">密钥凭据的值。</span><span class="sxs-lookup"><span data-stu-id="c291c-139">Value for the key credential.</span></span> <span data-ttu-id="c291c-140">应为 base 64 编码值。</span><span class="sxs-lookup"><span data-stu-id="c291c-140">Should be a base 64 encoded value.</span></span> |

## <a name="json-representation"></a><span data-ttu-id="c291c-141">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c291c-141">JSON representation</span></span>

<span data-ttu-id="c291c-142">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c291c-142">Here is a JSON representation of the resource</span></span>

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
