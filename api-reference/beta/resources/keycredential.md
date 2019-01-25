---
title: keyCredential 资源类型
description: 包含与应用程序或服务主体关键凭据。 应用程序和 servicePrincipal 实体的**keyCredentials**属性是**keyCredential**的集合。
localization_priority: Normal
ms.openlocfilehash: 87223ab77bc18ca57fb2bd9635cd0790f0651fb7
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519050"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="3049a-104">keyCredential 资源类型</span><span class="sxs-lookup"><span data-stu-id="3049a-104">keyCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3049a-105">包含与应用程序或服务主体关键凭据。</span><span class="sxs-lookup"><span data-stu-id="3049a-105">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="3049a-106">[应用程序](application.md)和[servicePrincipal](serviceprincipal.md)实体的**keyCredentials**属性是**keyCredential**的集合。</span><span class="sxs-lookup"><span data-stu-id="3049a-106">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="3049a-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3049a-107">JSON representation</span></span>

<span data-ttu-id="3049a-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3049a-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="3049a-109">属性</span><span class="sxs-lookup"><span data-stu-id="3049a-109">Properties</span></span>
| <span data-ttu-id="3049a-110">属性</span><span class="sxs-lookup"><span data-stu-id="3049a-110">Property</span></span>     | <span data-ttu-id="3049a-111">类型</span><span class="sxs-lookup"><span data-stu-id="3049a-111">Type</span></span>   |<span data-ttu-id="3049a-112">说明</span><span class="sxs-lookup"><span data-stu-id="3049a-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="3049a-113">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="3049a-113">customKeyIdentifier</span></span>|<span data-ttu-id="3049a-114">Binary</span><span class="sxs-lookup"><span data-stu-id="3049a-114">Binary</span></span>| <span data-ttu-id="3049a-115">自定义的密钥标识符</span><span class="sxs-lookup"><span data-stu-id="3049a-115">Custom key identifier</span></span> |
|<span data-ttu-id="3049a-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="3049a-116">endDateTime</span></span>|<span data-ttu-id="3049a-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3049a-117">DateTimeOffset</span></span>|<span data-ttu-id="3049a-118">过期日期和时间的凭据。时间戳类型表示使用 ISO 8601 格式的日期和时间信息且始终在 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="3049a-118">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3049a-119">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3049a-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3049a-120">密钥 id 为</span><span class="sxs-lookup"><span data-stu-id="3049a-120">keyId</span></span>|<span data-ttu-id="3049a-121">Guid</span><span class="sxs-lookup"><span data-stu-id="3049a-121">Guid</span></span>|<span data-ttu-id="3049a-122">唯一标识符 (GUID) 键。</span><span class="sxs-lookup"><span data-stu-id="3049a-122">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="3049a-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="3049a-123">startDateTime</span></span>|<span data-ttu-id="3049a-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3049a-124">DateTimeOffset</span></span>|<span data-ttu-id="3049a-125">日期和时间凭据生效。时间戳类型表示使用 ISO 8601 格式的日期和时间信息且始终在 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="3049a-125">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3049a-126">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="3049a-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="3049a-127">type</span><span class="sxs-lookup"><span data-stu-id="3049a-127">type</span></span>|<span data-ttu-id="3049a-128">String</span><span class="sxs-lookup"><span data-stu-id="3049a-128">String</span></span>|<span data-ttu-id="3049a-129">类型的关键凭据;例如，"对称"。</span><span class="sxs-lookup"><span data-stu-id="3049a-129">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="3049a-130">使用情况</span><span class="sxs-lookup"><span data-stu-id="3049a-130">usage</span></span>|<span data-ttu-id="3049a-131">String</span><span class="sxs-lookup"><span data-stu-id="3049a-131">String</span></span>|<span data-ttu-id="3049a-132">描述其密钥可用于; 用途的字符串例如，"验证"。</span><span class="sxs-lookup"><span data-stu-id="3049a-132">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="3049a-133">key</span><span class="sxs-lookup"><span data-stu-id="3049a-133">key</span></span>|<span data-ttu-id="3049a-134">二进制</span><span class="sxs-lookup"><span data-stu-id="3049a-134">Binary</span></span>|            |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/keycredential.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
