---
title: dateTimeTimeZone 资源类型
description: 介绍某个时间点的日期、时间和时区。
ms.openlocfilehash: a95ebf35d6a47b8b39c34cab8d6d35b92eaae2c3
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/29/2018
ms.locfileid: "27044000"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="6a2e2-103">dateTimeTimeZone 资源类型</span><span class="sxs-lookup"><span data-stu-id="6a2e2-103">dateTimeTimeZone resource type</span></span>

> <span data-ttu-id="6a2e2-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="6a2e2-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6a2e2-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="6a2e2-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6a2e2-106">介绍某个时间点的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="6a2e2-106">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="6a2e2-107">属性</span><span class="sxs-lookup"><span data-stu-id="6a2e2-107">Properties</span></span>
| <span data-ttu-id="6a2e2-108">属性</span><span class="sxs-lookup"><span data-stu-id="6a2e2-108">Property</span></span>     | <span data-ttu-id="6a2e2-109">类型</span><span class="sxs-lookup"><span data-stu-id="6a2e2-109">Type</span></span>   |<span data-ttu-id="6a2e2-110">说明</span><span class="sxs-lookup"><span data-stu-id="6a2e2-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6a2e2-111">DateTime</span><span class="sxs-lookup"><span data-stu-id="6a2e2-111">DateTime</span></span>|<span data-ttu-id="6a2e2-112">String</span><span class="sxs-lookup"><span data-stu-id="6a2e2-112">String</span></span>|<span data-ttu-id="6a2e2-113">日期和时间组合表示形式的单个时间点 (`<date>T<time>`)。</span><span class="sxs-lookup"><span data-stu-id="6a2e2-113">A single point of time in a combined date and time representation (`<date>T<time>`).</span></span>|
|<span data-ttu-id="6a2e2-114">TimeZone</span><span class="sxs-lookup"><span data-stu-id="6a2e2-114">TimeZone</span></span>|<span data-ttu-id="6a2e2-115">String</span><span class="sxs-lookup"><span data-stu-id="6a2e2-115">String</span></span>|<span data-ttu-id="6a2e2-116">以下时区名称之一。</span><span class="sxs-lookup"><span data-stu-id="6a2e2-116">One of the following time zone names.</span></span>|

<span data-ttu-id="6a2e2-117">_TimeZone_ 属性可以设置为 Windows 支持的任意时区，以及以下时区名称。</span><span class="sxs-lookup"><span data-stu-id="6a2e2-117">The _TimeZone_ property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="6a2e2-118">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="6a2e2-118">Etc/GMT+12</span></span>

<span data-ttu-id="6a2e2-119">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="6a2e2-119">Etc/GMT+11</span></span>

<span data-ttu-id="6a2e2-120">太平洋/火奴鲁鲁</span><span class="sxs-lookup"><span data-stu-id="6a2e2-120">Pacific/Honolulu</span></span>

<span data-ttu-id="6a2e2-121">美洲/安克雷奇</span><span class="sxs-lookup"><span data-stu-id="6a2e2-121">America/Anchorage</span></span>

<span data-ttu-id="6a2e2-122">美洲/圣伊莎贝尔</span><span class="sxs-lookup"><span data-stu-id="6a2e2-122">America/Santa_Isabel</span></span>

<span data-ttu-id="6a2e2-123">美洲/洛杉矶</span><span class="sxs-lookup"><span data-stu-id="6a2e2-123">America/Los_Angeles</span></span>

<span data-ttu-id="6a2e2-124">美洲/菲尼克斯</span><span class="sxs-lookup"><span data-stu-id="6a2e2-124">America/Phoenix</span></span>

<span data-ttu-id="6a2e2-125">美洲/奇瓦瓦</span><span class="sxs-lookup"><span data-stu-id="6a2e2-125">America/Chihuahua</span></span>

<span data-ttu-id="6a2e2-126">美洲/丹佛</span><span class="sxs-lookup"><span data-stu-id="6a2e2-126">America/Denver</span></span>

<span data-ttu-id="6a2e2-127">美洲/危地马拉</span><span class="sxs-lookup"><span data-stu-id="6a2e2-127">America/Guatemala</span></span>

<span data-ttu-id="6a2e2-128">美洲/芝加哥</span><span class="sxs-lookup"><span data-stu-id="6a2e2-128">America/Chicago</span></span>

<span data-ttu-id="6a2e2-129">美洲/墨西哥城</span><span class="sxs-lookup"><span data-stu-id="6a2e2-129">America/Mexico_City</span></span>

<span data-ttu-id="6a2e2-130">美洲/里贾纳</span><span class="sxs-lookup"><span data-stu-id="6a2e2-130">America/Regina</span></span>

<span data-ttu-id="6a2e2-131">美洲/波哥大</span><span class="sxs-lookup"><span data-stu-id="6a2e2-131">America/Bogota</span></span>

<span data-ttu-id="6a2e2-132">美洲/纽约</span><span class="sxs-lookup"><span data-stu-id="6a2e2-132">America/New_York</span></span>

<span data-ttu-id="6a2e2-133">美洲/印第安纳/印第安纳波利斯</span><span class="sxs-lookup"><span data-stu-id="6a2e2-133">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="6a2e2-134">美洲/加拉加斯</span><span class="sxs-lookup"><span data-stu-id="6a2e2-134">America/Caracas</span></span>

<span data-ttu-id="6a2e2-135">美洲/亚松森</span><span class="sxs-lookup"><span data-stu-id="6a2e2-135">America/Asuncion</span></span>

<span data-ttu-id="6a2e2-136">美洲/哈利法克斯</span><span class="sxs-lookup"><span data-stu-id="6a2e2-136">America/Halifax</span></span>

<span data-ttu-id="6a2e2-137">美洲/库亚巴</span><span class="sxs-lookup"><span data-stu-id="6a2e2-137">America/Cuiaba</span></span>

<span data-ttu-id="6a2e2-138">美洲/拉巴斯</span><span class="sxs-lookup"><span data-stu-id="6a2e2-138">America/La_Paz</span></span>

<span data-ttu-id="6a2e2-139">美洲/圣地亚哥</span><span class="sxs-lookup"><span data-stu-id="6a2e2-139">America/Santiago</span></span>

<span data-ttu-id="6a2e2-140">美洲/圣约翰斯</span><span class="sxs-lookup"><span data-stu-id="6a2e2-140">America/St_Johns</span></span>

<span data-ttu-id="6a2e2-141">美洲/圣保罗</span><span class="sxs-lookup"><span data-stu-id="6a2e2-141">America/Sao_Paulo</span></span>

<span data-ttu-id="6a2e2-142">美洲/阿根廷/布宜诺斯艾利斯</span><span class="sxs-lookup"><span data-stu-id="6a2e2-142">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="6a2e2-143">美洲/卡宴</span><span class="sxs-lookup"><span data-stu-id="6a2e2-143">America/Cayenne</span></span>

<span data-ttu-id="6a2e2-144">美洲/戈特霍布</span><span class="sxs-lookup"><span data-stu-id="6a2e2-144">America/Godthab</span></span>

<span data-ttu-id="6a2e2-145">美洲/蒙得维的亚</span><span class="sxs-lookup"><span data-stu-id="6a2e2-145">America/Montevideo</span></span>

<span data-ttu-id="6a2e2-146">美洲/巴伊亚</span><span class="sxs-lookup"><span data-stu-id="6a2e2-146">America/Bahia</span></span>

<span data-ttu-id="6a2e2-147">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="6a2e2-147">Etc/GMT+2</span></span>

<span data-ttu-id="6a2e2-148">大西洋/亚速尔群岛</span><span class="sxs-lookup"><span data-stu-id="6a2e2-148">Atlantic/Azores</span></span>

<span data-ttu-id="6a2e2-149">大西洋/佛得角</span><span class="sxs-lookup"><span data-stu-id="6a2e2-149">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="6a2e2-150">非洲/卡萨布兰卡</span><span class="sxs-lookup"><span data-stu-id="6a2e2-150">Africa/Casablanca</span></span>

<span data-ttu-id="6a2e2-151">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="6a2e2-151">Etc/GMT</span></span>

<span data-ttu-id="6a2e2-152">欧洲/伦敦</span><span class="sxs-lookup"><span data-stu-id="6a2e2-152">Europe/London</span></span>

<span data-ttu-id="6a2e2-153">大西洋/雷克雅未克</span><span class="sxs-lookup"><span data-stu-id="6a2e2-153">Atlantic/Reykjavik</span></span>

<span data-ttu-id="6a2e2-154">欧洲/柏林</span><span class="sxs-lookup"><span data-stu-id="6a2e2-154">Europe/Berlin</span></span>

<span data-ttu-id="6a2e2-155">欧洲/布达佩斯</span><span class="sxs-lookup"><span data-stu-id="6a2e2-155">Europe/Budapest</span></span>

<span data-ttu-id="6a2e2-156">欧洲/巴黎</span><span class="sxs-lookup"><span data-stu-id="6a2e2-156">Europe/Paris</span></span>

<span data-ttu-id="6a2e2-157">欧洲/华沙</span><span class="sxs-lookup"><span data-stu-id="6a2e2-157">Europe/Warsaw</span></span>

<span data-ttu-id="6a2e2-158">非洲/拉各斯</span><span class="sxs-lookup"><span data-stu-id="6a2e2-158">Africa/Lagos</span></span>

<span data-ttu-id="6a2e2-159">非洲/温得和克</span><span class="sxs-lookup"><span data-stu-id="6a2e2-159">Africa/Windhoek</span></span>

<span data-ttu-id="6a2e2-160">欧洲/布加勒斯特</span><span class="sxs-lookup"><span data-stu-id="6a2e2-160">Europe/Bucharest</span></span>

<span data-ttu-id="6a2e2-161">亚洲/贝鲁特</span><span class="sxs-lookup"><span data-stu-id="6a2e2-161">Asia/Beirut</span></span>

<span data-ttu-id="6a2e2-162">非洲/开罗</span><span class="sxs-lookup"><span data-stu-id="6a2e2-162">Africa/Cairo</span></span>

<span data-ttu-id="6a2e2-163">亚洲/大马士革</span><span class="sxs-lookup"><span data-stu-id="6a2e2-163">Asia/Damascus</span></span>

<span data-ttu-id="6a2e2-164">非洲/约翰内斯堡</span><span class="sxs-lookup"><span data-stu-id="6a2e2-164">Africa/Johannesburg</span></span>

<span data-ttu-id="6a2e2-165">欧洲/基辅</span><span class="sxs-lookup"><span data-stu-id="6a2e2-165">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="6a2e2-166">欧洲/伊斯坦布尔</span><span class="sxs-lookup"><span data-stu-id="6a2e2-166">Europe/Istanbul</span></span>

<span data-ttu-id="6a2e2-167">亚洲/耶路撒冷</span><span class="sxs-lookup"><span data-stu-id="6a2e2-167">Asia/Jerusalem</span></span>

<span data-ttu-id="6a2e2-168">亚洲/安曼</span><span class="sxs-lookup"><span data-stu-id="6a2e2-168">Asia/Amman</span></span>

<span data-ttu-id="6a2e2-169">亚洲/巴格达</span><span class="sxs-lookup"><span data-stu-id="6a2e2-169">Asia/Baghdad</span></span>

<span data-ttu-id="6a2e2-170">欧洲/加里宁格勒</span><span class="sxs-lookup"><span data-stu-id="6a2e2-170">Europe/Kaliningrad</span></span>

<span data-ttu-id="6a2e2-171">亚洲/利雅得</span><span class="sxs-lookup"><span data-stu-id="6a2e2-171">Asia/Riyadh</span></span>

<span data-ttu-id="6a2e2-172">非洲/内罗毕</span><span class="sxs-lookup"><span data-stu-id="6a2e2-172">Africa/Nairobi</span></span>

<span data-ttu-id="6a2e2-173">亚洲/德黑兰</span><span class="sxs-lookup"><span data-stu-id="6a2e2-173">Asia/Tehran</span></span>

<span data-ttu-id="6a2e2-174">亚洲/迪拜</span><span class="sxs-lookup"><span data-stu-id="6a2e2-174">Asia/Dubai</span></span>

<span data-ttu-id="6a2e2-175">亚洲/巴库</span><span class="sxs-lookup"><span data-stu-id="6a2e2-175">Asia/Baku</span></span>

<span data-ttu-id="6a2e2-176">欧洲/莫斯科</span><span class="sxs-lookup"><span data-stu-id="6a2e2-176">Europe/Moscow</span></span>

<span data-ttu-id="6a2e2-177">印度洋/毛里求斯</span><span class="sxs-lookup"><span data-stu-id="6a2e2-177">Indian/Mauritius</span></span>

<span data-ttu-id="6a2e2-178">亚洲/第比利斯</span><span class="sxs-lookup"><span data-stu-id="6a2e2-178">Asia/Tbilisi</span></span>

<span data-ttu-id="6a2e2-179">亚洲/埃里温</span><span class="sxs-lookup"><span data-stu-id="6a2e2-179">Asia/Yerevan</span></span>

<span data-ttu-id="6a2e2-180">亚洲/喀布尔</span><span class="sxs-lookup"><span data-stu-id="6a2e2-180">Asia/Kabul</span></span>

<span data-ttu-id="6a2e2-181">亚洲/卡拉奇</span><span class="sxs-lookup"><span data-stu-id="6a2e2-181">Asia/Karachi</span></span>

<span data-ttu-id="6a2e2-182">亚洲/塔什干</span><span class="sxs-lookup"><span data-stu-id="6a2e2-182">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="6a2e2-183">亚洲/加尔各答</span><span class="sxs-lookup"><span data-stu-id="6a2e2-183">Asia/Kolkata</span></span>

<span data-ttu-id="6a2e2-184">亚洲/科伦坡</span><span class="sxs-lookup"><span data-stu-id="6a2e2-184">Asia/Colombo</span></span>

<span data-ttu-id="6a2e2-185">亚洲/加德满都</span><span class="sxs-lookup"><span data-stu-id="6a2e2-185">Asia/Kathmandu</span></span>

<span data-ttu-id="6a2e2-186">亚洲/阿斯塔纳（阿拉木图）</span><span class="sxs-lookup"><span data-stu-id="6a2e2-186">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="6a2e2-187">亚洲/达卡</span><span class="sxs-lookup"><span data-stu-id="6a2e2-187">Asia/Dhaka</span></span>

<span data-ttu-id="6a2e2-188">亚洲/叶卡捷琳堡</span><span class="sxs-lookup"><span data-stu-id="6a2e2-188">Asia/Yekaterinburg</span></span>

<span data-ttu-id="6a2e2-189">亚洲/仰光</span><span class="sxs-lookup"><span data-stu-id="6a2e2-189">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="6a2e2-190">亚洲/曼谷</span><span class="sxs-lookup"><span data-stu-id="6a2e2-190">Asia/Bangkok</span></span>

<span data-ttu-id="6a2e2-191">亚洲/新西伯利亚</span><span class="sxs-lookup"><span data-stu-id="6a2e2-191">Asia/Novosibirsk</span></span>

<span data-ttu-id="6a2e2-192">亚洲/上海</span><span class="sxs-lookup"><span data-stu-id="6a2e2-192">Asia/Shanghai</span></span>

<span data-ttu-id="6a2e2-193">亚洲/克拉斯诺亚尔斯克</span><span class="sxs-lookup"><span data-stu-id="6a2e2-193">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="6a2e2-194">亚洲/新加坡</span><span class="sxs-lookup"><span data-stu-id="6a2e2-194">Asia/Singapore</span></span>

<span data-ttu-id="6a2e2-195">澳大利亚/珀斯</span><span class="sxs-lookup"><span data-stu-id="6a2e2-195">Australia/Perth</span></span>

<span data-ttu-id="6a2e2-196">亚洲/台北</span><span class="sxs-lookup"><span data-stu-id="6a2e2-196">Asia/Taipei</span></span>

<span data-ttu-id="6a2e2-197">亚洲/乌兰巴托</span><span class="sxs-lookup"><span data-stu-id="6a2e2-197">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="6a2e2-198">亚洲/伊尔库茨克</span><span class="sxs-lookup"><span data-stu-id="6a2e2-198">Asia/Irkutsk</span></span>

<span data-ttu-id="6a2e2-199">亚洲/东京</span><span class="sxs-lookup"><span data-stu-id="6a2e2-199">Asia/Tokyo</span></span>

<span data-ttu-id="6a2e2-200">亚洲/首尔</span><span class="sxs-lookup"><span data-stu-id="6a2e2-200">Asia/Seoul</span></span>

<span data-ttu-id="6a2e2-201">澳洲/阿德莱德</span><span class="sxs-lookup"><span data-stu-id="6a2e2-201">Australia/Adelaide</span></span>

<span data-ttu-id="6a2e2-202">澳洲/达尔文</span><span class="sxs-lookup"><span data-stu-id="6a2e2-202">Australia/Darwin</span></span>

<span data-ttu-id="6a2e2-203">澳洲/布里斯班</span><span class="sxs-lookup"><span data-stu-id="6a2e2-203">Australia/Brisbane</span></span>

<span data-ttu-id="6a2e2-204">澳洲/悉尼</span><span class="sxs-lookup"><span data-stu-id="6a2e2-204">Australia/Sydney</span></span>

<span data-ttu-id="6a2e2-205">太平洋/莫尔斯比港</span><span class="sxs-lookup"><span data-stu-id="6a2e2-205">Pacific/Port_Moresby</span></span>

<span data-ttu-id="6a2e2-206">澳洲/霍巴特</span><span class="sxs-lookup"><span data-stu-id="6a2e2-206">Australia/Hobart</span></span>

<span data-ttu-id="6a2e2-207">亚洲/雅库茨克</span><span class="sxs-lookup"><span data-stu-id="6a2e2-207">Asia/Yakutsk</span></span>

<span data-ttu-id="6a2e2-208">太平洋/瓜达尔卡纳尔</span><span class="sxs-lookup"><span data-stu-id="6a2e2-208">Pacific/Guadalcanal</span></span>

<span data-ttu-id="6a2e2-209">亚洲/符拉迪沃斯托克</span><span class="sxs-lookup"><span data-stu-id="6a2e2-209">Asia/Vladivostok</span></span>

<span data-ttu-id="6a2e2-210">太平洋/奥克兰</span><span class="sxs-lookup"><span data-stu-id="6a2e2-210">Pacific/Auckland</span></span>

<span data-ttu-id="6a2e2-211">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="6a2e2-211">Etc/GMT-12</span></span>

<span data-ttu-id="6a2e2-212">太平洋/斐济</span><span class="sxs-lookup"><span data-stu-id="6a2e2-212">Pacific/Fiji</span></span>

<span data-ttu-id="6a2e2-213">亚洲/马加丹</span><span class="sxs-lookup"><span data-stu-id="6a2e2-213">Asia/Magadan</span></span>

<span data-ttu-id="6a2e2-214">太平洋/汤加塔布</span><span class="sxs-lookup"><span data-stu-id="6a2e2-214">Pacific/Tongatapu</span></span>

<span data-ttu-id="6a2e2-215">太平洋/阿皮亚</span><span class="sxs-lookup"><span data-stu-id="6a2e2-215">Pacific/Apia</span></span>

<span data-ttu-id="6a2e2-216">太平洋/圣诞岛</span><span class="sxs-lookup"><span data-stu-id="6a2e2-216">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="6a2e2-217">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="6a2e2-217">JSON representation</span></span>

<span data-ttu-id="6a2e2-218">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="6a2e2-218">Here is a JSON representation of the resource</span></span>

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
