---
title: parentalControlSettings 资源类型
description: 指定应用程序的家长控制设置。 这些设置控制许可体验。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: microsoft-identity-platform
author: sureshja
ms.openlocfilehash: a65c2734cdb82ba249fe1cc3fa0f11e1c4d27fc0
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48094188"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="8cce8-104">parentalControlSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="8cce8-104">parentalControlSettings resource type</span></span>

<span data-ttu-id="8cce8-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="8cce8-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="8cce8-106">指定应用程序的家长控制设置。</span><span class="sxs-lookup"><span data-stu-id="8cce8-106">Specifies parental control settings for an application.</span></span> <span data-ttu-id="8cce8-107">这些设置控制许可体验。</span><span class="sxs-lookup"><span data-stu-id="8cce8-107">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="8cce8-108">属性</span><span class="sxs-lookup"><span data-stu-id="8cce8-108">Properties</span></span>

| <span data-ttu-id="8cce8-109">属性</span><span class="sxs-lookup"><span data-stu-id="8cce8-109">Property</span></span> | <span data-ttu-id="8cce8-110">类型</span><span class="sxs-lookup"><span data-stu-id="8cce8-110">Type</span></span> | <span data-ttu-id="8cce8-111">说明</span><span class="sxs-lookup"><span data-stu-id="8cce8-111">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="8cce8-112">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="8cce8-112">countriesBlockedForMinors</span></span>|<span data-ttu-id="8cce8-113">String collection</span><span class="sxs-lookup"><span data-stu-id="8cce8-113">String collection</span></span>| <span data-ttu-id="8cce8-114">指定 [两个字母的 ISO 国家/地区代码](https://www.iso.org/iso-3166-country-codes.html)。</span><span class="sxs-lookup"><span data-stu-id="8cce8-114">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="8cce8-115">将阻止对此列表中指定国家/地区的未成年人访问应用程序。</span><span class="sxs-lookup"><span data-stu-id="8cce8-115">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="8cce8-116">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="8cce8-116">legalAgeGroupRule</span></span>| <span data-ttu-id="8cce8-117">String</span><span class="sxs-lookup"><span data-stu-id="8cce8-117">String</span></span> | <span data-ttu-id="8cce8-118">指定适用于应用程序用户的法律年龄组规则。</span><span class="sxs-lookup"><span data-stu-id="8cce8-118">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="8cce8-119">可以设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="8cce8-119">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="8cce8-120">值</span><span class="sxs-lookup"><span data-stu-id="8cce8-120">Value</span></span></th><th><span data-ttu-id="8cce8-121">说明</span><span class="sxs-lookup"><span data-stu-id="8cce8-121">Description</span></span></th></tr><tr><td><span data-ttu-id="8cce8-122">允许</span><span class="sxs-lookup"><span data-stu-id="8cce8-122">Allow</span></span></td><td><span data-ttu-id="8cce8-123">默认值。</span><span class="sxs-lookup"><span data-stu-id="8cce8-123">Default.</span></span> <span data-ttu-id="8cce8-124">强制实施合法的最小值。</span><span class="sxs-lookup"><span data-stu-id="8cce8-124">Enforces the legal minimum.</span></span> <span data-ttu-id="8cce8-125">这意味着欧盟和韩国的未成年人需要家长同意。</span><span class="sxs-lookup"><span data-stu-id="8cce8-125">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="8cce8-126">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="8cce8-126">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="8cce8-127">强制用户指定要符合 COPPA 规则的出生日期。</span><span class="sxs-lookup"><span data-stu-id="8cce8-127">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="8cce8-128">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="8cce8-128">RequireConsentForMinors</span></span></td><td><span data-ttu-id="8cce8-129">要求对低于18岁的家长同意，而不考虑国家/地区的次要规则。</span><span class="sxs-lookup"><span data-stu-id="8cce8-129">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="8cce8-130">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="8cce8-130">RequireConsentForKids</span></span></td><td><span data-ttu-id="8cce8-131">需要对低于14的年龄进行家长同意，而不考虑国家/地区的次要规则。</span><span class="sxs-lookup"><span data-stu-id="8cce8-131">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="8cce8-132">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="8cce8-132">BlockMinors</span></span></td><td><span data-ttu-id="8cce8-133">阻止未成年人使用应用。</span><span class="sxs-lookup"><span data-stu-id="8cce8-133">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="8cce8-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="8cce8-134">JSON representation</span></span>
<span data-ttu-id="8cce8-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="8cce8-135">Here is a JSON representation of the resource.</span></span>

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

