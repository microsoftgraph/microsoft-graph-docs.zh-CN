---
title: passwordCredential 资源类型
description: 包含与应用程序或服务主体相关联的密码凭据。 servicePrincipal 实体和 application 实体的**passwordCredentials**属性是**passwordCredential**的集合。
localization_priority: Normal
ms.openlocfilehash: 900bfb8a5828d636dfa1f1abfd0348ceb4aee143
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32568463"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="117a9-104">passwordCredential 资源类型</span><span class="sxs-lookup"><span data-stu-id="117a9-104">passwordCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="117a9-105">包含与应用程序或服务主体相关联的密码凭据。</span><span class="sxs-lookup"><span data-stu-id="117a9-105">Contains a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="117a9-106">[servicePrincipal](serviceprincipal.md)实体和[application](application.md)实体的**passwordCredentials**属性是**passwordCredential**的集合。</span><span class="sxs-lookup"><span data-stu-id="117a9-106">The **passwordCredentials** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **passwordCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="117a9-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="117a9-107">JSON representation</span></span>

<span data-ttu-id="117a9-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="117a9-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "secretText": "string",
  "hint": "string"
}

```
## <a name="properties"></a><span data-ttu-id="117a9-109">属性</span><span class="sxs-lookup"><span data-stu-id="117a9-109">Properties</span></span>
| <span data-ttu-id="117a9-110">属性</span><span class="sxs-lookup"><span data-stu-id="117a9-110">Property</span></span>     | <span data-ttu-id="117a9-111">类型</span><span class="sxs-lookup"><span data-stu-id="117a9-111">Type</span></span>   |<span data-ttu-id="117a9-112">说明</span><span class="sxs-lookup"><span data-stu-id="117a9-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="117a9-113">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="117a9-113">customKeyIdentifier</span></span>|<span data-ttu-id="117a9-114">Binary</span><span class="sxs-lookup"><span data-stu-id="117a9-114">Binary</span></span>|            |
|<span data-ttu-id="117a9-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="117a9-115">endDateTime</span></span>|<span data-ttu-id="117a9-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="117a9-116">DateTimeOffset</span></span>|<span data-ttu-id="117a9-117">密码过期的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息, 并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="117a9-117">The date and time at which the password expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="117a9-118">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="117a9-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="117a9-119">keyId</span><span class="sxs-lookup"><span data-stu-id="117a9-119">keyId</span></span>|<span data-ttu-id="117a9-120">Guid</span><span class="sxs-lookup"><span data-stu-id="117a9-120">Guid</span></span>|            |
|<span data-ttu-id="117a9-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="117a9-121">startDateTime</span></span>|<span data-ttu-id="117a9-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="117a9-122">DateTimeOffset</span></span>|<span data-ttu-id="117a9-123">密码生效的日期和时间。时间戳类型表示使用 ISO 8601 格式的日期和时间信息, 并且始终采用 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="117a9-123">The date and time at which the password becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="117a9-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="117a9-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="117a9-125">secretText</span><span class="sxs-lookup"><span data-stu-id="117a9-125">secretText</span></span>|<span data-ttu-id="117a9-126">String</span><span class="sxs-lookup"><span data-stu-id="117a9-126">String</span></span>| <span data-ttu-id="117a9-127">密码长度必须为16-64 个字符</span><span class="sxs-lookup"><span data-stu-id="117a9-127">The passwords must be 16-64 characters in length</span></span> |
|<span data-ttu-id="117a9-128">提示</span><span class="sxs-lookup"><span data-stu-id="117a9-128">hint</span></span>|<span data-ttu-id="117a9-129">String</span><span class="sxs-lookup"><span data-stu-id="117a9-129">String</span></span>|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/passwordcredential.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
