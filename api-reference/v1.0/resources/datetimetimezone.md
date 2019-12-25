---
title: dateTimeTimeZone 资源类型
description: 介绍某个时间点的日期、时间和时区。
localization_priority: Priority
doc_type: resourcePageType
author: angelgolfer-ms
ms.prod: outlook
ms.openlocfilehash: 429f9b7d273b83b78580650ee323ea35343cdfaf
ms.sourcegitcommit: f27e81daeff242e623d1a3627405667310395734
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/25/2019
ms.locfileid: "40869834"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="73701-103">dateTimeTimeZone 资源类型</span><span class="sxs-lookup"><span data-stu-id="73701-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="73701-104">介绍某个时间点的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="73701-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="73701-105">属性</span><span class="sxs-lookup"><span data-stu-id="73701-105">Properties</span></span>
| <span data-ttu-id="73701-106">属性</span><span class="sxs-lookup"><span data-stu-id="73701-106">Property</span></span>     | <span data-ttu-id="73701-107">类型</span><span class="sxs-lookup"><span data-stu-id="73701-107">Type</span></span>   |<span data-ttu-id="73701-108">说明</span><span class="sxs-lookup"><span data-stu-id="73701-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="73701-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="73701-109">dateTime</span></span>|<span data-ttu-id="73701-110">字符串</span><span class="sxs-lookup"><span data-stu-id="73701-110">String</span></span>|<span data-ttu-id="73701-111">日期和时间组合表示形式的单个时间点（`{date}T{time}`；例如 `2017-08-29T04:00:00.0000000`）。</span><span class="sxs-lookup"><span data-stu-id="73701-111">A single point of time in a combined date and time representation (`{date}T{time}`; for example, `2017-08-29T04:00:00.0000000`).</span></span>|
|<span data-ttu-id="73701-112">timeZone</span><span class="sxs-lookup"><span data-stu-id="73701-112">timeZone</span></span>|<span data-ttu-id="73701-113">String</span><span class="sxs-lookup"><span data-stu-id="73701-113">String</span></span>|<span data-ttu-id="73701-114">表示时区，例如“太平洋标准时间”。</span><span class="sxs-lookup"><span data-stu-id="73701-114">Represents a time zone, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="73701-115">有关更多可能的值，请参见下文。</span><span class="sxs-lookup"><span data-stu-id="73701-115">See below for more possible values.</span></span>|

<span data-ttu-id="73701-116">通常，**timeZone** 属性_可以_ 设置为 [Windows 当前支持的任意时区](/windows-hardware/manufacture/desktop/default-time-zones)，以及[日历 API 支持的其他时区](#additional-time-zones)。</span><span class="sxs-lookup"><span data-stu-id="73701-116">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span>

<span data-ttu-id="73701-117">将 **dateTimeTimeZone** 与某一方法（例如[创建](../api/user-post-events.md)或[更新](../api/event-update.md)事件）结合使用时，请注意支持的实际时区，这可能是一个较小的子集。</span><span class="sxs-lookup"><span data-stu-id="73701-117">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="73701-118">其他时区</span><span class="sxs-lookup"><span data-stu-id="73701-118">Additional time zones</span></span>

<span data-ttu-id="73701-119">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="73701-119">Etc/GMT+12</span></span>

<span data-ttu-id="73701-120">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="73701-120">Etc/GMT+11</span></span>

<span data-ttu-id="73701-121">太平洋/火奴鲁鲁</span><span class="sxs-lookup"><span data-stu-id="73701-121">Pacific/Honolulu</span></span>

<span data-ttu-id="73701-122">美洲/安克雷奇</span><span class="sxs-lookup"><span data-stu-id="73701-122">America/Anchorage</span></span>

<span data-ttu-id="73701-123">美洲/圣伊莎贝尔</span><span class="sxs-lookup"><span data-stu-id="73701-123">America/Santa_Isabel</span></span>

<span data-ttu-id="73701-124">美洲/洛杉矶</span><span class="sxs-lookup"><span data-stu-id="73701-124">America/Los_Angeles</span></span>

<span data-ttu-id="73701-125">美洲/菲尼克斯</span><span class="sxs-lookup"><span data-stu-id="73701-125">America/Phoenix</span></span>

<span data-ttu-id="73701-126">美洲/奇瓦瓦</span><span class="sxs-lookup"><span data-stu-id="73701-126">America/Chihuahua</span></span>

<span data-ttu-id="73701-127">美洲/丹佛</span><span class="sxs-lookup"><span data-stu-id="73701-127">America/Denver</span></span>

<span data-ttu-id="73701-128">美洲/危地马拉</span><span class="sxs-lookup"><span data-stu-id="73701-128">America/Guatemala</span></span>

<span data-ttu-id="73701-129">美洲/芝加哥</span><span class="sxs-lookup"><span data-stu-id="73701-129">America/Chicago</span></span>

<span data-ttu-id="73701-130">美洲/墨西哥城</span><span class="sxs-lookup"><span data-stu-id="73701-130">America/Mexico_City</span></span>

<span data-ttu-id="73701-131">美洲/里贾纳</span><span class="sxs-lookup"><span data-stu-id="73701-131">America/Regina</span></span>

<span data-ttu-id="73701-132">美洲/波哥大</span><span class="sxs-lookup"><span data-stu-id="73701-132">America/Bogota</span></span>

<span data-ttu-id="73701-133">美洲/纽约</span><span class="sxs-lookup"><span data-stu-id="73701-133">America/New_York</span></span>

<span data-ttu-id="73701-134">美洲/印第安纳/印第安纳波利斯</span><span class="sxs-lookup"><span data-stu-id="73701-134">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="73701-135">美洲/加拉加斯</span><span class="sxs-lookup"><span data-stu-id="73701-135">America/Caracas</span></span>

<span data-ttu-id="73701-136">美洲/亚松森</span><span class="sxs-lookup"><span data-stu-id="73701-136">America/Asuncion</span></span>

<span data-ttu-id="73701-137">美洲/哈利法克斯</span><span class="sxs-lookup"><span data-stu-id="73701-137">America/Halifax</span></span>

<span data-ttu-id="73701-138">美洲/库亚巴</span><span class="sxs-lookup"><span data-stu-id="73701-138">America/Cuiaba</span></span>

<span data-ttu-id="73701-139">美洲/拉巴斯</span><span class="sxs-lookup"><span data-stu-id="73701-139">America/La_Paz</span></span>

<span data-ttu-id="73701-140">美洲/圣地亚哥</span><span class="sxs-lookup"><span data-stu-id="73701-140">America/Santiago</span></span>

<span data-ttu-id="73701-141">美洲/圣约翰斯</span><span class="sxs-lookup"><span data-stu-id="73701-141">America/St_Johns</span></span>

<span data-ttu-id="73701-142">美洲/圣保罗</span><span class="sxs-lookup"><span data-stu-id="73701-142">America/Sao_Paulo</span></span>

<span data-ttu-id="73701-143">美洲/阿根廷/布宜诺斯艾利斯</span><span class="sxs-lookup"><span data-stu-id="73701-143">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="73701-144">美洲/卡宴</span><span class="sxs-lookup"><span data-stu-id="73701-144">America/Cayenne</span></span>

<span data-ttu-id="73701-145">美洲/戈特霍布</span><span class="sxs-lookup"><span data-stu-id="73701-145">America/Godthab</span></span>

<span data-ttu-id="73701-146">美洲/蒙得维的亚</span><span class="sxs-lookup"><span data-stu-id="73701-146">America/Montevideo</span></span>

<span data-ttu-id="73701-147">美洲/巴伊亚</span><span class="sxs-lookup"><span data-stu-id="73701-147">America/Bahia</span></span>

<span data-ttu-id="73701-148">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="73701-148">Etc/GMT+2</span></span>

<span data-ttu-id="73701-149">大西洋/亚速尔群岛</span><span class="sxs-lookup"><span data-stu-id="73701-149">Atlantic/Azores</span></span>

<span data-ttu-id="73701-150">大西洋/佛得角</span><span class="sxs-lookup"><span data-stu-id="73701-150">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="73701-151">非洲/卡萨布兰卡</span><span class="sxs-lookup"><span data-stu-id="73701-151">Africa/Casablanca</span></span>

<span data-ttu-id="73701-152">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="73701-152">Etc/GMT</span></span>

<span data-ttu-id="73701-153">欧洲/伦敦</span><span class="sxs-lookup"><span data-stu-id="73701-153">Europe/London</span></span>

<span data-ttu-id="73701-154">大西洋/雷克雅未克</span><span class="sxs-lookup"><span data-stu-id="73701-154">Atlantic/Reykjavik</span></span>

<span data-ttu-id="73701-155">欧洲/柏林</span><span class="sxs-lookup"><span data-stu-id="73701-155">Europe/Berlin</span></span>

<span data-ttu-id="73701-156">欧洲/布达佩斯</span><span class="sxs-lookup"><span data-stu-id="73701-156">Europe/Budapest</span></span>

<span data-ttu-id="73701-157">欧洲/巴黎</span><span class="sxs-lookup"><span data-stu-id="73701-157">Europe/Paris</span></span>

<span data-ttu-id="73701-158">欧洲/华沙</span><span class="sxs-lookup"><span data-stu-id="73701-158">Europe/Warsaw</span></span>

<span data-ttu-id="73701-159">非洲/拉各斯</span><span class="sxs-lookup"><span data-stu-id="73701-159">Africa/Lagos</span></span>

<span data-ttu-id="73701-160">非洲/温得和克</span><span class="sxs-lookup"><span data-stu-id="73701-160">Africa/Windhoek</span></span>

<span data-ttu-id="73701-161">欧洲/布加勒斯特</span><span class="sxs-lookup"><span data-stu-id="73701-161">Europe/Bucharest</span></span>

<span data-ttu-id="73701-162">亚洲/贝鲁特</span><span class="sxs-lookup"><span data-stu-id="73701-162">Asia/Beirut</span></span>

<span data-ttu-id="73701-163">非洲/开罗</span><span class="sxs-lookup"><span data-stu-id="73701-163">Africa/Cairo</span></span>

<span data-ttu-id="73701-164">亚洲/大马士革</span><span class="sxs-lookup"><span data-stu-id="73701-164">Asia/Damascus</span></span>

<span data-ttu-id="73701-165">非洲/约翰内斯堡</span><span class="sxs-lookup"><span data-stu-id="73701-165">Africa/Johannesburg</span></span>

<span data-ttu-id="73701-166">欧洲/基辅</span><span class="sxs-lookup"><span data-stu-id="73701-166">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="73701-167">欧洲/伊斯坦布尔</span><span class="sxs-lookup"><span data-stu-id="73701-167">Europe/Istanbul</span></span>

<span data-ttu-id="73701-168">亚洲/耶路撒冷</span><span class="sxs-lookup"><span data-stu-id="73701-168">Asia/Jerusalem</span></span>

<span data-ttu-id="73701-169">亚洲/安曼</span><span class="sxs-lookup"><span data-stu-id="73701-169">Asia/Amman</span></span>

<span data-ttu-id="73701-170">亚洲/巴格达</span><span class="sxs-lookup"><span data-stu-id="73701-170">Asia/Baghdad</span></span>

<span data-ttu-id="73701-171">欧洲/加里宁格勒</span><span class="sxs-lookup"><span data-stu-id="73701-171">Europe/Kaliningrad</span></span>

<span data-ttu-id="73701-172">亚洲/利雅得</span><span class="sxs-lookup"><span data-stu-id="73701-172">Asia/Riyadh</span></span>

<span data-ttu-id="73701-173">非洲/内罗毕</span><span class="sxs-lookup"><span data-stu-id="73701-173">Africa/Nairobi</span></span>

<span data-ttu-id="73701-174">亚洲/德黑兰</span><span class="sxs-lookup"><span data-stu-id="73701-174">Asia/Tehran</span></span>

<span data-ttu-id="73701-175">亚洲/迪拜</span><span class="sxs-lookup"><span data-stu-id="73701-175">Asia/Dubai</span></span>

<span data-ttu-id="73701-176">亚洲/巴库</span><span class="sxs-lookup"><span data-stu-id="73701-176">Asia/Baku</span></span>

<span data-ttu-id="73701-177">欧洲/莫斯科</span><span class="sxs-lookup"><span data-stu-id="73701-177">Europe/Moscow</span></span>

<span data-ttu-id="73701-178">印度洋/毛里求斯</span><span class="sxs-lookup"><span data-stu-id="73701-178">Indian/Mauritius</span></span>

<span data-ttu-id="73701-179">亚洲/第比利斯</span><span class="sxs-lookup"><span data-stu-id="73701-179">Asia/Tbilisi</span></span>

<span data-ttu-id="73701-180">亚洲/埃里温</span><span class="sxs-lookup"><span data-stu-id="73701-180">Asia/Yerevan</span></span>

<span data-ttu-id="73701-181">亚洲/喀布尔</span><span class="sxs-lookup"><span data-stu-id="73701-181">Asia/Kabul</span></span>

<span data-ttu-id="73701-182">亚洲/卡拉奇</span><span class="sxs-lookup"><span data-stu-id="73701-182">Asia/Karachi</span></span>

<span data-ttu-id="73701-183">亚洲/塔什干</span><span class="sxs-lookup"><span data-stu-id="73701-183">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="73701-184">亚洲/加尔各答</span><span class="sxs-lookup"><span data-stu-id="73701-184">Asia/Kolkata</span></span>

<span data-ttu-id="73701-185">亚洲/科伦坡</span><span class="sxs-lookup"><span data-stu-id="73701-185">Asia/Colombo</span></span>

<span data-ttu-id="73701-186">亚洲/加德满都</span><span class="sxs-lookup"><span data-stu-id="73701-186">Asia/Kathmandu</span></span>

<span data-ttu-id="73701-187">亚洲/阿斯塔纳（阿拉木图）</span><span class="sxs-lookup"><span data-stu-id="73701-187">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="73701-188">亚洲/达卡</span><span class="sxs-lookup"><span data-stu-id="73701-188">Asia/Dhaka</span></span>

<span data-ttu-id="73701-189">亚洲/叶卡捷琳堡</span><span class="sxs-lookup"><span data-stu-id="73701-189">Asia/Yekaterinburg</span></span>

<span data-ttu-id="73701-190">亚洲/仰光</span><span class="sxs-lookup"><span data-stu-id="73701-190">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="73701-191">亚洲/曼谷</span><span class="sxs-lookup"><span data-stu-id="73701-191">Asia/Bangkok</span></span>

<span data-ttu-id="73701-192">亚洲/新西伯利亚</span><span class="sxs-lookup"><span data-stu-id="73701-192">Asia/Novosibirsk</span></span>

<span data-ttu-id="73701-193">亚洲/上海</span><span class="sxs-lookup"><span data-stu-id="73701-193">Asia/Shanghai</span></span>

<span data-ttu-id="73701-194">亚洲/克拉斯诺亚尔斯克</span><span class="sxs-lookup"><span data-stu-id="73701-194">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="73701-195">亚洲/新加坡</span><span class="sxs-lookup"><span data-stu-id="73701-195">Asia/Singapore</span></span>

<span data-ttu-id="73701-196">澳大利亚/珀斯</span><span class="sxs-lookup"><span data-stu-id="73701-196">Australia/Perth</span></span>

<span data-ttu-id="73701-197">亚洲/台北</span><span class="sxs-lookup"><span data-stu-id="73701-197">Asia/Taipei</span></span>

<span data-ttu-id="73701-198">亚洲/乌兰巴托</span><span class="sxs-lookup"><span data-stu-id="73701-198">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="73701-199">亚洲/伊尔库茨克</span><span class="sxs-lookup"><span data-stu-id="73701-199">Asia/Irkutsk</span></span>

<span data-ttu-id="73701-200">亚洲/东京</span><span class="sxs-lookup"><span data-stu-id="73701-200">Asia/Tokyo</span></span>

<span data-ttu-id="73701-201">亚洲/首尔</span><span class="sxs-lookup"><span data-stu-id="73701-201">Asia/Seoul</span></span>

<span data-ttu-id="73701-202">澳洲/阿德莱德</span><span class="sxs-lookup"><span data-stu-id="73701-202">Australia/Adelaide</span></span>

<span data-ttu-id="73701-203">澳洲/达尔文</span><span class="sxs-lookup"><span data-stu-id="73701-203">Australia/Darwin</span></span>

<span data-ttu-id="73701-204">澳洲/布里斯班</span><span class="sxs-lookup"><span data-stu-id="73701-204">Australia/Brisbane</span></span>

<span data-ttu-id="73701-205">澳洲/悉尼</span><span class="sxs-lookup"><span data-stu-id="73701-205">Australia/Sydney</span></span>

<span data-ttu-id="73701-206">太平洋/莫尔斯比港</span><span class="sxs-lookup"><span data-stu-id="73701-206">Pacific/Port_Moresby</span></span>

<span data-ttu-id="73701-207">澳洲/霍巴特</span><span class="sxs-lookup"><span data-stu-id="73701-207">Australia/Hobart</span></span>

<span data-ttu-id="73701-208">亚洲/雅库茨克</span><span class="sxs-lookup"><span data-stu-id="73701-208">Asia/Yakutsk</span></span>

<span data-ttu-id="73701-209">太平洋/瓜达尔卡纳尔</span><span class="sxs-lookup"><span data-stu-id="73701-209">Pacific/Guadalcanal</span></span>

<span data-ttu-id="73701-210">亚洲/符拉迪沃斯托克</span><span class="sxs-lookup"><span data-stu-id="73701-210">Asia/Vladivostok</span></span>

<span data-ttu-id="73701-211">太平洋/奥克兰</span><span class="sxs-lookup"><span data-stu-id="73701-211">Pacific/Auckland</span></span>

<span data-ttu-id="73701-212">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="73701-212">Etc/GMT-12</span></span>

<span data-ttu-id="73701-213">太平洋/斐济</span><span class="sxs-lookup"><span data-stu-id="73701-213">Pacific/Fiji</span></span>

<span data-ttu-id="73701-214">亚洲/马加丹</span><span class="sxs-lookup"><span data-stu-id="73701-214">Asia/Magadan</span></span>

<span data-ttu-id="73701-215">太平洋/汤加塔布</span><span class="sxs-lookup"><span data-stu-id="73701-215">Pacific/Tongatapu</span></span>

<span data-ttu-id="73701-216">太平洋/阿皮亚</span><span class="sxs-lookup"><span data-stu-id="73701-216">Pacific/Apia</span></span>

<span data-ttu-id="73701-217">太平洋/圣诞岛</span><span class="sxs-lookup"><span data-stu-id="73701-217">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="73701-218">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="73701-218">JSON representation</span></span>

<span data-ttu-id="73701-219">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="73701-219">Here is a JSON representation of the resource</span></span>

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
