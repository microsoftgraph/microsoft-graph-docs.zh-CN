---
title: keyCredential 资源类型
description: 包含与应用程序或服务主体相关联的密钥凭据。 application 和 servicePrincipal 实体的**keyCredentials**属性是**keyCredential**的集合。
localization_priority: Normal
ms.openlocfilehash: 312821a91bdbb1ad15e136d2b7fc8f9184df4eac
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345384"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="c9984-104">keyCredential 资源类型</span><span class="sxs-lookup"><span data-stu-id="c9984-104">keyCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c9984-105">包含与应用程序或服务主体相关联的密钥凭据。</span><span class="sxs-lookup"><span data-stu-id="c9984-105">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="c9984-106">[application](application.md)和[servicePrincipal](serviceprincipal.md)实体的**keyCredentials**属性是**keyCredential**的集合。</span><span class="sxs-lookup"><span data-stu-id="c9984-106">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="c9984-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="c9984-107">JSON representation</span></span>

<span data-ttu-id="c9984-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="c9984-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```
## <a name="properties"></a><span data-ttu-id="c9984-109">属性</span><span class="sxs-lookup"><span data-stu-id="c9984-109">Properties</span></span>
| <span data-ttu-id="c9984-110">属性</span><span class="sxs-lookup"><span data-stu-id="c9984-110">Property</span></span>     | <span data-ttu-id="c9984-111">类型</span><span class="sxs-lookup"><span data-stu-id="c9984-111">Type</span></span>   |<span data-ttu-id="c9984-112">说明</span><span class="sxs-lookup"><span data-stu-id="c9984-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c9984-113">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="c9984-113">customKeyIdentifier</span></span>|<span data-ttu-id="c9984-114">Binary</span><span class="sxs-lookup"><span data-stu-id="c9984-114">Binary</span></span>| <span data-ttu-id="c9984-115">自定义密钥标识符</span><span class="sxs-lookup"><span data-stu-id="c9984-115">Custom key identifier</span></span> |
|<span data-ttu-id="c9984-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="c9984-116">endDateTime</span></span>|<span data-ttu-id="c9984-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9984-117">DateTimeOffset</span></span>|<span data-ttu-id="c9984-118">凭据到期的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息, 并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="c9984-118">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c9984-119">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c9984-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c9984-120">keyId</span><span class="sxs-lookup"><span data-stu-id="c9984-120">keyId</span></span>|<span data-ttu-id="c9984-121">Guid</span><span class="sxs-lookup"><span data-stu-id="c9984-121">Guid</span></span>|<span data-ttu-id="c9984-122">键的唯一标识符 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="c9984-122">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="c9984-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="c9984-123">startDateTime</span></span>|<span data-ttu-id="c9984-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c9984-124">DateTimeOffset</span></span>|<span data-ttu-id="c9984-125">凭据生效的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息, 并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="c9984-125">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c9984-126">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c9984-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c9984-127">type</span><span class="sxs-lookup"><span data-stu-id="c9984-127">type</span></span>|<span data-ttu-id="c9984-128">String</span><span class="sxs-lookup"><span data-stu-id="c9984-128">String</span></span>|<span data-ttu-id="c9984-129">密钥凭据的类型;例如, "对称"。</span><span class="sxs-lookup"><span data-stu-id="c9984-129">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="c9984-130">使用率</span><span class="sxs-lookup"><span data-stu-id="c9984-130">usage</span></span>|<span data-ttu-id="c9984-131">String</span><span class="sxs-lookup"><span data-stu-id="c9984-131">String</span></span>|<span data-ttu-id="c9984-132">一个描述可对其使用密钥的用途的字符串;例如, "Verify"。</span><span class="sxs-lookup"><span data-stu-id="c9984-132">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="c9984-133">key</span><span class="sxs-lookup"><span data-stu-id="c9984-133">key</span></span>|<span data-ttu-id="c9984-134">二进制</span><span class="sxs-lookup"><span data-stu-id="c9984-134">Binary</span></span>|            |

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
