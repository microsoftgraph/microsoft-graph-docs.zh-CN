---
title: parentalControlSettings 资源类型
description: 指定应用程序的家长控制设置。 这些设置控制许可体验。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: 066182d0e591dc0a260313beafe75504b328a31b
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939002"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="911e5-104">parentalControlSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="911e5-104">parentalControlSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="911e5-105">指定应用程序的家长控制设置。</span><span class="sxs-lookup"><span data-stu-id="911e5-105">Specifies parental control settings for an application.</span></span> <span data-ttu-id="911e5-106">这些设置控制许可体验。</span><span class="sxs-lookup"><span data-stu-id="911e5-106">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="911e5-107">属性</span><span class="sxs-lookup"><span data-stu-id="911e5-107">Properties</span></span>

| <span data-ttu-id="911e5-108">属性</span><span class="sxs-lookup"><span data-stu-id="911e5-108">Property</span></span> | <span data-ttu-id="911e5-109">类型</span><span class="sxs-lookup"><span data-stu-id="911e5-109">Type</span></span> | <span data-ttu-id="911e5-110">描述</span><span class="sxs-lookup"><span data-stu-id="911e5-110">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="911e5-111">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="911e5-111">countriesBlockedForMinors</span></span>|<span data-ttu-id="911e5-112">String collection</span><span class="sxs-lookup"><span data-stu-id="911e5-112">String collection</span></span>| <span data-ttu-id="911e5-113">指定[两个字母的 ISO 国家/地区代码](https://www.iso.org/iso-3166-country-codes.html)。</span><span class="sxs-lookup"><span data-stu-id="911e5-113">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="911e5-114">将阻止对此列表中指定国家/地区的未成年人访问应用程序。</span><span class="sxs-lookup"><span data-stu-id="911e5-114">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="911e5-115">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="911e5-115">legalAgeGroupRule</span></span>| <span data-ttu-id="911e5-116">字符串</span><span class="sxs-lookup"><span data-stu-id="911e5-116">String</span></span> | <span data-ttu-id="911e5-117">指定适用于应用程序用户的法律年龄组规则。</span><span class="sxs-lookup"><span data-stu-id="911e5-117">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="911e5-118">可以设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="911e5-118">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="911e5-119">值</span><span class="sxs-lookup"><span data-stu-id="911e5-119">Value</span></span></th><th><span data-ttu-id="911e5-120">说明</span><span class="sxs-lookup"><span data-stu-id="911e5-120">Description</span></span></th></tr><tr><td><span data-ttu-id="911e5-121">允许</span><span class="sxs-lookup"><span data-stu-id="911e5-121">Allow</span></span></td><td><span data-ttu-id="911e5-122">默认值。</span><span class="sxs-lookup"><span data-stu-id="911e5-122">Default.</span></span> <span data-ttu-id="911e5-123">强制实施合法的最小值。</span><span class="sxs-lookup"><span data-stu-id="911e5-123">Enforces the legal minimum.</span></span> <span data-ttu-id="911e5-124">这意味着欧盟和韩国的未成年人需要家长同意。</span><span class="sxs-lookup"><span data-stu-id="911e5-124">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="911e5-125">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="911e5-125">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="911e5-126">强制用户指定要符合 COPPA 规则的出生日期。</span><span class="sxs-lookup"><span data-stu-id="911e5-126">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="911e5-127">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="911e5-127">RequireConsentForMinors</span></span></td><td><span data-ttu-id="911e5-128">要求对低于18岁的家长同意，而不考虑国家/地区的次要规则。</span><span class="sxs-lookup"><span data-stu-id="911e5-128">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="911e5-129">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="911e5-129">RequireConsentForKids</span></span></td><td><span data-ttu-id="911e5-130">需要对低于14的年龄进行家长同意，而不考虑国家/地区的次要规则。</span><span class="sxs-lookup"><span data-stu-id="911e5-130">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="911e5-131">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="911e5-131">BlockMinors</span></span></td><td><span data-ttu-id="911e5-132">阻止未成年人使用应用。</span><span class="sxs-lookup"><span data-stu-id="911e5-132">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="911e5-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="911e5-133">JSON representation</span></span>
<span data-ttu-id="911e5-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="911e5-134">Here is a JSON representation of the resource.</span></span>

<!--{
  "blockType": "resource",
  "@odata.type": "microsoft.graph.parentalControlSettings"
}-->
```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
