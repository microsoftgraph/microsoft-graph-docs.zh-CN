---
title: signInActivity 资源类型
description: 提供特定用户的上次登录日期。
localization_priority: Normal
author: khotz
ms.prod: microsoft-identity-platform
doc_type: resourcePageType
ms.openlocfilehash: 295b9c797da1c941dd09e5cd17b85bcc6d4a663d
ms.sourcegitcommit: 7ceec757fd82ef3fd80aa3089ef46d3807aa3aa2
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 10/09/2020
ms.locfileid: "48404369"
---
# <a name="signinactivity-resource-type"></a><span data-ttu-id="3ffd4-103">signInActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="3ffd4-103">signInActivity resource type</span></span>

<span data-ttu-id="3ffd4-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="3ffd4-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="3ffd4-105">提供特定 [用户](user.md)的上次登录日期。</span><span class="sxs-lookup"><span data-stu-id="3ffd4-105">Provides the last signed-in date for a specific [user](user.md).</span></span>

## <a name="properties"></a><span data-ttu-id="3ffd4-106">属性</span><span class="sxs-lookup"><span data-stu-id="3ffd4-106">Properties</span></span>

| <span data-ttu-id="3ffd4-107">属性</span><span class="sxs-lookup"><span data-stu-id="3ffd4-107">Property</span></span>     | <span data-ttu-id="3ffd4-108">类型</span><span class="sxs-lookup"><span data-stu-id="3ffd4-108">Type</span></span>        | <span data-ttu-id="3ffd4-109">说明</span><span class="sxs-lookup"><span data-stu-id="3ffd4-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="3ffd4-110">lastSignInDateTime</span><span class="sxs-lookup"><span data-stu-id="3ffd4-110">lastSignInDateTime</span></span>|<span data-ttu-id="3ffd4-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="3ffd4-111">DateTimeOffset</span></span>|<span data-ttu-id="3ffd4-112">特定用户的上次登录日期。</span><span class="sxs-lookup"><span data-stu-id="3ffd4-112">The last sign-in date for a specific user.</span></span> <span data-ttu-id="3ffd4-113">您可以使用此字段来计算用户上次登录目录的时间。</span><span class="sxs-lookup"><span data-stu-id="3ffd4-113">You can use this field to calculate the last time a user signed in to the directory.</span></span> <span data-ttu-id="3ffd4-114">此字段可用于生成报表，如非活动用户。</span><span class="sxs-lookup"><span data-stu-id="3ffd4-114">This field can be used to build reports, such as inactive users.</span></span> <span data-ttu-id="3ffd4-115">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="3ffd4-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="3ffd4-116">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`。</span><span class="sxs-lookup"><span data-stu-id="3ffd4-116">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="3ffd4-117">若要详细了解如何使用此属性的值，请参阅 [管理 AZURE AD 中的非活动用户帐户](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts)。</span><span class="sxs-lookup"><span data-stu-id="3ffd4-117">For more information about using the value of this property, see [Manage inactive user accounts in Azure AD](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts).</span></span>|
|<span data-ttu-id="3ffd4-118">lastSignInRequestId</span><span class="sxs-lookup"><span data-stu-id="3ffd4-118">lastSignInRequestId</span></span>|<span data-ttu-id="3ffd4-119">字符串</span><span class="sxs-lookup"><span data-stu-id="3ffd4-119">String</span></span>|<span data-ttu-id="3ffd4-120">此用户执行的最后一个登录的请求 ID。</span><span class="sxs-lookup"><span data-stu-id="3ffd4-120">Request ID of the last sign-in performed by this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="3ffd4-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="3ffd4-121">JSON representation</span></span>

<span data-ttu-id="3ffd4-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="3ffd4-122">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.signInActivity",
  "baseType": null
}-->

```json
{
  "lastSignInDateTime": "String (timestamp)",
  "lastSignInRequestId": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "signInActivity resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->