---
title: passwordCredential 资源类型
description: 包含与应用程序或服务主体密码凭据。 **PasswordCredentials**属性和应用程序实体的 servicePrincipal 实体是**passwordCredential**的集合。
localization_priority: Normal
ms.openlocfilehash: 5cb995c00a7dcfcfb4bda331e24dcb4d732f04f9
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27814439"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="ca5a1-104">passwordCredential 资源类型</span><span class="sxs-lookup"><span data-stu-id="ca5a1-104">passwordCredential resource type</span></span>

> <span data-ttu-id="ca5a1-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="ca5a1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="ca5a1-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="ca5a1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="ca5a1-107">包含与应用程序或服务主体密码凭据。</span><span class="sxs-lookup"><span data-stu-id="ca5a1-107">Contains a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="ca5a1-108">**PasswordCredentials**属性和[应用程序](application.md)实体的[servicePrincipal](serviceprincipal.md)实体是**passwordCredential**的集合。</span><span class="sxs-lookup"><span data-stu-id="ca5a1-108">The **passwordCredentials** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **passwordCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ca5a1-109">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ca5a1-109">JSON representation</span></span>

<span data-ttu-id="ca5a1-110">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ca5a1-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="ca5a1-111">属性</span><span class="sxs-lookup"><span data-stu-id="ca5a1-111">Properties</span></span>
| <span data-ttu-id="ca5a1-112">属性</span><span class="sxs-lookup"><span data-stu-id="ca5a1-112">Property</span></span>     | <span data-ttu-id="ca5a1-113">类型</span><span class="sxs-lookup"><span data-stu-id="ca5a1-113">Type</span></span>   |<span data-ttu-id="ca5a1-114">Description</span><span class="sxs-lookup"><span data-stu-id="ca5a1-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ca5a1-115">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="ca5a1-115">customKeyIdentifier</span></span>|<span data-ttu-id="ca5a1-116">Binary</span><span class="sxs-lookup"><span data-stu-id="ca5a1-116">Binary</span></span>|            |
|<span data-ttu-id="ca5a1-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ca5a1-117">endDateTime</span></span>|<span data-ttu-id="ca5a1-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca5a1-118">DateTimeOffset</span></span>|<span data-ttu-id="ca5a1-119">过期日期和时间的密码。时间戳类型表示使用 ISO 8601 格式的日期和时间信息且始终在 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="ca5a1-119">The date and time at which the password expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ca5a1-120">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ca5a1-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ca5a1-121">密钥 id 为</span><span class="sxs-lookup"><span data-stu-id="ca5a1-121">keyId</span></span>|<span data-ttu-id="ca5a1-122">Guid</span><span class="sxs-lookup"><span data-stu-id="ca5a1-122">Guid</span></span>|            |
|<span data-ttu-id="ca5a1-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ca5a1-123">startDateTime</span></span>|<span data-ttu-id="ca5a1-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ca5a1-124">DateTimeOffset</span></span>|<span data-ttu-id="ca5a1-125">日期和时间的密码将成为有效。时间戳类型表示使用 ISO 8601 格式的日期和时间信息且始终在 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="ca5a1-125">The date and time at which the password becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ca5a1-126">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ca5a1-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ca5a1-127">secretText</span><span class="sxs-lookup"><span data-stu-id="ca5a1-127">secretText</span></span>|<span data-ttu-id="ca5a1-128">字符串</span><span class="sxs-lookup"><span data-stu-id="ca5a1-128">String</span></span>| <span data-ttu-id="ca5a1-129">密码必须为 16-64 个字符的长度</span><span class="sxs-lookup"><span data-stu-id="ca5a1-129">The passwords must be 16-64 characters in length</span></span> |
|<span data-ttu-id="ca5a1-130">提示</span><span class="sxs-lookup"><span data-stu-id="ca5a1-130">hint</span></span>|<span data-ttu-id="ca5a1-131">String</span><span class="sxs-lookup"><span data-stu-id="ca5a1-131">String</span></span>|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
