---
title: parentalControlSettings 资源类型
description: 指定应用程序的家长控制设置。 这些设置控制同意体验。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: applications
author: sureshja
ms.openlocfilehash: 1f145ecabb4eccfe15eaedc856b1349fc6ce9f5a
ms.sourcegitcommit: 1004835b44271f2e50332a1bdc9097d4b06a914a
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 02/06/2021
ms.locfileid: "50128496"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="d9c11-104">parentalControlSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="d9c11-104">parentalControlSettings resource type</span></span>

<span data-ttu-id="d9c11-105">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d9c11-105">Namespace: microsoft.graph</span></span>

<span data-ttu-id="d9c11-106">指定应用程序的家长控制设置。</span><span class="sxs-lookup"><span data-stu-id="d9c11-106">Specifies parental control settings for an application.</span></span> <span data-ttu-id="d9c11-107">这些设置控制同意体验。</span><span class="sxs-lookup"><span data-stu-id="d9c11-107">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="d9c11-108">属性</span><span class="sxs-lookup"><span data-stu-id="d9c11-108">Properties</span></span>

| <span data-ttu-id="d9c11-109">属性</span><span class="sxs-lookup"><span data-stu-id="d9c11-109">Property</span></span> | <span data-ttu-id="d9c11-110">类型</span><span class="sxs-lookup"><span data-stu-id="d9c11-110">Type</span></span> | <span data-ttu-id="d9c11-111">说明</span><span class="sxs-lookup"><span data-stu-id="d9c11-111">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="d9c11-112">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="d9c11-112">countriesBlockedForMinors</span></span>|<span data-ttu-id="d9c11-113">String collection</span><span class="sxs-lookup"><span data-stu-id="d9c11-113">String collection</span></span>| <span data-ttu-id="d9c11-114">指定两 [个字母的 ISO 国家/地区代码](https://www.iso.org/iso-3166-country-codes.html)。</span><span class="sxs-lookup"><span data-stu-id="d9c11-114">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="d9c11-115">对于此列表中指定的国家/地区中的未成年人，将阻止其访问该应用程序。</span><span class="sxs-lookup"><span data-stu-id="d9c11-115">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="d9c11-116">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="d9c11-116">legalAgeGroupRule</span></span>| <span data-ttu-id="d9c11-117">String</span><span class="sxs-lookup"><span data-stu-id="d9c11-117">String</span></span> | <span data-ttu-id="d9c11-118">指定适用于应用用户的法律年龄组规则。</span><span class="sxs-lookup"><span data-stu-id="d9c11-118">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="d9c11-119">可以设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="d9c11-119">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="d9c11-120">值</span><span class="sxs-lookup"><span data-stu-id="d9c11-120">Value</span></span></th><th><span data-ttu-id="d9c11-121">说明</span><span class="sxs-lookup"><span data-stu-id="d9c11-121">Description</span></span></th></tr><tr><td><span data-ttu-id="d9c11-122">允许</span><span class="sxs-lookup"><span data-stu-id="d9c11-122">Allow</span></span></td><td><span data-ttu-id="d9c11-123">默认值。</span><span class="sxs-lookup"><span data-stu-id="d9c11-123">Default.</span></span> <span data-ttu-id="d9c11-124">强制执行法律最低要求。</span><span class="sxs-lookup"><span data-stu-id="d9c11-124">Enforces the legal minimum.</span></span> <span data-ttu-id="d9c11-125">这意味着欧盟和韩国的未成年人需要家长同意。</span><span class="sxs-lookup"><span data-stu-id="d9c11-125">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="d9c11-126">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="d9c11-126">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="d9c11-127">强制用户指定出生日期，以遵守 COPPA 规则。</span><span class="sxs-lookup"><span data-stu-id="d9c11-127">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="d9c11-128">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="d9c11-128">RequireConsentForMinors</span></span></td><td><span data-ttu-id="d9c11-129">需要 18 以下年龄的家长同意，无论国家/地区次要规则如何。</span><span class="sxs-lookup"><span data-stu-id="d9c11-129">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="d9c11-130">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="d9c11-130">RequireConsentForKids</span></span></td><td><span data-ttu-id="d9c11-131">需要 14 以下年龄的家长同意，无论国家/地区次要规则如何。</span><span class="sxs-lookup"><span data-stu-id="d9c11-131">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="d9c11-132">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="d9c11-132">BlockMinors</span></span></td><td><span data-ttu-id="d9c11-133">阻止未成年人使用应用。</span><span class="sxs-lookup"><span data-stu-id="d9c11-133">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="d9c11-134">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d9c11-134">JSON representation</span></span>
<span data-ttu-id="d9c11-135">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d9c11-135">Here is a JSON representation of the resource.</span></span>

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

