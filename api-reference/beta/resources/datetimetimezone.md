---
title: dateTimeTimeZone 资源类型
description: 介绍某个时间点的日期、时间和时区。
localization_priority: Normal
ms.openlocfilehash: ee5359c0ababad2a4f785d17a02ac5bb618d2681
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32535272"
---
# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="7bb7b-103">dateTimeTimeZone 资源类型</span><span class="sxs-lookup"><span data-stu-id="7bb7b-103">dateTimeTimeZone resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="7bb7b-104">介绍某个时间点的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="7bb7b-104">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="7bb7b-105">属性</span><span class="sxs-lookup"><span data-stu-id="7bb7b-105">Properties</span></span>
| <span data-ttu-id="7bb7b-106">属性</span><span class="sxs-lookup"><span data-stu-id="7bb7b-106">Property</span></span>     | <span data-ttu-id="7bb7b-107">类型</span><span class="sxs-lookup"><span data-stu-id="7bb7b-107">Type</span></span>   |<span data-ttu-id="7bb7b-108">说明</span><span class="sxs-lookup"><span data-stu-id="7bb7b-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="7bb7b-109">dateTime</span><span class="sxs-lookup"><span data-stu-id="7bb7b-109">dateTime</span></span>|<span data-ttu-id="7bb7b-110">String</span><span class="sxs-lookup"><span data-stu-id="7bb7b-110">String</span></span>|<span data-ttu-id="7bb7b-111">日期和时间组合表示形式的单个时间点 (`{date}T{time}`)。</span><span class="sxs-lookup"><span data-stu-id="7bb7b-111">A single point of time in a combined date and time representation (`{date}T{time}`).</span></span> <span data-ttu-id="7bb7b-112">例如, "2019-04-16T09:00:00"。</span><span class="sxs-lookup"><span data-stu-id="7bb7b-112">For example, "2019-04-16T09:00:00".</span></span>|
|<span data-ttu-id="7bb7b-113">timeZone</span><span class="sxs-lookup"><span data-stu-id="7bb7b-113">timeZone</span></span>|<span data-ttu-id="7bb7b-114">字符串</span><span class="sxs-lookup"><span data-stu-id="7bb7b-114">String</span></span>|<span data-ttu-id="7bb7b-115">时区名称, 如下所述。</span><span class="sxs-lookup"><span data-stu-id="7bb7b-115">A time zone name as described below.</span></span>|

<span data-ttu-id="7bb7b-116">可以将**时区**属性设置为 Windows 支持的任意时区, 以及以下时区名称。</span><span class="sxs-lookup"><span data-stu-id="7bb7b-116">The **timeZone** property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="7bb7b-117">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="7bb7b-117">Etc/GMT+12</span></span>

<span data-ttu-id="7bb7b-118">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="7bb7b-118">Etc/GMT+11</span></span>

<span data-ttu-id="7bb7b-119">太平洋/火奴鲁鲁</span><span class="sxs-lookup"><span data-stu-id="7bb7b-119">Pacific/Honolulu</span></span>

<span data-ttu-id="7bb7b-120">美洲/安克雷奇</span><span class="sxs-lookup"><span data-stu-id="7bb7b-120">America/Anchorage</span></span>

<span data-ttu-id="7bb7b-121">美洲/圣伊莎贝尔</span><span class="sxs-lookup"><span data-stu-id="7bb7b-121">America/Santa_Isabel</span></span>

<span data-ttu-id="7bb7b-122">美洲/洛杉矶</span><span class="sxs-lookup"><span data-stu-id="7bb7b-122">America/Los_Angeles</span></span>

<span data-ttu-id="7bb7b-123">美洲/菲尼克斯</span><span class="sxs-lookup"><span data-stu-id="7bb7b-123">America/Phoenix</span></span>

<span data-ttu-id="7bb7b-124">美洲/奇瓦瓦</span><span class="sxs-lookup"><span data-stu-id="7bb7b-124">America/Chihuahua</span></span>

<span data-ttu-id="7bb7b-125">美洲/丹佛</span><span class="sxs-lookup"><span data-stu-id="7bb7b-125">America/Denver</span></span>

<span data-ttu-id="7bb7b-126">美洲/危地马拉</span><span class="sxs-lookup"><span data-stu-id="7bb7b-126">America/Guatemala</span></span>

<span data-ttu-id="7bb7b-127">美洲/芝加哥</span><span class="sxs-lookup"><span data-stu-id="7bb7b-127">America/Chicago</span></span>

<span data-ttu-id="7bb7b-128">美洲/墨西哥城</span><span class="sxs-lookup"><span data-stu-id="7bb7b-128">America/Mexico_City</span></span>

<span data-ttu-id="7bb7b-129">美洲/里贾纳</span><span class="sxs-lookup"><span data-stu-id="7bb7b-129">America/Regina</span></span>

<span data-ttu-id="7bb7b-130">美洲/波哥大</span><span class="sxs-lookup"><span data-stu-id="7bb7b-130">America/Bogota</span></span>

<span data-ttu-id="7bb7b-131">美洲/纽约</span><span class="sxs-lookup"><span data-stu-id="7bb7b-131">America/New_York</span></span>

<span data-ttu-id="7bb7b-132">美洲/印第安纳/印第安纳波利斯</span><span class="sxs-lookup"><span data-stu-id="7bb7b-132">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="7bb7b-133">美洲/加拉加斯</span><span class="sxs-lookup"><span data-stu-id="7bb7b-133">America/Caracas</span></span>

<span data-ttu-id="7bb7b-134">美洲/亚松森</span><span class="sxs-lookup"><span data-stu-id="7bb7b-134">America/Asuncion</span></span>

<span data-ttu-id="7bb7b-135">美洲/哈利法克斯</span><span class="sxs-lookup"><span data-stu-id="7bb7b-135">America/Halifax</span></span>

<span data-ttu-id="7bb7b-136">美洲/库亚巴</span><span class="sxs-lookup"><span data-stu-id="7bb7b-136">America/Cuiaba</span></span>

<span data-ttu-id="7bb7b-137">美洲/拉巴斯</span><span class="sxs-lookup"><span data-stu-id="7bb7b-137">America/La_Paz</span></span>

<span data-ttu-id="7bb7b-138">美洲/圣地亚哥</span><span class="sxs-lookup"><span data-stu-id="7bb7b-138">America/Santiago</span></span>

<span data-ttu-id="7bb7b-139">美洲/圣约翰斯</span><span class="sxs-lookup"><span data-stu-id="7bb7b-139">America/St_Johns</span></span>

<span data-ttu-id="7bb7b-140">美洲/圣保罗</span><span class="sxs-lookup"><span data-stu-id="7bb7b-140">America/Sao_Paulo</span></span>

<span data-ttu-id="7bb7b-141">美洲/阿根廷/布宜诺斯艾利斯</span><span class="sxs-lookup"><span data-stu-id="7bb7b-141">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="7bb7b-142">美洲/卡宴</span><span class="sxs-lookup"><span data-stu-id="7bb7b-142">America/Cayenne</span></span>

<span data-ttu-id="7bb7b-143">美洲/戈特霍布</span><span class="sxs-lookup"><span data-stu-id="7bb7b-143">America/Godthab</span></span>

<span data-ttu-id="7bb7b-144">美洲/蒙得维的亚</span><span class="sxs-lookup"><span data-stu-id="7bb7b-144">America/Montevideo</span></span>

<span data-ttu-id="7bb7b-145">美洲/巴伊亚</span><span class="sxs-lookup"><span data-stu-id="7bb7b-145">America/Bahia</span></span>

<span data-ttu-id="7bb7b-146">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="7bb7b-146">Etc/GMT+2</span></span>

<span data-ttu-id="7bb7b-147">大西洋/亚速尔群岛</span><span class="sxs-lookup"><span data-stu-id="7bb7b-147">Atlantic/Azores</span></span>

<span data-ttu-id="7bb7b-148">大西洋/佛得角</span><span class="sxs-lookup"><span data-stu-id="7bb7b-148">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="7bb7b-149">非洲/卡萨布兰卡</span><span class="sxs-lookup"><span data-stu-id="7bb7b-149">Africa/Casablanca</span></span>

<span data-ttu-id="7bb7b-150">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="7bb7b-150">Etc/GMT</span></span>

<span data-ttu-id="7bb7b-151">欧洲/伦敦</span><span class="sxs-lookup"><span data-stu-id="7bb7b-151">Europe/London</span></span>

<span data-ttu-id="7bb7b-152">大西洋/雷克雅未克</span><span class="sxs-lookup"><span data-stu-id="7bb7b-152">Atlantic/Reykjavik</span></span>

<span data-ttu-id="7bb7b-153">欧洲/柏林</span><span class="sxs-lookup"><span data-stu-id="7bb7b-153">Europe/Berlin</span></span>

<span data-ttu-id="7bb7b-154">欧洲/布达佩斯</span><span class="sxs-lookup"><span data-stu-id="7bb7b-154">Europe/Budapest</span></span>

<span data-ttu-id="7bb7b-155">欧洲/巴黎</span><span class="sxs-lookup"><span data-stu-id="7bb7b-155">Europe/Paris</span></span>

<span data-ttu-id="7bb7b-156">欧洲/华沙</span><span class="sxs-lookup"><span data-stu-id="7bb7b-156">Europe/Warsaw</span></span>

<span data-ttu-id="7bb7b-157">非洲/拉各斯</span><span class="sxs-lookup"><span data-stu-id="7bb7b-157">Africa/Lagos</span></span>

<span data-ttu-id="7bb7b-158">非洲/温得和克</span><span class="sxs-lookup"><span data-stu-id="7bb7b-158">Africa/Windhoek</span></span>

<span data-ttu-id="7bb7b-159">欧洲/布加勒斯特</span><span class="sxs-lookup"><span data-stu-id="7bb7b-159">Europe/Bucharest</span></span>

<span data-ttu-id="7bb7b-160">亚洲/贝鲁特</span><span class="sxs-lookup"><span data-stu-id="7bb7b-160">Asia/Beirut</span></span>

<span data-ttu-id="7bb7b-161">非洲/开罗</span><span class="sxs-lookup"><span data-stu-id="7bb7b-161">Africa/Cairo</span></span>

<span data-ttu-id="7bb7b-162">亚洲/大马士革</span><span class="sxs-lookup"><span data-stu-id="7bb7b-162">Asia/Damascus</span></span>

<span data-ttu-id="7bb7b-163">非洲/约翰内斯堡</span><span class="sxs-lookup"><span data-stu-id="7bb7b-163">Africa/Johannesburg</span></span>

<span data-ttu-id="7bb7b-164">欧洲/基辅</span><span class="sxs-lookup"><span data-stu-id="7bb7b-164">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="7bb7b-165">欧洲/伊斯坦布尔</span><span class="sxs-lookup"><span data-stu-id="7bb7b-165">Europe/Istanbul</span></span>

<span data-ttu-id="7bb7b-166">亚洲/耶路撒冷</span><span class="sxs-lookup"><span data-stu-id="7bb7b-166">Asia/Jerusalem</span></span>

<span data-ttu-id="7bb7b-167">亚洲/安曼</span><span class="sxs-lookup"><span data-stu-id="7bb7b-167">Asia/Amman</span></span>

<span data-ttu-id="7bb7b-168">亚洲/巴格达</span><span class="sxs-lookup"><span data-stu-id="7bb7b-168">Asia/Baghdad</span></span>

<span data-ttu-id="7bb7b-169">欧洲/加里宁格勒</span><span class="sxs-lookup"><span data-stu-id="7bb7b-169">Europe/Kaliningrad</span></span>

<span data-ttu-id="7bb7b-170">亚洲/利雅得</span><span class="sxs-lookup"><span data-stu-id="7bb7b-170">Asia/Riyadh</span></span>

<span data-ttu-id="7bb7b-171">非洲/内罗毕</span><span class="sxs-lookup"><span data-stu-id="7bb7b-171">Africa/Nairobi</span></span>

<span data-ttu-id="7bb7b-172">亚洲/德黑兰</span><span class="sxs-lookup"><span data-stu-id="7bb7b-172">Asia/Tehran</span></span>

<span data-ttu-id="7bb7b-173">亚洲/迪拜</span><span class="sxs-lookup"><span data-stu-id="7bb7b-173">Asia/Dubai</span></span>

<span data-ttu-id="7bb7b-174">亚洲/巴库</span><span class="sxs-lookup"><span data-stu-id="7bb7b-174">Asia/Baku</span></span>

<span data-ttu-id="7bb7b-175">欧洲/莫斯科</span><span class="sxs-lookup"><span data-stu-id="7bb7b-175">Europe/Moscow</span></span>

<span data-ttu-id="7bb7b-176">印度洋/毛里求斯</span><span class="sxs-lookup"><span data-stu-id="7bb7b-176">Indian/Mauritius</span></span>

<span data-ttu-id="7bb7b-177">亚洲/第比利斯</span><span class="sxs-lookup"><span data-stu-id="7bb7b-177">Asia/Tbilisi</span></span>

<span data-ttu-id="7bb7b-178">亚洲/埃里温</span><span class="sxs-lookup"><span data-stu-id="7bb7b-178">Asia/Yerevan</span></span>

<span data-ttu-id="7bb7b-179">亚洲/喀布尔</span><span class="sxs-lookup"><span data-stu-id="7bb7b-179">Asia/Kabul</span></span>

<span data-ttu-id="7bb7b-180">亚洲/卡拉奇</span><span class="sxs-lookup"><span data-stu-id="7bb7b-180">Asia/Karachi</span></span>

<span data-ttu-id="7bb7b-181">亚洲/塔什干</span><span class="sxs-lookup"><span data-stu-id="7bb7b-181">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="7bb7b-182">亚洲/加尔各答</span><span class="sxs-lookup"><span data-stu-id="7bb7b-182">Asia/Kolkata</span></span>

<span data-ttu-id="7bb7b-183">亚洲/科伦坡</span><span class="sxs-lookup"><span data-stu-id="7bb7b-183">Asia/Colombo</span></span>

<span data-ttu-id="7bb7b-184">亚洲/加德满都</span><span class="sxs-lookup"><span data-stu-id="7bb7b-184">Asia/Kathmandu</span></span>

<span data-ttu-id="7bb7b-185">亚洲/阿斯塔纳（阿拉木图）</span><span class="sxs-lookup"><span data-stu-id="7bb7b-185">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="7bb7b-186">亚洲/达卡</span><span class="sxs-lookup"><span data-stu-id="7bb7b-186">Asia/Dhaka</span></span>

<span data-ttu-id="7bb7b-187">亚洲/叶卡捷琳堡</span><span class="sxs-lookup"><span data-stu-id="7bb7b-187">Asia/Yekaterinburg</span></span>

<span data-ttu-id="7bb7b-188">亚洲/仰光</span><span class="sxs-lookup"><span data-stu-id="7bb7b-188">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="7bb7b-189">亚洲/曼谷</span><span class="sxs-lookup"><span data-stu-id="7bb7b-189">Asia/Bangkok</span></span>

<span data-ttu-id="7bb7b-190">亚洲/新西伯利亚</span><span class="sxs-lookup"><span data-stu-id="7bb7b-190">Asia/Novosibirsk</span></span>

<span data-ttu-id="7bb7b-191">亚洲/上海</span><span class="sxs-lookup"><span data-stu-id="7bb7b-191">Asia/Shanghai</span></span>

<span data-ttu-id="7bb7b-192">亚洲/克拉斯诺亚尔斯克</span><span class="sxs-lookup"><span data-stu-id="7bb7b-192">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="7bb7b-193">亚洲/新加坡</span><span class="sxs-lookup"><span data-stu-id="7bb7b-193">Asia/Singapore</span></span>

<span data-ttu-id="7bb7b-194">澳大利亚/珀斯</span><span class="sxs-lookup"><span data-stu-id="7bb7b-194">Australia/Perth</span></span>

<span data-ttu-id="7bb7b-195">亚洲/台北</span><span class="sxs-lookup"><span data-stu-id="7bb7b-195">Asia/Taipei</span></span>

<span data-ttu-id="7bb7b-196">亚洲/乌兰巴托</span><span class="sxs-lookup"><span data-stu-id="7bb7b-196">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="7bb7b-197">亚洲/伊尔库茨克</span><span class="sxs-lookup"><span data-stu-id="7bb7b-197">Asia/Irkutsk</span></span>

<span data-ttu-id="7bb7b-198">亚洲/东京</span><span class="sxs-lookup"><span data-stu-id="7bb7b-198">Asia/Tokyo</span></span>

<span data-ttu-id="7bb7b-199">亚洲/首尔</span><span class="sxs-lookup"><span data-stu-id="7bb7b-199">Asia/Seoul</span></span>

<span data-ttu-id="7bb7b-200">澳洲/阿德莱德</span><span class="sxs-lookup"><span data-stu-id="7bb7b-200">Australia/Adelaide</span></span>

<span data-ttu-id="7bb7b-201">澳洲/达尔文</span><span class="sxs-lookup"><span data-stu-id="7bb7b-201">Australia/Darwin</span></span>

<span data-ttu-id="7bb7b-202">澳洲/布里斯班</span><span class="sxs-lookup"><span data-stu-id="7bb7b-202">Australia/Brisbane</span></span>

<span data-ttu-id="7bb7b-203">澳洲/悉尼</span><span class="sxs-lookup"><span data-stu-id="7bb7b-203">Australia/Sydney</span></span>

<span data-ttu-id="7bb7b-204">太平洋/莫尔斯比港</span><span class="sxs-lookup"><span data-stu-id="7bb7b-204">Pacific/Port_Moresby</span></span>

<span data-ttu-id="7bb7b-205">澳洲/霍巴特</span><span class="sxs-lookup"><span data-stu-id="7bb7b-205">Australia/Hobart</span></span>

<span data-ttu-id="7bb7b-206">亚洲/雅库茨克</span><span class="sxs-lookup"><span data-stu-id="7bb7b-206">Asia/Yakutsk</span></span>

<span data-ttu-id="7bb7b-207">太平洋/瓜达尔卡纳尔</span><span class="sxs-lookup"><span data-stu-id="7bb7b-207">Pacific/Guadalcanal</span></span>

<span data-ttu-id="7bb7b-208">亚洲/符拉迪沃斯托克</span><span class="sxs-lookup"><span data-stu-id="7bb7b-208">Asia/Vladivostok</span></span>

<span data-ttu-id="7bb7b-209">太平洋/奥克兰</span><span class="sxs-lookup"><span data-stu-id="7bb7b-209">Pacific/Auckland</span></span>

<span data-ttu-id="7bb7b-210">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="7bb7b-210">Etc/GMT-12</span></span>

<span data-ttu-id="7bb7b-211">太平洋/斐济</span><span class="sxs-lookup"><span data-stu-id="7bb7b-211">Pacific/Fiji</span></span>

<span data-ttu-id="7bb7b-212">亚洲/马加丹</span><span class="sxs-lookup"><span data-stu-id="7bb7b-212">Asia/Magadan</span></span>

<span data-ttu-id="7bb7b-213">太平洋/汤加塔布</span><span class="sxs-lookup"><span data-stu-id="7bb7b-213">Pacific/Tongatapu</span></span>

<span data-ttu-id="7bb7b-214">太平洋/阿皮亚</span><span class="sxs-lookup"><span data-stu-id="7bb7b-214">Pacific/Apia</span></span>

<span data-ttu-id="7bb7b-215">太平洋/圣诞岛</span><span class="sxs-lookup"><span data-stu-id="7bb7b-215">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="7bb7b-216">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="7bb7b-216">JSON representation</span></span>

<span data-ttu-id="7bb7b-217">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="7bb7b-217">Here is a JSON representation of the resource</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/datetimetimezone.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
