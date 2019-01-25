---
title: passwordCredential 资源类型
description: 包含与应用程序或服务主体密码凭据。 **PasswordCredentials**属性和应用程序实体的 servicePrincipal 实体是**passwordCredential**的集合。
localization_priority: Normal
ms.openlocfilehash: 900bfb8a5828d636dfa1f1abfd0348ceb4aee143
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523146"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="7e401-104">passwordCredential 资源类型</span><span class="sxs-lookup"><span data-stu-id="7e401-104">passwordCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7e401-105">包含与应用程序或服务主体密码凭据。</span><span class="sxs-lookup"><span data-stu-id="7e401-105">Contains a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="7e401-106">**PasswordCredentials**属性和[应用程序](application.md)实体的[servicePrincipal](serviceprincipal.md)实体是**passwordCredential**的集合。</span><span class="sxs-lookup"><span data-stu-id="7e401-106">The **passwordCredentials** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **passwordCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="7e401-107">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7e401-107">JSON representation</span></span>

<span data-ttu-id="7e401-108">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7e401-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="7e401-109">属性</span><span class="sxs-lookup"><span data-stu-id="7e401-109">Properties</span></span>
| <span data-ttu-id="7e401-110">属性</span><span class="sxs-lookup"><span data-stu-id="7e401-110">Property</span></span>     | <span data-ttu-id="7e401-111">类型</span><span class="sxs-lookup"><span data-stu-id="7e401-111">Type</span></span>   |<span data-ttu-id="7e401-112">说明</span><span class="sxs-lookup"><span data-stu-id="7e401-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7e401-113">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="7e401-113">customKeyIdentifier</span></span>|<span data-ttu-id="7e401-114">Binary</span><span class="sxs-lookup"><span data-stu-id="7e401-114">Binary</span></span>|            |
|<span data-ttu-id="7e401-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="7e401-115">endDateTime</span></span>|<span data-ttu-id="7e401-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e401-116">DateTimeOffset</span></span>|<span data-ttu-id="7e401-117">过期日期和时间的密码。时间戳类型表示使用 ISO 8601 格式的日期和时间信息且始终在 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="7e401-117">The date and time at which the password expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7e401-118">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7e401-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7e401-119">密钥 id 为</span><span class="sxs-lookup"><span data-stu-id="7e401-119">keyId</span></span>|<span data-ttu-id="7e401-120">Guid</span><span class="sxs-lookup"><span data-stu-id="7e401-120">Guid</span></span>|            |
|<span data-ttu-id="7e401-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="7e401-121">startDateTime</span></span>|<span data-ttu-id="7e401-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="7e401-122">DateTimeOffset</span></span>|<span data-ttu-id="7e401-123">日期和时间的密码将成为有效。时间戳类型表示使用 ISO 8601 格式的日期和时间信息且始终在 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="7e401-123">The date and time at which the password becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="7e401-124">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="7e401-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="7e401-125">secretText</span><span class="sxs-lookup"><span data-stu-id="7e401-125">secretText</span></span>|<span data-ttu-id="7e401-126">String</span><span class="sxs-lookup"><span data-stu-id="7e401-126">String</span></span>| <span data-ttu-id="7e401-127">密码必须为 16-64 个字符的长度</span><span class="sxs-lookup"><span data-stu-id="7e401-127">The passwords must be 16-64 characters in length</span></span> |
|<span data-ttu-id="7e401-128">提示</span><span class="sxs-lookup"><span data-stu-id="7e401-128">hint</span></span>|<span data-ttu-id="7e401-129">String</span><span class="sxs-lookup"><span data-stu-id="7e401-129">String</span></span>|  |

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
