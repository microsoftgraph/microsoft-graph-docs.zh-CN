---
title: dateTimeTimeZone 资源类型
description: 介绍某个时间点的日期、时间和时区。
localization_priority: Normal
doc_type: resourcePageType
author: harini84
ms.prod: outlook
ms.openlocfilehash: e7f283cc98406564a7c58a525a689b54e043a333
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48049966"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="d650b-103">dateTimeTimeZone 资源类型</span><span class="sxs-lookup"><span data-stu-id="d650b-103">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="d650b-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="d650b-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d650b-105">介绍某个时间点的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="d650b-105">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="d650b-106">属性</span><span class="sxs-lookup"><span data-stu-id="d650b-106">Properties</span></span>
| <span data-ttu-id="d650b-107">属性</span><span class="sxs-lookup"><span data-stu-id="d650b-107">Property</span></span>     | <span data-ttu-id="d650b-108">类型</span><span class="sxs-lookup"><span data-stu-id="d650b-108">Type</span></span>   |<span data-ttu-id="d650b-109">说明</span><span class="sxs-lookup"><span data-stu-id="d650b-109">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="d650b-110">dateTime</span><span class="sxs-lookup"><span data-stu-id="d650b-110">dateTime</span></span>|<span data-ttu-id="d650b-111">字符串</span><span class="sxs-lookup"><span data-stu-id="d650b-111">String</span></span>|<span data-ttu-id="d650b-112">日期和时间组合表示形式的单个时间点 (`{date}T{time}`)。</span><span class="sxs-lookup"><span data-stu-id="d650b-112">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span> <span data-ttu-id="d650b-113">例如，"2019-04-16T09：00： 00"。</span><span class="sxs-lookup"><span data-stu-id="d650b-113">For example, "2019-04-16T09:00:00".</span></span>|
|<span data-ttu-id="d650b-114">timeZone</span><span class="sxs-lookup"><span data-stu-id="d650b-114">timeZone</span></span>|<span data-ttu-id="d650b-115">String</span><span class="sxs-lookup"><span data-stu-id="d650b-115">String</span></span>|<span data-ttu-id="d650b-116">表示时区，例如“太平洋标准时间”。</span><span class="sxs-lookup"><span data-stu-id="d650b-116">Represents a time zone, for example, "Pacific Standard Time".</span></span> <span data-ttu-id="d650b-117">有关可能值，请参阅下文。</span><span class="sxs-lookup"><span data-stu-id="d650b-117">See below for possible values.</span></span>|

<span data-ttu-id="d650b-118">通常，**timeZone** 属性_可以_ 设置为 [Windows 当前支持的任意时区](/windows-hardware/manufacture/desktop/default-time-zones)，以及[日历 API 支持的其他时区](#additional-time-zones)。</span><span class="sxs-lookup"><span data-stu-id="d650b-118">In general, the **timeZone** property _can_ be set to any of the [time zones currently supported by Windows](/windows-hardware/manufacture/desktop/default-time-zones), as well as the additional [time zones supported by the calendar API](#additional-time-zones).</span></span>

<span data-ttu-id="d650b-119">将 **dateTimeTimeZone** 与某一方法（例如[创建](../api/user-post-events.md)或[更新](../api/event-update.md)事件）结合使用时，请注意支持的实际时区，这可能是一个较小的子集。</span><span class="sxs-lookup"><span data-stu-id="d650b-119">When using **dateTimeTimeZone** in conjunction with a method (such as [creating](../api/user-post-events.md) or [updating](../api/event-update.md) an event), take note of the actual time zones supported, which can be a smaller subset.</span></span>

### <a name="additional-time-zones"></a><span data-ttu-id="d650b-120">其他时区</span><span class="sxs-lookup"><span data-stu-id="d650b-120">Additional time zones</span></span>

<span data-ttu-id="d650b-121">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="d650b-121">Etc/GMT+12</span></span>

<span data-ttu-id="d650b-122">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="d650b-122">Etc/GMT+11</span></span>

<span data-ttu-id="d650b-123">太平洋/火奴鲁鲁</span><span class="sxs-lookup"><span data-stu-id="d650b-123">Pacific/Honolulu</span></span>

<span data-ttu-id="d650b-124">美洲/安克雷奇</span><span class="sxs-lookup"><span data-stu-id="d650b-124">America/Anchorage</span></span>

<span data-ttu-id="d650b-125">美洲/圣伊莎贝尔</span><span class="sxs-lookup"><span data-stu-id="d650b-125">America/Santa_Isabel</span></span>

<span data-ttu-id="d650b-126">美洲/洛杉矶</span><span class="sxs-lookup"><span data-stu-id="d650b-126">America/Los_Angeles</span></span>

<span data-ttu-id="d650b-127">美洲/菲尼克斯</span><span class="sxs-lookup"><span data-stu-id="d650b-127">America/Phoenix</span></span>

<span data-ttu-id="d650b-128">美洲/奇瓦瓦</span><span class="sxs-lookup"><span data-stu-id="d650b-128">America/Chihuahua</span></span>

<span data-ttu-id="d650b-129">美洲/丹佛</span><span class="sxs-lookup"><span data-stu-id="d650b-129">America/Denver</span></span>

<span data-ttu-id="d650b-130">美洲/危地马拉</span><span class="sxs-lookup"><span data-stu-id="d650b-130">America/Guatemala</span></span>

<span data-ttu-id="d650b-131">美洲/芝加哥</span><span class="sxs-lookup"><span data-stu-id="d650b-131">America/Chicago</span></span>

<span data-ttu-id="d650b-132">美洲/墨西哥城</span><span class="sxs-lookup"><span data-stu-id="d650b-132">America/Mexico_City</span></span>

<span data-ttu-id="d650b-133">美洲/里贾纳</span><span class="sxs-lookup"><span data-stu-id="d650b-133">America/Regina</span></span>

<span data-ttu-id="d650b-134">美洲/波哥大</span><span class="sxs-lookup"><span data-stu-id="d650b-134">America/Bogota</span></span>

<span data-ttu-id="d650b-135">美洲/纽约</span><span class="sxs-lookup"><span data-stu-id="d650b-135">America/New_York</span></span>

<span data-ttu-id="d650b-136">美洲/印第安纳/印第安纳波利斯</span><span class="sxs-lookup"><span data-stu-id="d650b-136">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="d650b-137">美洲/加拉加斯</span><span class="sxs-lookup"><span data-stu-id="d650b-137">America/Caracas</span></span>

<span data-ttu-id="d650b-138">美洲/亚松森</span><span class="sxs-lookup"><span data-stu-id="d650b-138">America/Asuncion</span></span>

<span data-ttu-id="d650b-139">美洲/哈利法克斯</span><span class="sxs-lookup"><span data-stu-id="d650b-139">America/Halifax</span></span>

<span data-ttu-id="d650b-140">美洲/库亚巴</span><span class="sxs-lookup"><span data-stu-id="d650b-140">America/Cuiaba</span></span>

<span data-ttu-id="d650b-141">美洲/拉巴斯</span><span class="sxs-lookup"><span data-stu-id="d650b-141">America/La_Paz</span></span>

<span data-ttu-id="d650b-142">美洲/圣地亚哥</span><span class="sxs-lookup"><span data-stu-id="d650b-142">America/Santiago</span></span>

<span data-ttu-id="d650b-143">美洲/圣约翰斯</span><span class="sxs-lookup"><span data-stu-id="d650b-143">America/St_Johns</span></span>

<span data-ttu-id="d650b-144">美洲/圣保罗</span><span class="sxs-lookup"><span data-stu-id="d650b-144">America/Sao_Paulo</span></span>

<span data-ttu-id="d650b-145">美洲/阿根廷/布宜诺斯艾利斯</span><span class="sxs-lookup"><span data-stu-id="d650b-145">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="d650b-146">美洲/卡宴</span><span class="sxs-lookup"><span data-stu-id="d650b-146">America/Cayenne</span></span>

<span data-ttu-id="d650b-147">美洲/戈特霍布</span><span class="sxs-lookup"><span data-stu-id="d650b-147">America/Godthab</span></span>

<span data-ttu-id="d650b-148">美洲/蒙得维的亚</span><span class="sxs-lookup"><span data-stu-id="d650b-148">America/Montevideo</span></span>

<span data-ttu-id="d650b-149">美洲/巴伊亚</span><span class="sxs-lookup"><span data-stu-id="d650b-149">America/Bahia</span></span>

<span data-ttu-id="d650b-150">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="d650b-150">Etc/GMT+2</span></span>

<span data-ttu-id="d650b-151">大西洋/亚速尔群岛</span><span class="sxs-lookup"><span data-stu-id="d650b-151">Atlantic/Azores</span></span>

<span data-ttu-id="d650b-152">大西洋/佛得角</span><span class="sxs-lookup"><span data-stu-id="d650b-152">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="d650b-153">非洲/卡萨布兰卡</span><span class="sxs-lookup"><span data-stu-id="d650b-153">Africa/Casablanca</span></span>

<span data-ttu-id="d650b-154">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="d650b-154">Etc/GMT</span></span>

<span data-ttu-id="d650b-155">欧洲/伦敦</span><span class="sxs-lookup"><span data-stu-id="d650b-155">Europe/London</span></span>

<span data-ttu-id="d650b-156">大西洋/雷克雅未克</span><span class="sxs-lookup"><span data-stu-id="d650b-156">Atlantic/Reykjavik</span></span>

<span data-ttu-id="d650b-157">欧洲/柏林</span><span class="sxs-lookup"><span data-stu-id="d650b-157">Europe/Berlin</span></span>

<span data-ttu-id="d650b-158">欧洲/布达佩斯</span><span class="sxs-lookup"><span data-stu-id="d650b-158">Europe/Budapest</span></span>

<span data-ttu-id="d650b-159">欧洲/巴黎</span><span class="sxs-lookup"><span data-stu-id="d650b-159">Europe/Paris</span></span>

<span data-ttu-id="d650b-160">欧洲/华沙</span><span class="sxs-lookup"><span data-stu-id="d650b-160">Europe/Warsaw</span></span>

<span data-ttu-id="d650b-161">非洲/拉各斯</span><span class="sxs-lookup"><span data-stu-id="d650b-161">Africa/Lagos</span></span>

<span data-ttu-id="d650b-162">非洲/温得和克</span><span class="sxs-lookup"><span data-stu-id="d650b-162">Africa/Windhoek</span></span>

<span data-ttu-id="d650b-163">欧洲/布加勒斯特</span><span class="sxs-lookup"><span data-stu-id="d650b-163">Europe/Bucharest</span></span>

<span data-ttu-id="d650b-164">亚洲/贝鲁特</span><span class="sxs-lookup"><span data-stu-id="d650b-164">Asia/Beirut</span></span>

<span data-ttu-id="d650b-165">非洲/开罗</span><span class="sxs-lookup"><span data-stu-id="d650b-165">Africa/Cairo</span></span>

<span data-ttu-id="d650b-166">亚洲/大马士革</span><span class="sxs-lookup"><span data-stu-id="d650b-166">Asia/Damascus</span></span>

<span data-ttu-id="d650b-167">非洲/约翰内斯堡</span><span class="sxs-lookup"><span data-stu-id="d650b-167">Africa/Johannesburg</span></span>

<span data-ttu-id="d650b-168">欧洲/基辅</span><span class="sxs-lookup"><span data-stu-id="d650b-168">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="d650b-169">欧洲/伊斯坦布尔</span><span class="sxs-lookup"><span data-stu-id="d650b-169">Europe/Istanbul</span></span>

<span data-ttu-id="d650b-170">亚洲/耶路撒冷</span><span class="sxs-lookup"><span data-stu-id="d650b-170">Asia/Jerusalem</span></span>

<span data-ttu-id="d650b-171">亚洲/安曼</span><span class="sxs-lookup"><span data-stu-id="d650b-171">Asia/Amman</span></span>

<span data-ttu-id="d650b-172">亚洲/巴格达</span><span class="sxs-lookup"><span data-stu-id="d650b-172">Asia/Baghdad</span></span>

<span data-ttu-id="d650b-173">欧洲/加里宁格勒</span><span class="sxs-lookup"><span data-stu-id="d650b-173">Europe/Kaliningrad</span></span>

<span data-ttu-id="d650b-174">亚洲/利雅得</span><span class="sxs-lookup"><span data-stu-id="d650b-174">Asia/Riyadh</span></span>

<span data-ttu-id="d650b-175">非洲/内罗毕</span><span class="sxs-lookup"><span data-stu-id="d650b-175">Africa/Nairobi</span></span>

<span data-ttu-id="d650b-176">亚洲/德黑兰</span><span class="sxs-lookup"><span data-stu-id="d650b-176">Asia/Tehran</span></span>

<span data-ttu-id="d650b-177">亚洲/迪拜</span><span class="sxs-lookup"><span data-stu-id="d650b-177">Asia/Dubai</span></span>

<span data-ttu-id="d650b-178">亚洲/巴库</span><span class="sxs-lookup"><span data-stu-id="d650b-178">Asia/Baku</span></span>

<span data-ttu-id="d650b-179">欧洲/莫斯科</span><span class="sxs-lookup"><span data-stu-id="d650b-179">Europe/Moscow</span></span>

<span data-ttu-id="d650b-180">印度洋/毛里求斯</span><span class="sxs-lookup"><span data-stu-id="d650b-180">Indian/Mauritius</span></span>

<span data-ttu-id="d650b-181">亚洲/第比利斯</span><span class="sxs-lookup"><span data-stu-id="d650b-181">Asia/Tbilisi</span></span>

<span data-ttu-id="d650b-182">亚洲/埃里温</span><span class="sxs-lookup"><span data-stu-id="d650b-182">Asia/Yerevan</span></span>

<span data-ttu-id="d650b-183">亚洲/喀布尔</span><span class="sxs-lookup"><span data-stu-id="d650b-183">Asia/Kabul</span></span>

<span data-ttu-id="d650b-184">亚洲/卡拉奇</span><span class="sxs-lookup"><span data-stu-id="d650b-184">Asia/Karachi</span></span>

<span data-ttu-id="d650b-185">亚洲/塔什干</span><span class="sxs-lookup"><span data-stu-id="d650b-185">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="d650b-186">亚洲/加尔各答</span><span class="sxs-lookup"><span data-stu-id="d650b-186">Asia/Kolkata</span></span>

<span data-ttu-id="d650b-187">亚洲/科伦坡</span><span class="sxs-lookup"><span data-stu-id="d650b-187">Asia/Colombo</span></span>

<span data-ttu-id="d650b-188">亚洲/加德满都</span><span class="sxs-lookup"><span data-stu-id="d650b-188">Asia/Kathmandu</span></span>

<span data-ttu-id="d650b-189">亚洲/阿斯塔纳（阿拉木图）</span><span class="sxs-lookup"><span data-stu-id="d650b-189">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="d650b-190">亚洲/达卡</span><span class="sxs-lookup"><span data-stu-id="d650b-190">Asia/Dhaka</span></span>

<span data-ttu-id="d650b-191">亚洲/叶卡捷琳堡</span><span class="sxs-lookup"><span data-stu-id="d650b-191">Asia/Yekaterinburg</span></span>

<span data-ttu-id="d650b-192">亚洲/仰光</span><span class="sxs-lookup"><span data-stu-id="d650b-192">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="d650b-193">亚洲/曼谷</span><span class="sxs-lookup"><span data-stu-id="d650b-193">Asia/Bangkok</span></span>

<span data-ttu-id="d650b-194">亚洲/新西伯利亚</span><span class="sxs-lookup"><span data-stu-id="d650b-194">Asia/Novosibirsk</span></span>

<span data-ttu-id="d650b-195">亚洲/上海</span><span class="sxs-lookup"><span data-stu-id="d650b-195">Asia/Shanghai</span></span>

<span data-ttu-id="d650b-196">亚洲/克拉斯诺亚尔斯克</span><span class="sxs-lookup"><span data-stu-id="d650b-196">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="d650b-197">亚洲/新加坡</span><span class="sxs-lookup"><span data-stu-id="d650b-197">Asia/Singapore</span></span>

<span data-ttu-id="d650b-198">澳大利亚/珀斯</span><span class="sxs-lookup"><span data-stu-id="d650b-198">Australia/Perth</span></span>

<span data-ttu-id="d650b-199">亚洲/台北</span><span class="sxs-lookup"><span data-stu-id="d650b-199">Asia/Taipei</span></span>

<span data-ttu-id="d650b-200">亚洲/乌兰巴托</span><span class="sxs-lookup"><span data-stu-id="d650b-200">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="d650b-201">亚洲/伊尔库茨克</span><span class="sxs-lookup"><span data-stu-id="d650b-201">Asia/Irkutsk</span></span>

<span data-ttu-id="d650b-202">亚洲/东京</span><span class="sxs-lookup"><span data-stu-id="d650b-202">Asia/Tokyo</span></span>

<span data-ttu-id="d650b-203">亚洲/首尔</span><span class="sxs-lookup"><span data-stu-id="d650b-203">Asia/Seoul</span></span>

<span data-ttu-id="d650b-204">澳洲/阿德莱德</span><span class="sxs-lookup"><span data-stu-id="d650b-204">Australia/Adelaide</span></span>

<span data-ttu-id="d650b-205">澳洲/达尔文</span><span class="sxs-lookup"><span data-stu-id="d650b-205">Australia/Darwin</span></span>

<span data-ttu-id="d650b-206">澳洲/布里斯班</span><span class="sxs-lookup"><span data-stu-id="d650b-206">Australia/Brisbane</span></span>

<span data-ttu-id="d650b-207">澳洲/悉尼</span><span class="sxs-lookup"><span data-stu-id="d650b-207">Australia/Sydney</span></span>

<span data-ttu-id="d650b-208">太平洋/莫尔斯比港</span><span class="sxs-lookup"><span data-stu-id="d650b-208">Pacific/Port_Moresby</span></span>

<span data-ttu-id="d650b-209">澳洲/霍巴特</span><span class="sxs-lookup"><span data-stu-id="d650b-209">Australia/Hobart</span></span>

<span data-ttu-id="d650b-210">亚洲/雅库茨克</span><span class="sxs-lookup"><span data-stu-id="d650b-210">Asia/Yakutsk</span></span>

<span data-ttu-id="d650b-211">太平洋/瓜达尔卡纳尔</span><span class="sxs-lookup"><span data-stu-id="d650b-211">Pacific/Guadalcanal</span></span>

<span data-ttu-id="d650b-212">亚洲/符拉迪沃斯托克</span><span class="sxs-lookup"><span data-stu-id="d650b-212">Asia/Vladivostok</span></span>

<span data-ttu-id="d650b-213">太平洋/奥克兰</span><span class="sxs-lookup"><span data-stu-id="d650b-213">Pacific/Auckland</span></span>

<span data-ttu-id="d650b-214">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="d650b-214">Etc/GMT-12</span></span>

<span data-ttu-id="d650b-215">太平洋/斐济</span><span class="sxs-lookup"><span data-stu-id="d650b-215">Pacific/Fiji</span></span>

<span data-ttu-id="d650b-216">亚洲/马加丹</span><span class="sxs-lookup"><span data-stu-id="d650b-216">Asia/Magadan</span></span>

<span data-ttu-id="d650b-217">太平洋/汤加塔布</span><span class="sxs-lookup"><span data-stu-id="d650b-217">Pacific/Tongatapu</span></span>

<span data-ttu-id="d650b-218">太平洋/阿皮亚</span><span class="sxs-lookup"><span data-stu-id="d650b-218">Pacific/Apia</span></span>

<span data-ttu-id="d650b-219">太平洋/圣诞岛</span><span class="sxs-lookup"><span data-stu-id="d650b-219">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="d650b-220">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="d650b-220">JSON representation</span></span>

<span data-ttu-id="d650b-221">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="d650b-221">Here is a JSON representation of the resource</span></span>

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
<!--
{
  "type": "#page.annotation",
  "description": "dateTimeTimeZone resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->


