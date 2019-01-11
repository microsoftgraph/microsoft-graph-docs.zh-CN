---
title: dateTimeTimeZone 资源类型
description: 介绍某个时间点的日期、时间和时区。
localization_priority: Priority
ms.openlocfilehash: 9bec62c21f97c58b915ecc40010f8030ea760825
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 01/11/2019
ms.locfileid: "27827326"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="b45de-103">dateTimeTimeZone 资源类型</span><span class="sxs-lookup"><span data-stu-id="b45de-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="b45de-104">介绍某个时间点的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="b45de-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="b45de-105">属性</span><span class="sxs-lookup"><span data-stu-id="b45de-105">Properties</span></span>
| <span data-ttu-id="b45de-106">属性</span><span class="sxs-lookup"><span data-stu-id="b45de-106">Property</span></span>     | <span data-ttu-id="b45de-107">类型</span><span class="sxs-lookup"><span data-stu-id="b45de-107">Type</span></span>   |<span data-ttu-id="b45de-108">Description</span><span class="sxs-lookup"><span data-stu-id="b45de-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="b45de-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="b45de-109">dateTime</span></span>|<span data-ttu-id="b45de-110">String</span><span class="sxs-lookup"><span data-stu-id="b45de-110">String</span></span>|<span data-ttu-id="b45de-111">日期和时间组合表示形式的单个时间点 (`<date>T<time>`)。</span><span class="sxs-lookup"><span data-stu-id="b45de-111">A single point of time in a combined date and time representation (`<date>T<time>`).</span></span>|
|<span data-ttu-id="b45de-112">timeZone</span><span class="sxs-lookup"><span data-stu-id="b45de-112">timeZone</span></span>|<span data-ttu-id="b45de-113">String</span><span class="sxs-lookup"><span data-stu-id="b45de-113">String</span></span>|<span data-ttu-id="b45de-114">以下时区名称之一。</span><span class="sxs-lookup"><span data-stu-id="b45de-114">One of the following time zone names.</span></span>|

<span data-ttu-id="b45de-115">_TimeZone_ 属性可以设置为 Windows 支持的任意时区，以及以下时区名称。</span><span class="sxs-lookup"><span data-stu-id="b45de-115">The _TimeZone_ property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="b45de-116">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="b45de-116">Etc/GMT+12</span></span>

<span data-ttu-id="b45de-117">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="b45de-117">Etc/GMT+11</span></span>

<span data-ttu-id="b45de-118">太平洋/火奴鲁鲁</span><span class="sxs-lookup"><span data-stu-id="b45de-118">Pacific/Honolulu</span></span>

<span data-ttu-id="b45de-119">美洲/安克雷奇</span><span class="sxs-lookup"><span data-stu-id="b45de-119">America/Anchorage</span></span>

<span data-ttu-id="b45de-120">美洲/圣伊莎贝尔</span><span class="sxs-lookup"><span data-stu-id="b45de-120">America/Santa_Isabel</span></span>

<span data-ttu-id="b45de-121">美洲/洛杉矶</span><span class="sxs-lookup"><span data-stu-id="b45de-121">America/Los_Angeles</span></span>

<span data-ttu-id="b45de-122">美洲/菲尼克斯</span><span class="sxs-lookup"><span data-stu-id="b45de-122">America/Phoenix</span></span>

<span data-ttu-id="b45de-123">美洲/奇瓦瓦</span><span class="sxs-lookup"><span data-stu-id="b45de-123">America/Chihuahua</span></span>

<span data-ttu-id="b45de-124">美洲/丹佛</span><span class="sxs-lookup"><span data-stu-id="b45de-124">America/Denver</span></span>

<span data-ttu-id="b45de-125">美洲/危地马拉</span><span class="sxs-lookup"><span data-stu-id="b45de-125">America/Guatemala</span></span>

<span data-ttu-id="b45de-126">美洲/芝加哥</span><span class="sxs-lookup"><span data-stu-id="b45de-126">America/Chicago</span></span>

<span data-ttu-id="b45de-127">美洲/墨西哥城</span><span class="sxs-lookup"><span data-stu-id="b45de-127">America/Mexico_City</span></span>

<span data-ttu-id="b45de-128">美洲/里贾纳</span><span class="sxs-lookup"><span data-stu-id="b45de-128">America/Regina</span></span>

<span data-ttu-id="b45de-129">美洲/波哥大</span><span class="sxs-lookup"><span data-stu-id="b45de-129">America/Bogota</span></span>

<span data-ttu-id="b45de-130">美洲/纽约</span><span class="sxs-lookup"><span data-stu-id="b45de-130">America/New_York</span></span>

<span data-ttu-id="b45de-131">美洲/印第安纳/印第安纳波利斯</span><span class="sxs-lookup"><span data-stu-id="b45de-131">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="b45de-132">美洲/加拉加斯</span><span class="sxs-lookup"><span data-stu-id="b45de-132">America/Caracas</span></span>

<span data-ttu-id="b45de-133">美洲/亚松森</span><span class="sxs-lookup"><span data-stu-id="b45de-133">America/Asuncion</span></span>

<span data-ttu-id="b45de-134">美洲/哈利法克斯</span><span class="sxs-lookup"><span data-stu-id="b45de-134">America/Halifax</span></span>

<span data-ttu-id="b45de-135">美洲/库亚巴</span><span class="sxs-lookup"><span data-stu-id="b45de-135">America/Cuiaba</span></span>

<span data-ttu-id="b45de-136">美洲/拉巴斯</span><span class="sxs-lookup"><span data-stu-id="b45de-136">America/La_Paz</span></span>

<span data-ttu-id="b45de-137">美洲/圣地亚哥</span><span class="sxs-lookup"><span data-stu-id="b45de-137">America/Santiago</span></span>

<span data-ttu-id="b45de-138">美洲/圣约翰斯</span><span class="sxs-lookup"><span data-stu-id="b45de-138">America/St_Johns</span></span>

<span data-ttu-id="b45de-139">美洲/圣保罗</span><span class="sxs-lookup"><span data-stu-id="b45de-139">America/Sao_Paulo</span></span>

<span data-ttu-id="b45de-140">美洲/阿根廷/布宜诺斯艾利斯</span><span class="sxs-lookup"><span data-stu-id="b45de-140">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="b45de-141">美洲/卡宴</span><span class="sxs-lookup"><span data-stu-id="b45de-141">America/Cayenne</span></span>

<span data-ttu-id="b45de-142">美洲/戈特霍布</span><span class="sxs-lookup"><span data-stu-id="b45de-142">America/Godthab</span></span>

<span data-ttu-id="b45de-143">美洲/蒙得维的亚</span><span class="sxs-lookup"><span data-stu-id="b45de-143">America/Montevideo</span></span>

<span data-ttu-id="b45de-144">美洲/巴伊亚</span><span class="sxs-lookup"><span data-stu-id="b45de-144">America/Bahia</span></span>

<span data-ttu-id="b45de-145">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="b45de-145">Etc/GMT+2</span></span>

<span data-ttu-id="b45de-146">大西洋/亚速尔群岛</span><span class="sxs-lookup"><span data-stu-id="b45de-146">Atlantic/Azores</span></span>

<span data-ttu-id="b45de-147">大西洋/佛得角</span><span class="sxs-lookup"><span data-stu-id="b45de-147">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="b45de-148">非洲/卡萨布兰卡</span><span class="sxs-lookup"><span data-stu-id="b45de-148">Africa/Casablanca</span></span>

<span data-ttu-id="b45de-149">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="b45de-149">Etc/GMT</span></span>

<span data-ttu-id="b45de-150">欧洲/伦敦</span><span class="sxs-lookup"><span data-stu-id="b45de-150">Europe/London</span></span>

<span data-ttu-id="b45de-151">大西洋/雷克雅未克</span><span class="sxs-lookup"><span data-stu-id="b45de-151">Atlantic/Reykjavik</span></span>

<span data-ttu-id="b45de-152">欧洲/柏林</span><span class="sxs-lookup"><span data-stu-id="b45de-152">Europe/Berlin</span></span>

<span data-ttu-id="b45de-153">欧洲/布达佩斯</span><span class="sxs-lookup"><span data-stu-id="b45de-153">Europe/Budapest</span></span>

<span data-ttu-id="b45de-154">欧洲/巴黎</span><span class="sxs-lookup"><span data-stu-id="b45de-154">Europe/Paris</span></span>

<span data-ttu-id="b45de-155">欧洲/华沙</span><span class="sxs-lookup"><span data-stu-id="b45de-155">Europe/Warsaw</span></span>

<span data-ttu-id="b45de-156">非洲/拉各斯</span><span class="sxs-lookup"><span data-stu-id="b45de-156">Africa/Lagos</span></span>

<span data-ttu-id="b45de-157">非洲/温得和克</span><span class="sxs-lookup"><span data-stu-id="b45de-157">Africa/Windhoek</span></span>

<span data-ttu-id="b45de-158">欧洲/布加勒斯特</span><span class="sxs-lookup"><span data-stu-id="b45de-158">Europe/Bucharest</span></span>

<span data-ttu-id="b45de-159">亚洲/贝鲁特</span><span class="sxs-lookup"><span data-stu-id="b45de-159">Asia/Beirut</span></span>

<span data-ttu-id="b45de-160">非洲/开罗</span><span class="sxs-lookup"><span data-stu-id="b45de-160">Africa/Cairo</span></span>

<span data-ttu-id="b45de-161">亚洲/大马士革</span><span class="sxs-lookup"><span data-stu-id="b45de-161">Asia/Damascus</span></span>

<span data-ttu-id="b45de-162">非洲/约翰内斯堡</span><span class="sxs-lookup"><span data-stu-id="b45de-162">Africa/Johannesburg</span></span>

<span data-ttu-id="b45de-163">欧洲/基辅</span><span class="sxs-lookup"><span data-stu-id="b45de-163">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="b45de-164">欧洲/伊斯坦布尔</span><span class="sxs-lookup"><span data-stu-id="b45de-164">Europe/Istanbul</span></span>

<span data-ttu-id="b45de-165">亚洲/耶路撒冷</span><span class="sxs-lookup"><span data-stu-id="b45de-165">Asia/Jerusalem</span></span>

<span data-ttu-id="b45de-166">亚洲/安曼</span><span class="sxs-lookup"><span data-stu-id="b45de-166">Asia/Amman</span></span>

<span data-ttu-id="b45de-167">亚洲/巴格达</span><span class="sxs-lookup"><span data-stu-id="b45de-167">Asia/Baghdad</span></span>

<span data-ttu-id="b45de-168">欧洲/加里宁格勒</span><span class="sxs-lookup"><span data-stu-id="b45de-168">Europe/Kaliningrad</span></span>

<span data-ttu-id="b45de-169">亚洲/利雅得</span><span class="sxs-lookup"><span data-stu-id="b45de-169">Asia/Riyadh</span></span>

<span data-ttu-id="b45de-170">非洲/内罗毕</span><span class="sxs-lookup"><span data-stu-id="b45de-170">Africa/Nairobi</span></span>

<span data-ttu-id="b45de-171">亚洲/德黑兰</span><span class="sxs-lookup"><span data-stu-id="b45de-171">Asia/Tehran</span></span>

<span data-ttu-id="b45de-172">亚洲/迪拜</span><span class="sxs-lookup"><span data-stu-id="b45de-172">Asia/Dubai</span></span>

<span data-ttu-id="b45de-173">亚洲/巴库</span><span class="sxs-lookup"><span data-stu-id="b45de-173">Asia/Baku</span></span>

<span data-ttu-id="b45de-174">欧洲/莫斯科</span><span class="sxs-lookup"><span data-stu-id="b45de-174">Europe/Moscow</span></span>

<span data-ttu-id="b45de-175">印度洋/毛里求斯</span><span class="sxs-lookup"><span data-stu-id="b45de-175">Indian/Mauritius</span></span>

<span data-ttu-id="b45de-176">亚洲/第比利斯</span><span class="sxs-lookup"><span data-stu-id="b45de-176">Asia/Tbilisi</span></span>

<span data-ttu-id="b45de-177">亚洲/埃里温</span><span class="sxs-lookup"><span data-stu-id="b45de-177">Asia/Yerevan</span></span>

<span data-ttu-id="b45de-178">亚洲/喀布尔</span><span class="sxs-lookup"><span data-stu-id="b45de-178">Asia/Kabul</span></span>

<span data-ttu-id="b45de-179">亚洲/卡拉奇</span><span class="sxs-lookup"><span data-stu-id="b45de-179">Asia/Karachi</span></span>

<span data-ttu-id="b45de-180">亚洲/塔什干</span><span class="sxs-lookup"><span data-stu-id="b45de-180">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="b45de-181">亚洲/加尔各答</span><span class="sxs-lookup"><span data-stu-id="b45de-181">Asia/Kolkata</span></span>

<span data-ttu-id="b45de-182">亚洲/科伦坡</span><span class="sxs-lookup"><span data-stu-id="b45de-182">Asia/Colombo</span></span>

<span data-ttu-id="b45de-183">亚洲/加德满都</span><span class="sxs-lookup"><span data-stu-id="b45de-183">Asia/Kathmandu</span></span>

<span data-ttu-id="b45de-184">亚洲/阿斯塔纳（阿拉木图）</span><span class="sxs-lookup"><span data-stu-id="b45de-184">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="b45de-185">亚洲/达卡</span><span class="sxs-lookup"><span data-stu-id="b45de-185">Asia/Dhaka</span></span>

<span data-ttu-id="b45de-186">亚洲/叶卡捷琳堡</span><span class="sxs-lookup"><span data-stu-id="b45de-186">Asia/Yekaterinburg</span></span>

<span data-ttu-id="b45de-187">亚洲/仰光</span><span class="sxs-lookup"><span data-stu-id="b45de-187">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="b45de-188">亚洲/曼谷</span><span class="sxs-lookup"><span data-stu-id="b45de-188">Asia/Bangkok</span></span>

<span data-ttu-id="b45de-189">亚洲/新西伯利亚</span><span class="sxs-lookup"><span data-stu-id="b45de-189">Asia/Novosibirsk</span></span>

<span data-ttu-id="b45de-190">亚洲/上海</span><span class="sxs-lookup"><span data-stu-id="b45de-190">Asia/Shanghai</span></span>

<span data-ttu-id="b45de-191">亚洲/克拉斯诺亚尔斯克</span><span class="sxs-lookup"><span data-stu-id="b45de-191">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="b45de-192">亚洲/新加坡</span><span class="sxs-lookup"><span data-stu-id="b45de-192">Asia/Singapore</span></span>

<span data-ttu-id="b45de-193">澳大利亚/珀斯</span><span class="sxs-lookup"><span data-stu-id="b45de-193">Australia/Perth</span></span>

<span data-ttu-id="b45de-194">亚洲/台北</span><span class="sxs-lookup"><span data-stu-id="b45de-194">Asia/Taipei</span></span>

<span data-ttu-id="b45de-195">亚洲/乌兰巴托</span><span class="sxs-lookup"><span data-stu-id="b45de-195">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="b45de-196">亚洲/伊尔库茨克</span><span class="sxs-lookup"><span data-stu-id="b45de-196">Asia/Irkutsk</span></span>

<span data-ttu-id="b45de-197">亚洲/东京</span><span class="sxs-lookup"><span data-stu-id="b45de-197">Asia/Tokyo</span></span>

<span data-ttu-id="b45de-198">亚洲/首尔</span><span class="sxs-lookup"><span data-stu-id="b45de-198">Asia/Seoul</span></span>

<span data-ttu-id="b45de-199">澳洲/阿德莱德</span><span class="sxs-lookup"><span data-stu-id="b45de-199">Australia/Adelaide</span></span>

<span data-ttu-id="b45de-200">澳洲/达尔文</span><span class="sxs-lookup"><span data-stu-id="b45de-200">Australia/Darwin</span></span>

<span data-ttu-id="b45de-201">澳洲/布里斯班</span><span class="sxs-lookup"><span data-stu-id="b45de-201">Australia/Brisbane</span></span>

<span data-ttu-id="b45de-202">澳洲/悉尼</span><span class="sxs-lookup"><span data-stu-id="b45de-202">Australia/Sydney</span></span>

<span data-ttu-id="b45de-203">太平洋/莫尔斯比港</span><span class="sxs-lookup"><span data-stu-id="b45de-203">Pacific/Port_Moresby</span></span>

<span data-ttu-id="b45de-204">澳洲/霍巴特</span><span class="sxs-lookup"><span data-stu-id="b45de-204">Australia/Hobart</span></span>

<span data-ttu-id="b45de-205">亚洲/雅库茨克</span><span class="sxs-lookup"><span data-stu-id="b45de-205">Asia/Yakutsk</span></span>

<span data-ttu-id="b45de-206">太平洋/瓜达尔卡纳尔</span><span class="sxs-lookup"><span data-stu-id="b45de-206">Pacific/Guadalcanal</span></span>

<span data-ttu-id="b45de-207">亚洲/符拉迪沃斯托克</span><span class="sxs-lookup"><span data-stu-id="b45de-207">Asia/Vladivostok</span></span>

<span data-ttu-id="b45de-208">太平洋/奥克兰</span><span class="sxs-lookup"><span data-stu-id="b45de-208">Pacific/Auckland</span></span>

<span data-ttu-id="b45de-209">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="b45de-209">Etc/GMT-12</span></span>

<span data-ttu-id="b45de-210">太平洋/斐济</span><span class="sxs-lookup"><span data-stu-id="b45de-210">Pacific/Fiji</span></span>

<span data-ttu-id="b45de-211">亚洲/马加丹</span><span class="sxs-lookup"><span data-stu-id="b45de-211">Asia/Magadan</span></span>

<span data-ttu-id="b45de-212">太平洋/汤加塔布</span><span class="sxs-lookup"><span data-stu-id="b45de-212">Pacific/Tongatapu</span></span>

<span data-ttu-id="b45de-213">太平洋/阿皮亚</span><span class="sxs-lookup"><span data-stu-id="b45de-213">Pacific/Apia</span></span>

<span data-ttu-id="b45de-214">太平洋/圣诞岛</span><span class="sxs-lookup"><span data-stu-id="b45de-214">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="b45de-215">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b45de-215">JSON representation</span></span>

<span data-ttu-id="b45de-216">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b45de-216">Here is a JSON representation of the resource</span></span>

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
