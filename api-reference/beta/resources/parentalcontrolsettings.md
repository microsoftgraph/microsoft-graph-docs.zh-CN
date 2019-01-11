---
title: parentalControlSettings 资源类型
description: 指定应用程序的家长的控制设置。 这些设置控制的同意体验。
localization_priority: Normal
ms.openlocfilehash: bb6f776d5f206fb0ed35a999effc7bbdc0768512
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27806515"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="d90c0-104">parentalControlSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d90c0-104">parentalControlSettings resource type</span></span>

> <span data-ttu-id="d90c0-105">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="d90c0-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="d90c0-106">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="d90c0-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="d90c0-107">指定应用程序的家长的控制设置。</span><span class="sxs-lookup"><span data-stu-id="d90c0-107">Specifies parental control settings for an application.</span></span> <span data-ttu-id="d90c0-108">这些设置控制的同意体验。</span><span class="sxs-lookup"><span data-stu-id="d90c0-108">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="d90c0-109">属性</span><span class="sxs-lookup"><span data-stu-id="d90c0-109">Properties</span></span>

| <span data-ttu-id="d90c0-110">属性</span><span class="sxs-lookup"><span data-stu-id="d90c0-110">Property</span></span> | <span data-ttu-id="d90c0-111">类型</span><span class="sxs-lookup"><span data-stu-id="d90c0-111">Type</span></span> | <span data-ttu-id="d90c0-112">Description</span><span class="sxs-lookup"><span data-stu-id="d90c0-112">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="d90c0-113">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="d90c0-113">countriesBlockedForMinors</span></span>|<span data-ttu-id="d90c0-114">String 集合</span><span class="sxs-lookup"><span data-stu-id="d90c0-114">String collection</span></span>| <span data-ttu-id="d90c0-115">指定[两个字母的 ISO 国家/地区代码](https://www.iso.org/iso-3166-country-codes.html)。</span><span class="sxs-lookup"><span data-stu-id="d90c0-115">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="d90c0-116">将此列表中指定的国家/地区从未成年人阻止访问应用程序。</span><span class="sxs-lookup"><span data-stu-id="d90c0-116">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="d90c0-117">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="d90c0-117">legalAgeGroupRule</span></span>| <span data-ttu-id="d90c0-118">字符串</span><span class="sxs-lookup"><span data-stu-id="d90c0-118">String</span></span> | <span data-ttu-id="d90c0-119">指定应用于用户的应用程序的法律期限组规则。</span><span class="sxs-lookup"><span data-stu-id="d90c0-119">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="d90c0-120">可以设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="d90c0-120">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="d90c0-121">值</span><span class="sxs-lookup"><span data-stu-id="d90c0-121">Value</span></span></th><th><span data-ttu-id="d90c0-122">Description</span><span class="sxs-lookup"><span data-stu-id="d90c0-122">Description</span></span></th></tr><tr><td><span data-ttu-id="d90c0-123">允许</span><span class="sxs-lookup"><span data-stu-id="d90c0-123">Allow</span></span></td><td><span data-ttu-id="d90c0-124">默认值。</span><span class="sxs-lookup"><span data-stu-id="d90c0-124">Default.</span></span> <span data-ttu-id="d90c0-125">强制执行法律最小值。</span><span class="sxs-lookup"><span data-stu-id="d90c0-125">Enforces the legal minimum.</span></span> <span data-ttu-id="d90c0-126">这意味着家长同意，则需要进行评级欧盟和韩国中。</span><span class="sxs-lookup"><span data-stu-id="d90c0-126">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="d90c0-127">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="d90c0-127">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="d90c0-128">强制执行用户指定出生日期遵守 COPPA 规则。</span><span class="sxs-lookup"><span data-stu-id="d90c0-128">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="d90c0-129">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="d90c0-129">RequireConsentForMinors</span></span></td><td><span data-ttu-id="d90c0-130">需要为 18，无论国家/地区次要规则下方岁家长同意。</span><span class="sxs-lookup"><span data-stu-id="d90c0-130">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="d90c0-131">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="d90c0-131">RequireConsentForKids</span></span></td><td><span data-ttu-id="d90c0-132">需要为 14，无论国家/地区次要规则下方岁家长同意。</span><span class="sxs-lookup"><span data-stu-id="d90c0-132">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="d90c0-133">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="d90c0-133">BlockMinors</span></span></td><td><span data-ttu-id="d90c0-134">使用应用程序的块未成年人。</span><span class="sxs-lookup"><span data-stu-id="d90c0-134">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="d90c0-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d90c0-135">JSON representation</span></span>
<span data-ttu-id="d90c0-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d90c0-136">Here is a JSON representation of the resource.</span></span>

```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
