---
title: keyCredential 资源类型
description: 包含与应用程序或服务主体关键凭据。 应用程序和 servicePrincipal 实体的**keyCredentials**属性是**keyCredential**的集合。
ms.openlocfilehash: d4509360c0425c255566b9f77b9ecd96cf349dec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27041792"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="f3c4a-104">keyCredential 资源类型</span><span class="sxs-lookup"><span data-stu-id="f3c4a-104">keyCredential resource type</span></span>

> <span data-ttu-id="f3c4a-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="f3c4a-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f3c4a-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="f3c4a-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="f3c4a-107">包含与应用程序或服务主体关键凭据。</span><span class="sxs-lookup"><span data-stu-id="f3c4a-107">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="f3c4a-108">[应用程序](application.md)和[servicePrincipal](serviceprincipal.md)实体的**keyCredentials**属性是**keyCredential**的集合。</span><span class="sxs-lookup"><span data-stu-id="f3c4a-108">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="f3c4a-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f3c4a-109">JSON representation</span></span>

<span data-ttu-id="f3c4a-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f3c4a-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="f3c4a-111">属性</span><span class="sxs-lookup"><span data-stu-id="f3c4a-111">Properties</span></span>
| <span data-ttu-id="f3c4a-112">属性</span><span class="sxs-lookup"><span data-stu-id="f3c4a-112">Property</span></span>     | <span data-ttu-id="f3c4a-113">类型</span><span class="sxs-lookup"><span data-stu-id="f3c4a-113">Type</span></span>   |<span data-ttu-id="f3c4a-114">说明</span><span class="sxs-lookup"><span data-stu-id="f3c4a-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f3c4a-115">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="f3c4a-115">customKeyIdentifier</span></span>|<span data-ttu-id="f3c4a-116">二进制数</span><span class="sxs-lookup"><span data-stu-id="f3c4a-116">Binary</span></span>| <span data-ttu-id="f3c4a-117">自定义的密钥标识符</span><span class="sxs-lookup"><span data-stu-id="f3c4a-117">Custom key identifier</span></span> |
|<span data-ttu-id="f3c4a-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="f3c4a-118">endDateTime</span></span>|<span data-ttu-id="f3c4a-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3c4a-119">DateTimeOffset</span></span>|<span data-ttu-id="f3c4a-120">过期日期和时间的凭据。时间戳类型表示使用 ISO 8601 格式的日期和时间信息且始终在 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="f3c4a-120">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f3c4a-121">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f3c4a-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f3c4a-122">密钥 id 为</span><span class="sxs-lookup"><span data-stu-id="f3c4a-122">keyId</span></span>|<span data-ttu-id="f3c4a-123">Guid</span><span class="sxs-lookup"><span data-stu-id="f3c4a-123">Guid</span></span>|<span data-ttu-id="f3c4a-124">唯一标识符 (GUID) 键。</span><span class="sxs-lookup"><span data-stu-id="f3c4a-124">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="f3c4a-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="f3c4a-125">startDateTime</span></span>|<span data-ttu-id="f3c4a-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f3c4a-126">DateTimeOffset</span></span>|<span data-ttu-id="f3c4a-127">日期和时间凭据生效。时间戳类型表示使用 ISO 8601 格式的日期和时间信息且始终在 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="f3c4a-127">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f3c4a-128">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f3c4a-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f3c4a-129">type</span><span class="sxs-lookup"><span data-stu-id="f3c4a-129">type</span></span>|<span data-ttu-id="f3c4a-130">字符串</span><span class="sxs-lookup"><span data-stu-id="f3c4a-130">String</span></span>|<span data-ttu-id="f3c4a-131">类型的关键凭据;例如，"对称"。</span><span class="sxs-lookup"><span data-stu-id="f3c4a-131">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="f3c4a-132">使用情况</span><span class="sxs-lookup"><span data-stu-id="f3c4a-132">usage</span></span>|<span data-ttu-id="f3c4a-133">字符串</span><span class="sxs-lookup"><span data-stu-id="f3c4a-133">String</span></span>|<span data-ttu-id="f3c4a-134">描述其密钥可用于; 用途的字符串例如，"验证"。</span><span class="sxs-lookup"><span data-stu-id="f3c4a-134">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="f3c4a-135">key</span><span class="sxs-lookup"><span data-stu-id="f3c4a-135">key</span></span>|<span data-ttu-id="f3c4a-136">二进制</span><span class="sxs-lookup"><span data-stu-id="f3c4a-136">Binary</span></span>|            |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->