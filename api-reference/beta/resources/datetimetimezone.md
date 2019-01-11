---
title: dateTimeTimeZone 资源类型
description: 介绍某个时间点的日期、时间和时区。
localization_priority: Normal
ms.openlocfilehash: 5090edce8d86ff12470cc1bb39f92ef13b42ba15
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27876067"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="89027-103">dateTimeTimeZone 资源类型</span><span class="sxs-lookup"><span data-stu-id="89027-103">dateTimeTimeZone resource type</span></span>

> <span data-ttu-id="89027-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="89027-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="89027-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="89027-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="89027-106">介绍某个时间点的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="89027-106">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="89027-107">属性</span><span class="sxs-lookup"><span data-stu-id="89027-107">Properties</span></span>
| <span data-ttu-id="89027-108">属性</span><span class="sxs-lookup"><span data-stu-id="89027-108">Property</span></span>     | <span data-ttu-id="89027-109">类型</span><span class="sxs-lookup"><span data-stu-id="89027-109">Type</span></span>   |<span data-ttu-id="89027-110">说明</span><span class="sxs-lookup"><span data-stu-id="89027-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="89027-111">DateTime</span><span class="sxs-lookup"><span data-stu-id="89027-111">DateTime</span></span>|<span data-ttu-id="89027-112">String</span><span class="sxs-lookup"><span data-stu-id="89027-112">String</span></span>|<span data-ttu-id="89027-113">日期和时间组合表示形式的单个时间点 (`<date>T<time>`)。</span><span class="sxs-lookup"><span data-stu-id="89027-113">A single point of time in a combined date and time representation (`<date>T<time>`).</span></span>|
|<span data-ttu-id="89027-114">TimeZone</span><span class="sxs-lookup"><span data-stu-id="89027-114">TimeZone</span></span>|<span data-ttu-id="89027-115">String</span><span class="sxs-lookup"><span data-stu-id="89027-115">String</span></span>|<span data-ttu-id="89027-116">以下时区名称之一。</span><span class="sxs-lookup"><span data-stu-id="89027-116">One of the following time zone names.</span></span>|

<span data-ttu-id="89027-117">_TimeZone_ 属性可以设置为 Windows 支持的任意时区，以及以下时区名称。</span><span class="sxs-lookup"><span data-stu-id="89027-117">The _TimeZone_ property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="89027-118">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="89027-118">Etc/GMT+12</span></span>

<span data-ttu-id="89027-119">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="89027-119">Etc/GMT+11</span></span>

<span data-ttu-id="89027-120">太平洋/火奴鲁鲁</span><span class="sxs-lookup"><span data-stu-id="89027-120">Pacific/Honolulu</span></span>

<span data-ttu-id="89027-121">美洲/安克雷奇</span><span class="sxs-lookup"><span data-stu-id="89027-121">America/Anchorage</span></span>

<span data-ttu-id="89027-122">美洲/圣伊莎贝尔</span><span class="sxs-lookup"><span data-stu-id="89027-122">America/Santa_Isabel</span></span>

<span data-ttu-id="89027-123">美洲/洛杉矶</span><span class="sxs-lookup"><span data-stu-id="89027-123">America/Los_Angeles</span></span>

<span data-ttu-id="89027-124">美洲/菲尼克斯</span><span class="sxs-lookup"><span data-stu-id="89027-124">America/Phoenix</span></span>

<span data-ttu-id="89027-125">美洲/奇瓦瓦</span><span class="sxs-lookup"><span data-stu-id="89027-125">America/Chihuahua</span></span>

<span data-ttu-id="89027-126">美洲/丹佛</span><span class="sxs-lookup"><span data-stu-id="89027-126">America/Denver</span></span>

<span data-ttu-id="89027-127">美洲/危地马拉</span><span class="sxs-lookup"><span data-stu-id="89027-127">America/Guatemala</span></span>

<span data-ttu-id="89027-128">美洲/芝加哥</span><span class="sxs-lookup"><span data-stu-id="89027-128">America/Chicago</span></span>

<span data-ttu-id="89027-129">美洲/墨西哥城</span><span class="sxs-lookup"><span data-stu-id="89027-129">America/Mexico_City</span></span>

<span data-ttu-id="89027-130">美洲/里贾纳</span><span class="sxs-lookup"><span data-stu-id="89027-130">America/Regina</span></span>

<span data-ttu-id="89027-131">美洲/波哥大</span><span class="sxs-lookup"><span data-stu-id="89027-131">America/Bogota</span></span>

<span data-ttu-id="89027-132">美洲/纽约</span><span class="sxs-lookup"><span data-stu-id="89027-132">America/New_York</span></span>

<span data-ttu-id="89027-133">美洲/印第安纳/印第安纳波利斯</span><span class="sxs-lookup"><span data-stu-id="89027-133">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="89027-134">美洲/加拉加斯</span><span class="sxs-lookup"><span data-stu-id="89027-134">America/Caracas</span></span>

<span data-ttu-id="89027-135">美洲/亚松森</span><span class="sxs-lookup"><span data-stu-id="89027-135">America/Asuncion</span></span>

<span data-ttu-id="89027-136">美洲/哈利法克斯</span><span class="sxs-lookup"><span data-stu-id="89027-136">America/Halifax</span></span>

<span data-ttu-id="89027-137">美洲/库亚巴</span><span class="sxs-lookup"><span data-stu-id="89027-137">America/Cuiaba</span></span>

<span data-ttu-id="89027-138">美洲/拉巴斯</span><span class="sxs-lookup"><span data-stu-id="89027-138">America/La_Paz</span></span>

<span data-ttu-id="89027-139">美洲/圣地亚哥</span><span class="sxs-lookup"><span data-stu-id="89027-139">America/Santiago</span></span>

<span data-ttu-id="89027-140">美洲/圣约翰斯</span><span class="sxs-lookup"><span data-stu-id="89027-140">America/St_Johns</span></span>

<span data-ttu-id="89027-141">美洲/圣保罗</span><span class="sxs-lookup"><span data-stu-id="89027-141">America/Sao_Paulo</span></span>

<span data-ttu-id="89027-142">美洲/阿根廷/布宜诺斯艾利斯</span><span class="sxs-lookup"><span data-stu-id="89027-142">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="89027-143">美洲/卡宴</span><span class="sxs-lookup"><span data-stu-id="89027-143">America/Cayenne</span></span>

<span data-ttu-id="89027-144">美洲/戈特霍布</span><span class="sxs-lookup"><span data-stu-id="89027-144">America/Godthab</span></span>

<span data-ttu-id="89027-145">美洲/蒙得维的亚</span><span class="sxs-lookup"><span data-stu-id="89027-145">America/Montevideo</span></span>

<span data-ttu-id="89027-146">美洲/巴伊亚</span><span class="sxs-lookup"><span data-stu-id="89027-146">America/Bahia</span></span>

<span data-ttu-id="89027-147">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="89027-147">Etc/GMT+2</span></span>

<span data-ttu-id="89027-148">大西洋/亚速尔群岛</span><span class="sxs-lookup"><span data-stu-id="89027-148">Atlantic/Azores</span></span>

<span data-ttu-id="89027-149">大西洋/佛得角</span><span class="sxs-lookup"><span data-stu-id="89027-149">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="89027-150">非洲/卡萨布兰卡</span><span class="sxs-lookup"><span data-stu-id="89027-150">Africa/Casablanca</span></span>

<span data-ttu-id="89027-151">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="89027-151">Etc/GMT</span></span>

<span data-ttu-id="89027-152">欧洲/伦敦</span><span class="sxs-lookup"><span data-stu-id="89027-152">Europe/London</span></span>

<span data-ttu-id="89027-153">大西洋/雷克雅未克</span><span class="sxs-lookup"><span data-stu-id="89027-153">Atlantic/Reykjavik</span></span>

<span data-ttu-id="89027-154">欧洲/柏林</span><span class="sxs-lookup"><span data-stu-id="89027-154">Europe/Berlin</span></span>

<span data-ttu-id="89027-155">欧洲/布达佩斯</span><span class="sxs-lookup"><span data-stu-id="89027-155">Europe/Budapest</span></span>

<span data-ttu-id="89027-156">欧洲/巴黎</span><span class="sxs-lookup"><span data-stu-id="89027-156">Europe/Paris</span></span>

<span data-ttu-id="89027-157">欧洲/华沙</span><span class="sxs-lookup"><span data-stu-id="89027-157">Europe/Warsaw</span></span>

<span data-ttu-id="89027-158">非洲/拉各斯</span><span class="sxs-lookup"><span data-stu-id="89027-158">Africa/Lagos</span></span>

<span data-ttu-id="89027-159">非洲/温得和克</span><span class="sxs-lookup"><span data-stu-id="89027-159">Africa/Windhoek</span></span>

<span data-ttu-id="89027-160">欧洲/布加勒斯特</span><span class="sxs-lookup"><span data-stu-id="89027-160">Europe/Bucharest</span></span>

<span data-ttu-id="89027-161">亚洲/贝鲁特</span><span class="sxs-lookup"><span data-stu-id="89027-161">Asia/Beirut</span></span>

<span data-ttu-id="89027-162">非洲/开罗</span><span class="sxs-lookup"><span data-stu-id="89027-162">Africa/Cairo</span></span>

<span data-ttu-id="89027-163">亚洲/大马士革</span><span class="sxs-lookup"><span data-stu-id="89027-163">Asia/Damascus</span></span>

<span data-ttu-id="89027-164">非洲/约翰内斯堡</span><span class="sxs-lookup"><span data-stu-id="89027-164">Africa/Johannesburg</span></span>

<span data-ttu-id="89027-165">欧洲/基辅</span><span class="sxs-lookup"><span data-stu-id="89027-165">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="89027-166">欧洲/伊斯坦布尔</span><span class="sxs-lookup"><span data-stu-id="89027-166">Europe/Istanbul</span></span>

<span data-ttu-id="89027-167">亚洲/耶路撒冷</span><span class="sxs-lookup"><span data-stu-id="89027-167">Asia/Jerusalem</span></span>

<span data-ttu-id="89027-168">亚洲/安曼</span><span class="sxs-lookup"><span data-stu-id="89027-168">Asia/Amman</span></span>

<span data-ttu-id="89027-169">亚洲/巴格达</span><span class="sxs-lookup"><span data-stu-id="89027-169">Asia/Baghdad</span></span>

<span data-ttu-id="89027-170">欧洲/加里宁格勒</span><span class="sxs-lookup"><span data-stu-id="89027-170">Europe/Kaliningrad</span></span>

<span data-ttu-id="89027-171">亚洲/利雅得</span><span class="sxs-lookup"><span data-stu-id="89027-171">Asia/Riyadh</span></span>

<span data-ttu-id="89027-172">非洲/内罗毕</span><span class="sxs-lookup"><span data-stu-id="89027-172">Africa/Nairobi</span></span>

<span data-ttu-id="89027-173">亚洲/德黑兰</span><span class="sxs-lookup"><span data-stu-id="89027-173">Asia/Tehran</span></span>

<span data-ttu-id="89027-174">亚洲/迪拜</span><span class="sxs-lookup"><span data-stu-id="89027-174">Asia/Dubai</span></span>

<span data-ttu-id="89027-175">亚洲/巴库</span><span class="sxs-lookup"><span data-stu-id="89027-175">Asia/Baku</span></span>

<span data-ttu-id="89027-176">欧洲/莫斯科</span><span class="sxs-lookup"><span data-stu-id="89027-176">Europe/Moscow</span></span>

<span data-ttu-id="89027-177">印度洋/毛里求斯</span><span class="sxs-lookup"><span data-stu-id="89027-177">Indian/Mauritius</span></span>

<span data-ttu-id="89027-178">亚洲/第比利斯</span><span class="sxs-lookup"><span data-stu-id="89027-178">Asia/Tbilisi</span></span>

<span data-ttu-id="89027-179">亚洲/埃里温</span><span class="sxs-lookup"><span data-stu-id="89027-179">Asia/Yerevan</span></span>

<span data-ttu-id="89027-180">亚洲/喀布尔</span><span class="sxs-lookup"><span data-stu-id="89027-180">Asia/Kabul</span></span>

<span data-ttu-id="89027-181">亚洲/卡拉奇</span><span class="sxs-lookup"><span data-stu-id="89027-181">Asia/Karachi</span></span>

<span data-ttu-id="89027-182">亚洲/塔什干</span><span class="sxs-lookup"><span data-stu-id="89027-182">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="89027-183">亚洲/加尔各答</span><span class="sxs-lookup"><span data-stu-id="89027-183">Asia/Kolkata</span></span>

<span data-ttu-id="89027-184">亚洲/科伦坡</span><span class="sxs-lookup"><span data-stu-id="89027-184">Asia/Colombo</span></span>

<span data-ttu-id="89027-185">亚洲/加德满都</span><span class="sxs-lookup"><span data-stu-id="89027-185">Asia/Kathmandu</span></span>

<span data-ttu-id="89027-186">亚洲/阿斯塔纳（阿拉木图）</span><span class="sxs-lookup"><span data-stu-id="89027-186">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="89027-187">亚洲/达卡</span><span class="sxs-lookup"><span data-stu-id="89027-187">Asia/Dhaka</span></span>

<span data-ttu-id="89027-188">亚洲/叶卡捷琳堡</span><span class="sxs-lookup"><span data-stu-id="89027-188">Asia/Yekaterinburg</span></span>

<span data-ttu-id="89027-189">亚洲/仰光</span><span class="sxs-lookup"><span data-stu-id="89027-189">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="89027-190">亚洲/曼谷</span><span class="sxs-lookup"><span data-stu-id="89027-190">Asia/Bangkok</span></span>

<span data-ttu-id="89027-191">亚洲/新西伯利亚</span><span class="sxs-lookup"><span data-stu-id="89027-191">Asia/Novosibirsk</span></span>

<span data-ttu-id="89027-192">亚洲/上海</span><span class="sxs-lookup"><span data-stu-id="89027-192">Asia/Shanghai</span></span>

<span data-ttu-id="89027-193">亚洲/克拉斯诺亚尔斯克</span><span class="sxs-lookup"><span data-stu-id="89027-193">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="89027-194">亚洲/新加坡</span><span class="sxs-lookup"><span data-stu-id="89027-194">Asia/Singapore</span></span>

<span data-ttu-id="89027-195">澳大利亚/珀斯</span><span class="sxs-lookup"><span data-stu-id="89027-195">Australia/Perth</span></span>

<span data-ttu-id="89027-196">亚洲/台北</span><span class="sxs-lookup"><span data-stu-id="89027-196">Asia/Taipei</span></span>

<span data-ttu-id="89027-197">亚洲/乌兰巴托</span><span class="sxs-lookup"><span data-stu-id="89027-197">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="89027-198">亚洲/伊尔库茨克</span><span class="sxs-lookup"><span data-stu-id="89027-198">Asia/Irkutsk</span></span>

<span data-ttu-id="89027-199">亚洲/东京</span><span class="sxs-lookup"><span data-stu-id="89027-199">Asia/Tokyo</span></span>

<span data-ttu-id="89027-200">亚洲/首尔</span><span class="sxs-lookup"><span data-stu-id="89027-200">Asia/Seoul</span></span>

<span data-ttu-id="89027-201">澳洲/阿德莱德</span><span class="sxs-lookup"><span data-stu-id="89027-201">Australia/Adelaide</span></span>

<span data-ttu-id="89027-202">澳洲/达尔文</span><span class="sxs-lookup"><span data-stu-id="89027-202">Australia/Darwin</span></span>

<span data-ttu-id="89027-203">澳洲/布里斯班</span><span class="sxs-lookup"><span data-stu-id="89027-203">Australia/Brisbane</span></span>

<span data-ttu-id="89027-204">澳洲/悉尼</span><span class="sxs-lookup"><span data-stu-id="89027-204">Australia/Sydney</span></span>

<span data-ttu-id="89027-205">太平洋/莫尔斯比港</span><span class="sxs-lookup"><span data-stu-id="89027-205">Pacific/Port_Moresby</span></span>

<span data-ttu-id="89027-206">澳洲/霍巴特</span><span class="sxs-lookup"><span data-stu-id="89027-206">Australia/Hobart</span></span>

<span data-ttu-id="89027-207">亚洲/雅库茨克</span><span class="sxs-lookup"><span data-stu-id="89027-207">Asia/Yakutsk</span></span>

<span data-ttu-id="89027-208">太平洋/瓜达尔卡纳尔</span><span class="sxs-lookup"><span data-stu-id="89027-208">Pacific/Guadalcanal</span></span>

<span data-ttu-id="89027-209">亚洲/符拉迪沃斯托克</span><span class="sxs-lookup"><span data-stu-id="89027-209">Asia/Vladivostok</span></span>

<span data-ttu-id="89027-210">太平洋/奥克兰</span><span class="sxs-lookup"><span data-stu-id="89027-210">Pacific/Auckland</span></span>

<span data-ttu-id="89027-211">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="89027-211">Etc/GMT-12</span></span>

<span data-ttu-id="89027-212">太平洋/斐济</span><span class="sxs-lookup"><span data-stu-id="89027-212">Pacific/Fiji</span></span>

<span data-ttu-id="89027-213">亚洲/马加丹</span><span class="sxs-lookup"><span data-stu-id="89027-213">Asia/Magadan</span></span>

<span data-ttu-id="89027-214">太平洋/汤加塔布</span><span class="sxs-lookup"><span data-stu-id="89027-214">Pacific/Tongatapu</span></span>

<span data-ttu-id="89027-215">太平洋/阿皮亚</span><span class="sxs-lookup"><span data-stu-id="89027-215">Pacific/Apia</span></span>

<span data-ttu-id="89027-216">太平洋/圣诞岛</span><span class="sxs-lookup"><span data-stu-id="89027-216">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="89027-217">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="89027-217">JSON representation</span></span>

<span data-ttu-id="89027-218">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="89027-218">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.dateTimeTimeZone"
}-->

```json
{
  "dateTime": "string",
  "timeZone": "string"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "dateTimeTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
