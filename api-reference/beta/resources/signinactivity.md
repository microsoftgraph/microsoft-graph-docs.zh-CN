---
title: signInActivity 资源类型
description: 为特定用户提供上次登录日期。
localization_priority: Normal
author: besiler
ms.prod: identity-and-access-reports
doc_type: resourcePageType
ms.openlocfilehash: 7d57324b7953b865b98c01d6b16236dea54e73a5
ms.sourcegitcommit: 9d98d9e9cc1e193850ab9b82aaaf906d70e1378b
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/12/2021
ms.locfileid: "50761056"
---
# <a name="signinactivity-resource-type"></a><span data-ttu-id="f9a3b-103">signInActivity 资源类型</span><span class="sxs-lookup"><span data-stu-id="f9a3b-103">signInActivity resource type</span></span>

<span data-ttu-id="f9a3b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="f9a3b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f9a3b-105">为特定用户提供上次登录 [日期](user.md)。</span><span class="sxs-lookup"><span data-stu-id="f9a3b-105">Provides the last signed-in date for a specific [user](user.md).</span></span>

## <a name="properties"></a><span data-ttu-id="f9a3b-106">属性</span><span class="sxs-lookup"><span data-stu-id="f9a3b-106">Properties</span></span>

| <span data-ttu-id="f9a3b-107">属性</span><span class="sxs-lookup"><span data-stu-id="f9a3b-107">Property</span></span>     | <span data-ttu-id="f9a3b-108">类型</span><span class="sxs-lookup"><span data-stu-id="f9a3b-108">Type</span></span>        | <span data-ttu-id="f9a3b-109">说明</span><span class="sxs-lookup"><span data-stu-id="f9a3b-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="f9a3b-110">lastSignInDateTime</span><span class="sxs-lookup"><span data-stu-id="f9a3b-110">lastSignInDateTime</span></span>|<span data-ttu-id="f9a3b-111">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f9a3b-111">DateTimeOffset</span></span>|<span data-ttu-id="f9a3b-112">特定用户的上次交互式登录日期。</span><span class="sxs-lookup"><span data-stu-id="f9a3b-112">The last interactive sign-in date for a specific user.</span></span> <span data-ttu-id="f9a3b-113">可以使用此字段计算用户最后一次使用交互式身份验证方法登录到目录的时间。</span><span class="sxs-lookup"><span data-stu-id="f9a3b-113">You can use this field to calculate the last time a user signed in to the directory with an interactive authentication method.</span></span> <span data-ttu-id="f9a3b-114">此字段可用于生成报告，例如非活动用户。</span><span class="sxs-lookup"><span data-stu-id="f9a3b-114">This field can be used to build reports, such as inactive users.</span></span> <span data-ttu-id="f9a3b-115">时间戳表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="f9a3b-115">The timestamp represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f9a3b-116">例如，2014 年 1 月 1 日午夜 UTC 为 `'2014-01-01T00:00:00Z'` ：。</span><span class="sxs-lookup"><span data-stu-id="f9a3b-116">For example, midnight UTC on Jan 1, 2014 is: `'2014-01-01T00:00:00Z'`.</span></span> <span data-ttu-id="f9a3b-117">有关使用此属性的值的信息，请参阅在 [Azure AD](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts)中管理非活动用户帐户。</span><span class="sxs-lookup"><span data-stu-id="f9a3b-117">For more information about using the value of this property, see [Manage inactive user accounts in Azure AD](/azure/active-directory/reports-monitoring/howto-manage-inactive-user-accounts).</span></span>|
|<span data-ttu-id="f9a3b-118">lastSignInRequestId</span><span class="sxs-lookup"><span data-stu-id="f9a3b-118">lastSignInRequestId</span></span>|<span data-ttu-id="f9a3b-119">String</span><span class="sxs-lookup"><span data-stu-id="f9a3b-119">String</span></span>|<span data-ttu-id="f9a3b-120">此用户执行的最后一次登录的请求 ID。</span><span class="sxs-lookup"><span data-stu-id="f9a3b-120">Request ID of the last sign-in performed by this user.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f9a3b-121">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="f9a3b-121">JSON representation</span></span>

<span data-ttu-id="f9a3b-122">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="f9a3b-122">The following is a JSON representation of the resource.</span></span>

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
