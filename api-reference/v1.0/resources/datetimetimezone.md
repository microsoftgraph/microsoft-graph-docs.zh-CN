---
title: dateTimeTimeZone 资源类型
description: 介绍某个时间点的日期、时间和时区。
localization_priority: Priority
doc_type: resourcePageType
author: harini84
ms.prod: outlook
ms.openlocfilehash: 3af4a12dad40cd6f18790ddedf99ef7e3a1770f6
ms.sourcegitcommit: bbcf074f0be9d5e02f84c290122850cc5968fb1f
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/14/2020
ms.locfileid: "43449423"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="2965a-103">dateTimeTimeZone 资源类型</span><span class="sxs-lookup"><span data-stu-id="2965a-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="2965a-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2965a-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="2965a-105">介绍某个时间点的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="2965a-105">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="2965a-106">属性</span><span class="sxs-lookup"><span data-stu-id="2965a-106">Properties</span></span>
| <span data-ttu-id="2965a-107">属性</span><span class="sxs-lookup"><span data-stu-id="2965a-107">Property</span></span>     | <span data-ttu-id="2965a-108">类型</span><span class="sxs-lookup"><span data-stu-id="2965a-108">Type</span></span>   |<span data-ttu-id="2965a-109">说明</span><span class="sxs-lookup"><span data-stu-id="2965a-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2965a-110">dateTime</span><span class="sxs-lookup"><span data-stu-id="2965a-110">dateTime</span></span>|<span data-ttu-id="2965a-111">字符串</span><span class="sxs-lookup"><span data-stu-id="2965a-111">String</span></span>|<span data-ttu-id="2965a-112">日期和时间组合表示形式的单个时间点（`{date}T{time}`；例如 `2017-08-29T04:00:00.0000000`）。</span><span class="sxs-lookup"><span data-stu-id="2965a-112">A single point of time in a combined date and time representation (`{date}T{time}`; for example, `2017-08-29T04:00:00.0000000`).</span></span>|
|<span data-ttu-id="2965a-113">timeZone</span><span class="sxs-lookup"><span data-stu-id="2965a-113">timeZone</span></span>|<span data-ttu-id="2965a-114">String</span><span class="sxs-lookup"><span data-stu-id="2965a-114">String</span></span>|<span data-ttu-id="2965a-115">表示时区，例如“太平洋标准时间”。</span><span class="sxs-lookup"><span data-stu-id="2965a-115">Represents a time zone, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="2965a-116">有关更多可能的值，请参见下文。</span><span class="sxs-lookup"><span data-stu-id="2965a-116">See below for more possible values.</span></span>|

<span data-ttu-id="2965a-117">通常，**timeZone** 属性_可以_ 设置为 [Windows 当前支持的任意时区](/windows-hardware/manufacture/desktop/default-time-zones)，以及[日历 API 支持的其他时区](#additional-time-zones)。</span><span class="sxs-lookup"><span data-stu-id="2965a-117">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span>

<span data-ttu-id="2965a-118">将 **dateTimeTimeZone** 与某一方法（例如[创建](../api/user-post-events.md)或[更新](../api/event-update.md)事件）结合使用时，请注意支持的实际时区，这可能是一个较小的子集。</span><span class="sxs-lookup"><span data-stu-id="2965a-118">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="2965a-119">其他时区</span><span class="sxs-lookup"><span data-stu-id="2965a-119">Additional time zones</span></span>

<span data-ttu-id="2965a-120">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="2965a-120">Etc/GMT+12</span></span>

<span data-ttu-id="2965a-121">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="2965a-121">Etc/GMT+11</span></span>

<span data-ttu-id="2965a-122">太平洋/火奴鲁鲁</span><span class="sxs-lookup"><span data-stu-id="2965a-122">Pacific/Honolulu</span></span>

<span data-ttu-id="2965a-123">美洲/安克雷奇</span><span class="sxs-lookup"><span data-stu-id="2965a-123">America/Anchorage</span></span>

<span data-ttu-id="2965a-124">美洲/圣伊莎贝尔</span><span class="sxs-lookup"><span data-stu-id="2965a-124">America/Santa_Isabel</span></span>

<span data-ttu-id="2965a-125">美洲/洛杉矶</span><span class="sxs-lookup"><span data-stu-id="2965a-125">America/Los_Angeles</span></span>

<span data-ttu-id="2965a-126">美洲/菲尼克斯</span><span class="sxs-lookup"><span data-stu-id="2965a-126">America/Phoenix</span></span>

<span data-ttu-id="2965a-127">美洲/奇瓦瓦</span><span class="sxs-lookup"><span data-stu-id="2965a-127">America/Chihuahua</span></span>

<span data-ttu-id="2965a-128">美洲/丹佛</span><span class="sxs-lookup"><span data-stu-id="2965a-128">America/Denver</span></span>

<span data-ttu-id="2965a-129">美洲/危地马拉</span><span class="sxs-lookup"><span data-stu-id="2965a-129">America/Guatemala</span></span>

<span data-ttu-id="2965a-130">美洲/芝加哥</span><span class="sxs-lookup"><span data-stu-id="2965a-130">America/Chicago</span></span>

<span data-ttu-id="2965a-131">美洲/墨西哥城</span><span class="sxs-lookup"><span data-stu-id="2965a-131">America/Mexico_City</span></span>

<span data-ttu-id="2965a-132">美洲/里贾纳</span><span class="sxs-lookup"><span data-stu-id="2965a-132">America/Regina</span></span>

<span data-ttu-id="2965a-133">美洲/波哥大</span><span class="sxs-lookup"><span data-stu-id="2965a-133">America/Bogota</span></span>

<span data-ttu-id="2965a-134">美洲/纽约</span><span class="sxs-lookup"><span data-stu-id="2965a-134">America/New_York</span></span>

<span data-ttu-id="2965a-135">美洲/印第安纳/印第安纳波利斯</span><span class="sxs-lookup"><span data-stu-id="2965a-135">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="2965a-136">美洲/加拉加斯</span><span class="sxs-lookup"><span data-stu-id="2965a-136">America/Caracas</span></span>

<span data-ttu-id="2965a-137">美洲/亚松森</span><span class="sxs-lookup"><span data-stu-id="2965a-137">America/Asuncion</span></span>

<span data-ttu-id="2965a-138">美洲/哈利法克斯</span><span class="sxs-lookup"><span data-stu-id="2965a-138">America/Halifax</span></span>

<span data-ttu-id="2965a-139">美洲/库亚巴</span><span class="sxs-lookup"><span data-stu-id="2965a-139">America/Cuiaba</span></span>

<span data-ttu-id="2965a-140">美洲/拉巴斯</span><span class="sxs-lookup"><span data-stu-id="2965a-140">America/La_Paz</span></span>

<span data-ttu-id="2965a-141">美洲/圣地亚哥</span><span class="sxs-lookup"><span data-stu-id="2965a-141">America/Santiago</span></span>

<span data-ttu-id="2965a-142">美洲/圣约翰斯</span><span class="sxs-lookup"><span data-stu-id="2965a-142">America/St_Johns</span></span>

<span data-ttu-id="2965a-143">美洲/圣保罗</span><span class="sxs-lookup"><span data-stu-id="2965a-143">America/Sao_Paulo</span></span>

<span data-ttu-id="2965a-144">美洲/阿根廷/布宜诺斯艾利斯</span><span class="sxs-lookup"><span data-stu-id="2965a-144">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="2965a-145">美洲/卡宴</span><span class="sxs-lookup"><span data-stu-id="2965a-145">America/Cayenne</span></span>

<span data-ttu-id="2965a-146">美洲/戈特霍布</span><span class="sxs-lookup"><span data-stu-id="2965a-146">America/Godthab</span></span>

<span data-ttu-id="2965a-147">美洲/蒙得维的亚</span><span class="sxs-lookup"><span data-stu-id="2965a-147">America/Montevideo</span></span>

<span data-ttu-id="2965a-148">美洲/巴伊亚</span><span class="sxs-lookup"><span data-stu-id="2965a-148">America/Bahia</span></span>

<span data-ttu-id="2965a-149">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="2965a-149">Etc/GMT+2</span></span>

<span data-ttu-id="2965a-150">大西洋/亚速尔群岛</span><span class="sxs-lookup"><span data-stu-id="2965a-150">Atlantic/Azores</span></span>

<span data-ttu-id="2965a-151">大西洋/佛得角</span><span class="sxs-lookup"><span data-stu-id="2965a-151">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="2965a-152">非洲/卡萨布兰卡</span><span class="sxs-lookup"><span data-stu-id="2965a-152">Africa/Casablanca</span></span>

<span data-ttu-id="2965a-153">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="2965a-153">Etc/GMT</span></span>

<span data-ttu-id="2965a-154">欧洲/伦敦</span><span class="sxs-lookup"><span data-stu-id="2965a-154">Europe/London</span></span>

<span data-ttu-id="2965a-155">大西洋/雷克雅未克</span><span class="sxs-lookup"><span data-stu-id="2965a-155">Atlantic/Reykjavik</span></span>

<span data-ttu-id="2965a-156">欧洲/柏林</span><span class="sxs-lookup"><span data-stu-id="2965a-156">Europe/Berlin</span></span>

<span data-ttu-id="2965a-157">欧洲/布达佩斯</span><span class="sxs-lookup"><span data-stu-id="2965a-157">Europe/Budapest</span></span>

<span data-ttu-id="2965a-158">欧洲/巴黎</span><span class="sxs-lookup"><span data-stu-id="2965a-158">Europe/Paris</span></span>

<span data-ttu-id="2965a-159">欧洲/华沙</span><span class="sxs-lookup"><span data-stu-id="2965a-159">Europe/Warsaw</span></span>

<span data-ttu-id="2965a-160">非洲/拉各斯</span><span class="sxs-lookup"><span data-stu-id="2965a-160">Africa/Lagos</span></span>

<span data-ttu-id="2965a-161">非洲/温得和克</span><span class="sxs-lookup"><span data-stu-id="2965a-161">Africa/Windhoek</span></span>

<span data-ttu-id="2965a-162">欧洲/布加勒斯特</span><span class="sxs-lookup"><span data-stu-id="2965a-162">Europe/Bucharest</span></span>

<span data-ttu-id="2965a-163">亚洲/贝鲁特</span><span class="sxs-lookup"><span data-stu-id="2965a-163">Asia/Beirut</span></span>

<span data-ttu-id="2965a-164">非洲/开罗</span><span class="sxs-lookup"><span data-stu-id="2965a-164">Africa/Cairo</span></span>

<span data-ttu-id="2965a-165">亚洲/大马士革</span><span class="sxs-lookup"><span data-stu-id="2965a-165">Asia/Damascus</span></span>

<span data-ttu-id="2965a-166">非洲/约翰内斯堡</span><span class="sxs-lookup"><span data-stu-id="2965a-166">Africa/Johannesburg</span></span>

<span data-ttu-id="2965a-167">欧洲/基辅</span><span class="sxs-lookup"><span data-stu-id="2965a-167">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="2965a-168">欧洲/伊斯坦布尔</span><span class="sxs-lookup"><span data-stu-id="2965a-168">Europe/Istanbul</span></span>

<span data-ttu-id="2965a-169">亚洲/耶路撒冷</span><span class="sxs-lookup"><span data-stu-id="2965a-169">Asia/Jerusalem</span></span>

<span data-ttu-id="2965a-170">亚洲/安曼</span><span class="sxs-lookup"><span data-stu-id="2965a-170">Asia/Amman</span></span>

<span data-ttu-id="2965a-171">亚洲/巴格达</span><span class="sxs-lookup"><span data-stu-id="2965a-171">Asia/Baghdad</span></span>

<span data-ttu-id="2965a-172">欧洲/加里宁格勒</span><span class="sxs-lookup"><span data-stu-id="2965a-172">Europe/Kaliningrad</span></span>

<span data-ttu-id="2965a-173">亚洲/利雅得</span><span class="sxs-lookup"><span data-stu-id="2965a-173">Asia/Riyadh</span></span>

<span data-ttu-id="2965a-174">非洲/内罗毕</span><span class="sxs-lookup"><span data-stu-id="2965a-174">Africa/Nairobi</span></span>

<span data-ttu-id="2965a-175">亚洲/德黑兰</span><span class="sxs-lookup"><span data-stu-id="2965a-175">Asia/Tehran</span></span>

<span data-ttu-id="2965a-176">亚洲/迪拜</span><span class="sxs-lookup"><span data-stu-id="2965a-176">Asia/Dubai</span></span>

<span data-ttu-id="2965a-177">亚洲/巴库</span><span class="sxs-lookup"><span data-stu-id="2965a-177">Asia/Baku</span></span>

<span data-ttu-id="2965a-178">欧洲/莫斯科</span><span class="sxs-lookup"><span data-stu-id="2965a-178">Europe/Moscow</span></span>

<span data-ttu-id="2965a-179">印度洋/毛里求斯</span><span class="sxs-lookup"><span data-stu-id="2965a-179">Indian/Mauritius</span></span>

<span data-ttu-id="2965a-180">亚洲/第比利斯</span><span class="sxs-lookup"><span data-stu-id="2965a-180">Asia/Tbilisi</span></span>

<span data-ttu-id="2965a-181">亚洲/埃里温</span><span class="sxs-lookup"><span data-stu-id="2965a-181">Asia/Yerevan</span></span>

<span data-ttu-id="2965a-182">亚洲/喀布尔</span><span class="sxs-lookup"><span data-stu-id="2965a-182">Asia/Kabul</span></span>

<span data-ttu-id="2965a-183">亚洲/卡拉奇</span><span class="sxs-lookup"><span data-stu-id="2965a-183">Asia/Karachi</span></span>

<span data-ttu-id="2965a-184">亚洲/塔什干</span><span class="sxs-lookup"><span data-stu-id="2965a-184">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="2965a-185">亚洲/加尔各答</span><span class="sxs-lookup"><span data-stu-id="2965a-185">Asia/Kolkata</span></span>

<span data-ttu-id="2965a-186">亚洲/科伦坡</span><span class="sxs-lookup"><span data-stu-id="2965a-186">Asia/Colombo</span></span>

<span data-ttu-id="2965a-187">亚洲/加德满都</span><span class="sxs-lookup"><span data-stu-id="2965a-187">Asia/Kathmandu</span></span>

<span data-ttu-id="2965a-188">亚洲/阿斯塔纳（阿拉木图）</span><span class="sxs-lookup"><span data-stu-id="2965a-188">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="2965a-189">亚洲/达卡</span><span class="sxs-lookup"><span data-stu-id="2965a-189">Asia/Dhaka</span></span>

<span data-ttu-id="2965a-190">亚洲/叶卡捷琳堡</span><span class="sxs-lookup"><span data-stu-id="2965a-190">Asia/Yekaterinburg</span></span>

<span data-ttu-id="2965a-191">亚洲/仰光</span><span class="sxs-lookup"><span data-stu-id="2965a-191">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="2965a-192">亚洲/曼谷</span><span class="sxs-lookup"><span data-stu-id="2965a-192">Asia/Bangkok</span></span>

<span data-ttu-id="2965a-193">亚洲/新西伯利亚</span><span class="sxs-lookup"><span data-stu-id="2965a-193">Asia/Novosibirsk</span></span>

<span data-ttu-id="2965a-194">亚洲/上海</span><span class="sxs-lookup"><span data-stu-id="2965a-194">Asia/Shanghai</span></span>

<span data-ttu-id="2965a-195">亚洲/克拉斯诺亚尔斯克</span><span class="sxs-lookup"><span data-stu-id="2965a-195">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="2965a-196">亚洲/新加坡</span><span class="sxs-lookup"><span data-stu-id="2965a-196">Asia/Singapore</span></span>

<span data-ttu-id="2965a-197">澳大利亚/珀斯</span><span class="sxs-lookup"><span data-stu-id="2965a-197">Australia/Perth</span></span>

<span data-ttu-id="2965a-198">亚洲/台北</span><span class="sxs-lookup"><span data-stu-id="2965a-198">Asia/Taipei</span></span>

<span data-ttu-id="2965a-199">亚洲/乌兰巴托</span><span class="sxs-lookup"><span data-stu-id="2965a-199">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="2965a-200">亚洲/伊尔库茨克</span><span class="sxs-lookup"><span data-stu-id="2965a-200">Asia/Irkutsk</span></span>

<span data-ttu-id="2965a-201">亚洲/东京</span><span class="sxs-lookup"><span data-stu-id="2965a-201">Asia/Tokyo</span></span>

<span data-ttu-id="2965a-202">亚洲/首尔</span><span class="sxs-lookup"><span data-stu-id="2965a-202">Asia/Seoul</span></span>

<span data-ttu-id="2965a-203">澳洲/阿德莱德</span><span class="sxs-lookup"><span data-stu-id="2965a-203">Australia/Adelaide</span></span>

<span data-ttu-id="2965a-204">澳洲/达尔文</span><span class="sxs-lookup"><span data-stu-id="2965a-204">Australia/Darwin</span></span>

<span data-ttu-id="2965a-205">澳洲/布里斯班</span><span class="sxs-lookup"><span data-stu-id="2965a-205">Australia/Brisbane</span></span>

<span data-ttu-id="2965a-206">澳洲/悉尼</span><span class="sxs-lookup"><span data-stu-id="2965a-206">Australia/Sydney</span></span>

<span data-ttu-id="2965a-207">太平洋/莫尔斯比港</span><span class="sxs-lookup"><span data-stu-id="2965a-207">Pacific/Port_Moresby</span></span>

<span data-ttu-id="2965a-208">澳洲/霍巴特</span><span class="sxs-lookup"><span data-stu-id="2965a-208">Australia/Hobart</span></span>

<span data-ttu-id="2965a-209">亚洲/雅库茨克</span><span class="sxs-lookup"><span data-stu-id="2965a-209">Asia/Yakutsk</span></span>

<span data-ttu-id="2965a-210">太平洋/瓜达尔卡纳尔</span><span class="sxs-lookup"><span data-stu-id="2965a-210">Pacific/Guadalcanal</span></span>

<span data-ttu-id="2965a-211">亚洲/符拉迪沃斯托克</span><span class="sxs-lookup"><span data-stu-id="2965a-211">Asia/Vladivostok</span></span>

<span data-ttu-id="2965a-212">太平洋/奥克兰</span><span class="sxs-lookup"><span data-stu-id="2965a-212">Pacific/Auckland</span></span>

<span data-ttu-id="2965a-213">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="2965a-213">Etc/GMT-12</span></span>

<span data-ttu-id="2965a-214">太平洋/斐济</span><span class="sxs-lookup"><span data-stu-id="2965a-214">Pacific/Fiji</span></span>

<span data-ttu-id="2965a-215">亚洲/马加丹</span><span class="sxs-lookup"><span data-stu-id="2965a-215">Asia/Magadan</span></span>

<span data-ttu-id="2965a-216">太平洋/汤加塔布</span><span class="sxs-lookup"><span data-stu-id="2965a-216">Pacific/Tongatapu</span></span>

<span data-ttu-id="2965a-217">太平洋/阿皮亚</span><span class="sxs-lookup"><span data-stu-id="2965a-217">Pacific/Apia</span></span>

<span data-ttu-id="2965a-218">太平洋/圣诞岛</span><span class="sxs-lookup"><span data-stu-id="2965a-218">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="2965a-219">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2965a-219">JSON representation</span></span>

<span data-ttu-id="2965a-220">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2965a-220">Here is a JSON representation of the resource</span></span>

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
