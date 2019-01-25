---
title: parentalControlSettings 资源类型
description: 指定应用程序的家长的控制设置。 这些设置控制的同意体验。
localization_priority: Normal
ms.openlocfilehash: 52a808cd4c3e6f29e4d43c7c4ea5c9e30a81447b
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/24/2019
ms.locfileid: "29528401"
---
# <a name="parentalcontrolsettings-resource-type"></a><span data-ttu-id="45180-104">parentalControlSettings 资源类型</span><span class="sxs-lookup"><span data-stu-id="45180-104">parentalControlSettings resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="45180-105">指定应用程序的家长的控制设置。</span><span class="sxs-lookup"><span data-stu-id="45180-105">Specifies parental control settings for an application.</span></span> <span data-ttu-id="45180-106">这些设置控制的同意体验。</span><span class="sxs-lookup"><span data-stu-id="45180-106">These settings control the consent experience.</span></span>

## <a name="properties"></a><span data-ttu-id="45180-107">属性</span><span class="sxs-lookup"><span data-stu-id="45180-107">Properties</span></span>

| <span data-ttu-id="45180-108">属性</span><span class="sxs-lookup"><span data-stu-id="45180-108">Property</span></span> | <span data-ttu-id="45180-109">类型</span><span class="sxs-lookup"><span data-stu-id="45180-109">Type</span></span> | <span data-ttu-id="45180-110">描述</span><span class="sxs-lookup"><span data-stu-id="45180-110">Description</span></span> |
:---------------|:--------|:----------|
|<span data-ttu-id="45180-111">countriesBlockedForMinors</span><span class="sxs-lookup"><span data-stu-id="45180-111">countriesBlockedForMinors</span></span>|<span data-ttu-id="45180-112">String 集合</span><span class="sxs-lookup"><span data-stu-id="45180-112">String collection</span></span>| <span data-ttu-id="45180-113">指定[两个字母的 ISO 国家/地区代码](https://www.iso.org/iso-3166-country-codes.html)。</span><span class="sxs-lookup"><span data-stu-id="45180-113">Specifies the [two-letter ISO country codes](https://www.iso.org/iso-3166-country-codes.html).</span></span> <span data-ttu-id="45180-114">将此列表中指定的国家/地区从未成年人阻止访问应用程序。</span><span class="sxs-lookup"><span data-stu-id="45180-114">Access to the application will be blocked for minors from the countries specified in this list.</span></span>|
|<span data-ttu-id="45180-115">legalAgeGroupRule</span><span class="sxs-lookup"><span data-stu-id="45180-115">legalAgeGroupRule</span></span>| <span data-ttu-id="45180-116">String</span><span class="sxs-lookup"><span data-stu-id="45180-116">String</span></span> | <span data-ttu-id="45180-117">指定应用于用户的应用程序的法律期限组规则。</span><span class="sxs-lookup"><span data-stu-id="45180-117">Specifies the legal age group rule that applies to users of the app.</span></span> <span data-ttu-id="45180-118">可以设置为下列值之一：</span><span class="sxs-lookup"><span data-stu-id="45180-118">Can be set to one of the following values:</span></span> <table><tr><th><span data-ttu-id="45180-119">值</span><span class="sxs-lookup"><span data-stu-id="45180-119">Value</span></span></th><th><span data-ttu-id="45180-120">说明</span><span class="sxs-lookup"><span data-stu-id="45180-120">Description</span></span></th></tr><tr><td><span data-ttu-id="45180-121">允许</span><span class="sxs-lookup"><span data-stu-id="45180-121">Allow</span></span></td><td><span data-ttu-id="45180-122">默认值。</span><span class="sxs-lookup"><span data-stu-id="45180-122">Default.</span></span> <span data-ttu-id="45180-123">强制执行法律最小值。</span><span class="sxs-lookup"><span data-stu-id="45180-123">Enforces the legal minimum.</span></span> <span data-ttu-id="45180-124">这意味着家长同意，则需要进行评级欧盟和韩国中。</span><span class="sxs-lookup"><span data-stu-id="45180-124">This means parental consent is required for minors in the European Union and Korea.</span></span></td></tr><tr><td><span data-ttu-id="45180-125">RequireConsentForPrivacyServices</span><span class="sxs-lookup"><span data-stu-id="45180-125">RequireConsentForPrivacyServices</span></span></td><td><span data-ttu-id="45180-126">强制执行用户指定出生日期遵守 COPPA 规则。</span><span class="sxs-lookup"><span data-stu-id="45180-126">Enforces the user to specify date of birth to comply with COPPA rules.</span></span> </td></tr><tr><td><span data-ttu-id="45180-127">RequireConsentForMinors</span><span class="sxs-lookup"><span data-stu-id="45180-127">RequireConsentForMinors</span></span></td><td><span data-ttu-id="45180-128">需要为 18，无论国家/地区次要规则下方岁家长同意。</span><span class="sxs-lookup"><span data-stu-id="45180-128">Requires parental consent for ages below 18, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="45180-129">RequireConsentForKids</span><span class="sxs-lookup"><span data-stu-id="45180-129">RequireConsentForKids</span></span></td><td><span data-ttu-id="45180-130">需要为 14，无论国家/地区次要规则下方岁家长同意。</span><span class="sxs-lookup"><span data-stu-id="45180-130">Requires parental consent for ages below 14, regardless of country minor rules.</span></span></td></tr><tr><td><span data-ttu-id="45180-131">BlockMinors</span><span class="sxs-lookup"><span data-stu-id="45180-131">BlockMinors</span></span></td><td><span data-ttu-id="45180-132">使用应用程序的块未成年人。</span><span class="sxs-lookup"><span data-stu-id="45180-132">Blocks minors from using the app.</span></span></td></tr></table> |

## <a name="json-representation"></a><span data-ttu-id="45180-133">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="45180-133">JSON representation</span></span>
<span data-ttu-id="45180-134">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="45180-134">Here is a JSON representation of the resource.</span></span>

```json
{
  "countriesBlockedForMinors": [ "String" ],
  "legalAgeGroupRule": "String"
}

```
<!--
{
  "type": "#page.annotation",
  "suppressions": [
    "Error: /api-reference/beta/resources/parentalcontrolsettings.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
