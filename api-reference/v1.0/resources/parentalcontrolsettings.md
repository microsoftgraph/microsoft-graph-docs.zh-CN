---
title: parentalControlSettings 资源类型
description: 指定应用程序的家长控制设置。 这些设置控制许可体验。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: davidmu1
ms.openlocfilehash: bec744a555cd7aa71d9dbf577f6006980501ac61
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42447232"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="e24c9-104">parentalControlSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="e24c9-104">parentalControlSettings resource type</span></span>

<span data-ttu-id="e24c9-105">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="e24c9-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="e24c9-106">指定应用程序的家长控制设置。</span><span class="sxs-lookup"><span data-stu-id="e24c9-106">Specifies parental control settings for an application.</span></span> <span data-ttu-id="e24c9-107">这些设置控制许可体验。</span><span class="sxs-lookup"><span data-stu-id="e24c9-107">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="e24c9-108">属性</span><span class="sxs-lookup"><span data-stu-id="e24c9-108">Properties</span></span>

| <span data-ttu-id="e24c9-109">属性</span><span class="sxs-lookup"><span data-stu-id="e24c9-109">Property</span></span> | <span data-ttu-id="e24c9-110">类型</span><span class="sxs-lookup"><span data-stu-id="e24c9-110">Type</span></span> | <span data-ttu-id="e24c9-111">说明</span><span class="sxs-lookup"><span data-stu-id="e24c9-111">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="e24c9-112">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="e24c9-112">countriesBlockedForMinors</span></span>|<span data-ttu-id="e24c9-113">String 集合</span><span class="sxs-lookup"><span data-stu-id="e24c9-113">String collection</span></span>| <span data-ttu-id="e24c9-114">指定[两个字母的 ISO 国家/地区代码](https://www.iso.org/iso-3166-country-codes.html)。</span><span class="sxs-lookup"><span data-stu-id="e24c9-114">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="e24c9-115">将阻止对此列表中指定国家/地区的未成年人访问应用程序。</span><span class="sxs-lookup"><span data-stu-id="e24c9-115">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="e24c9-116">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="e24c9-116">legalAgeGroupRule</span></span>| <span data-ttu-id="e24c9-117">String</span><span class="sxs-lookup"><span data-stu-id="e24c9-117">String</span></span> | <span data-ttu-id="e24c9-118">指定适用于应用程序用户的法律年龄组规则。</span><span class="sxs-lookup"><span data-stu-id="e24c9-118">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="e24c9-119">可以设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="e24c9-119">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="e24c9-120">值</span><span class="sxs-lookup"><span data-stu-id="e24c9-120">Value</span></span></th><th><span data-ttu-id="e24c9-121">说明</span><span class="sxs-lookup"><span data-stu-id="e24c9-121">Description</span></span></th></tr><tr><td><span data-ttu-id="e24c9-122">允许</span><span class="sxs-lookup"><span data-stu-id="e24c9-122">Allow</span></span></td><td><span data-ttu-id="e24c9-123">默认值。</span><span class="sxs-lookup"><span data-stu-id="e24c9-123">Default.</span></span> <span data-ttu-id="e24c9-124">强制实施合法的最小值。</span><span class="sxs-lookup"><span data-stu-id="e24c9-124">Enforces the legal minimum.</span></span> <span data-ttu-id="e24c9-125">这意味着欧盟和韩国的未成年人需要家长同意。</span><span class="sxs-lookup"><span data-stu-id="e24c9-125">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="e24c9-126">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="e24c9-126">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="e24c9-127">强制用户指定要符合 COPPA 规则的出生日期。</span><span class="sxs-lookup"><span data-stu-id="e24c9-127">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="e24c9-128">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="e24c9-128">RequireConsentForMinors</span></span></td><td><span data-ttu-id="e24c9-129">要求对低于18岁的家长同意，而不考虑国家/地区的次要规则。</span><span class="sxs-lookup"><span data-stu-id="e24c9-129">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="e24c9-130">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="e24c9-130">RequireConsentForKids</span></span></td><td><span data-ttu-id="e24c9-131">需要对低于14的年龄进行家长同意，而不考虑国家/地区的次要规则。</span><span class="sxs-lookup"><span data-stu-id="e24c9-131">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="e24c9-132">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="e24c9-132">BlockMinors</span></span></td><td><span data-ttu-id="e24c9-133">阻止未成年人使用应用。</span><span class="sxs-lookup"><span data-stu-id="e24c9-133">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="e24c9-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="e24c9-134">JSON representation</span></span>
<span data-ttu-id="e24c9-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="e24c9-135">Here is a JSON representation of the resource.</span></span>

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
