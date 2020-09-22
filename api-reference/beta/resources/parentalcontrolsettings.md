---
title: parentalControlSettings 资源类型
description: 指定应用程序的家长控制设置。 这些设置控制许可体验。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: ee1b9d7f41e51f7dfaacfde6aac967cf49461cc2
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "47998262"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="01fe1-104">parentalControlSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="01fe1-104">parentalControlSettings resource type</span></span>

<span data-ttu-id="01fe1-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="01fe1-105">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="01fe1-106">指定应用程序的家长控制设置。</span><span class="sxs-lookup"><span data-stu-id="01fe1-106">Specifies parental control settings for an application.</span></span> <span data-ttu-id="01fe1-107">这些设置控制许可体验。</span><span class="sxs-lookup"><span data-stu-id="01fe1-107">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="01fe1-108">属性</span><span class="sxs-lookup"><span data-stu-id="01fe1-108">Properties</span></span>

| <span data-ttu-id="01fe1-109">属性</span><span class="sxs-lookup"><span data-stu-id="01fe1-109">Property</span></span> | <span data-ttu-id="01fe1-110">类型</span><span class="sxs-lookup"><span data-stu-id="01fe1-110">Type</span></span> | <span data-ttu-id="01fe1-111">说明</span><span class="sxs-lookup"><span data-stu-id="01fe1-111">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="01fe1-112">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="01fe1-112">countriesBlockedForMinors</span></span>|<span data-ttu-id="01fe1-113">String collection</span><span class="sxs-lookup"><span data-stu-id="01fe1-113">String collection</span></span>| <span data-ttu-id="01fe1-114">指定 [两个字母的 ISO 国家/地区代码](https://www.iso.org/iso-3166-country-codes.html)。</span><span class="sxs-lookup"><span data-stu-id="01fe1-114">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="01fe1-115">将阻止对此列表中指定国家/地区的未成年人访问应用程序。</span><span class="sxs-lookup"><span data-stu-id="01fe1-115">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="01fe1-116">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="01fe1-116">legalAgeGroupRule</span></span>| <span data-ttu-id="01fe1-117">String</span><span class="sxs-lookup"><span data-stu-id="01fe1-117">String</span></span> | <span data-ttu-id="01fe1-118">指定适用于应用程序用户的法律年龄组规则。</span><span class="sxs-lookup"><span data-stu-id="01fe1-118">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="01fe1-119">可以设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="01fe1-119">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="01fe1-120">值</span><span class="sxs-lookup"><span data-stu-id="01fe1-120">Value</span></span></th><th><span data-ttu-id="01fe1-121">说明</span><span class="sxs-lookup"><span data-stu-id="01fe1-121">Description</span></span></th></tr><tr><td><span data-ttu-id="01fe1-122">允许</span><span class="sxs-lookup"><span data-stu-id="01fe1-122">Allow</span></span></td><td><span data-ttu-id="01fe1-123">默认值。</span><span class="sxs-lookup"><span data-stu-id="01fe1-123">Default.</span></span> <span data-ttu-id="01fe1-124">强制实施合法的最小值。</span><span class="sxs-lookup"><span data-stu-id="01fe1-124">Enforces the legal minimum.</span></span> <span data-ttu-id="01fe1-125">这意味着欧盟和韩国的未成年人需要家长同意。</span><span class="sxs-lookup"><span data-stu-id="01fe1-125">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="01fe1-126">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="01fe1-126">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="01fe1-127">强制用户指定要符合 COPPA 规则的出生日期。</span><span class="sxs-lookup"><span data-stu-id="01fe1-127">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="01fe1-128">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="01fe1-128">RequireConsentForMinors</span></span></td><td><span data-ttu-id="01fe1-129">要求对低于18岁的家长同意，而不考虑国家/地区的次要规则。</span><span class="sxs-lookup"><span data-stu-id="01fe1-129">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="01fe1-130">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="01fe1-130">RequireConsentForKids</span></span></td><td><span data-ttu-id="01fe1-131">需要对低于14的年龄进行家长同意，而不考虑国家/地区的次要规则。</span><span class="sxs-lookup"><span data-stu-id="01fe1-131">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="01fe1-132">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="01fe1-132">BlockMinors</span></span></td><td><span data-ttu-id="01fe1-133">阻止未成年人使用应用。</span><span class="sxs-lookup"><span data-stu-id="01fe1-133">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="01fe1-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="01fe1-134">JSON representation</span></span>
<span data-ttu-id="01fe1-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="01fe1-135">Here is a JSON representation of the resource.</span></span>

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


