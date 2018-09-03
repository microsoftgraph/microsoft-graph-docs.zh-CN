# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="451ec-101">dateTimeTimeZone 资源类型</span><span class="sxs-lookup"><span data-stu-id="451ec-101">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="451ec-102">介绍某个时间点的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="451ec-102">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="451ec-103">属性</span><span class="sxs-lookup"><span data-stu-id="451ec-103">Properties</span></span>
| <span data-ttu-id="451ec-104">属性</span><span class="sxs-lookup"><span data-stu-id="451ec-104">Property</span></span>     | <span data-ttu-id="451ec-105">类型</span><span class="sxs-lookup"><span data-stu-id="451ec-105">Type</span></span>   |<span data-ttu-id="451ec-106">说明</span><span class="sxs-lookup"><span data-stu-id="451ec-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="451ec-107">dateTime</span><span class="sxs-lookup"><span data-stu-id="451ec-107">dateTime</span></span>|<span data-ttu-id="451ec-108">String</span><span class="sxs-lookup"><span data-stu-id="451ec-108">String</span></span>|<span data-ttu-id="451ec-109">日期和时间组合表示形式 (`<date>T<time>`) 的单个时间点。</span><span class="sxs-lookup"><span data-stu-id="451ec-109">A single point of time in a combined date and time representation (`<date>T<time>`).</span></span>|
|<span data-ttu-id="451ec-110">timeZone</span><span class="sxs-lookup"><span data-stu-id="451ec-110">timeZone</span></span>|<span data-ttu-id="451ec-111">String</span><span class="sxs-lookup"><span data-stu-id="451ec-111">String</span></span>|<span data-ttu-id="451ec-112">以下时区名称之一。</span><span class="sxs-lookup"><span data-stu-id="451ec-112">One of the following time zone names.</span></span>|

<span data-ttu-id="451ec-113">_TimeZone_ 属性可以设置为 Windows 支持的任意时区，以及以下时区名称。</span><span class="sxs-lookup"><span data-stu-id="451ec-113">The _TimeZone_ property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="451ec-114">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="451ec-114">Etc/GMT+12</span></span>

<span data-ttu-id="451ec-115">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="451ec-115">Etc/GMT+11</span></span>

<span data-ttu-id="451ec-116">太平洋/火奴鲁鲁</span><span class="sxs-lookup"><span data-stu-id="451ec-116">Pacific/Honolulu</span></span>

<span data-ttu-id="451ec-117">美洲/安克雷奇</span><span class="sxs-lookup"><span data-stu-id="451ec-117">America/Anchorage</span></span>

<span data-ttu-id="451ec-118">美洲/圣伊莎贝尔</span><span class="sxs-lookup"><span data-stu-id="451ec-118">America/Santa_Isabel</span></span>

<span data-ttu-id="451ec-119">美洲/洛杉矶</span><span class="sxs-lookup"><span data-stu-id="451ec-119">America/Los_Angeles</span></span>

<span data-ttu-id="451ec-120">美洲/菲尼克斯</span><span class="sxs-lookup"><span data-stu-id="451ec-120">America/Phoenix</span></span>

<span data-ttu-id="451ec-121">美洲/奇瓦瓦</span><span class="sxs-lookup"><span data-stu-id="451ec-121">America/Chihuahua</span></span>

<span data-ttu-id="451ec-122">美洲/丹佛</span><span class="sxs-lookup"><span data-stu-id="451ec-122">America/Denver</span></span>

<span data-ttu-id="451ec-123">美洲/危地马拉</span><span class="sxs-lookup"><span data-stu-id="451ec-123">America/Guatemala</span></span>

<span data-ttu-id="451ec-124">美洲/芝加哥</span><span class="sxs-lookup"><span data-stu-id="451ec-124">America/Chicago</span></span>

<span data-ttu-id="451ec-125">美洲/墨西哥城</span><span class="sxs-lookup"><span data-stu-id="451ec-125">America/Mexico_City</span></span>

<span data-ttu-id="451ec-126">美洲/里贾纳</span><span class="sxs-lookup"><span data-stu-id="451ec-126">America/Regina</span></span>

<span data-ttu-id="451ec-127">美洲/波哥大</span><span class="sxs-lookup"><span data-stu-id="451ec-127">America/Bogota</span></span>

<span data-ttu-id="451ec-128">美洲/纽约</span><span class="sxs-lookup"><span data-stu-id="451ec-128">America/New_York</span></span>

<span data-ttu-id="451ec-129">美洲/印第安纳/印第安纳波利斯</span><span class="sxs-lookup"><span data-stu-id="451ec-129">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="451ec-130">美洲/加拉加斯</span><span class="sxs-lookup"><span data-stu-id="451ec-130">America/Caracas</span></span>

<span data-ttu-id="451ec-131">美洲/亚松森</span><span class="sxs-lookup"><span data-stu-id="451ec-131">America/Asuncion</span></span>

<span data-ttu-id="451ec-132">美洲/哈利法克斯</span><span class="sxs-lookup"><span data-stu-id="451ec-132">America/Halifax</span></span>

<span data-ttu-id="451ec-133">美洲/库亚巴</span><span class="sxs-lookup"><span data-stu-id="451ec-133">America/Cuiaba</span></span>

<span data-ttu-id="451ec-134">美洲/拉巴斯</span><span class="sxs-lookup"><span data-stu-id="451ec-134">America/La_Paz</span></span>

<span data-ttu-id="451ec-135">美洲/圣地亚哥</span><span class="sxs-lookup"><span data-stu-id="451ec-135">America/Santiago</span></span>

<span data-ttu-id="451ec-136">美洲/圣约翰斯</span><span class="sxs-lookup"><span data-stu-id="451ec-136">America/St_Johns</span></span>

<span data-ttu-id="451ec-137">美洲/圣保罗</span><span class="sxs-lookup"><span data-stu-id="451ec-137">America/Sao_Paulo</span></span>

<span data-ttu-id="451ec-138">美洲/阿根廷/布宜诺斯艾利斯</span><span class="sxs-lookup"><span data-stu-id="451ec-138">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="451ec-139">美洲/卡宴</span><span class="sxs-lookup"><span data-stu-id="451ec-139">America/Cayenne</span></span>

<span data-ttu-id="451ec-140">美洲/戈特霍布</span><span class="sxs-lookup"><span data-stu-id="451ec-140">America/Godthab</span></span>

<span data-ttu-id="451ec-141">美洲/蒙得维的亚</span><span class="sxs-lookup"><span data-stu-id="451ec-141">America/Montevideo</span></span>

<span data-ttu-id="451ec-142">美洲/巴伊亚</span><span class="sxs-lookup"><span data-stu-id="451ec-142">America/Bahia</span></span>

<span data-ttu-id="451ec-143">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="451ec-143">Etc/GMT+2</span></span>

<span data-ttu-id="451ec-144">大西洋/亚速尔群岛</span><span class="sxs-lookup"><span data-stu-id="451ec-144">Atlantic/Azores</span></span>

<span data-ttu-id="451ec-145">大西洋/佛得角</span><span class="sxs-lookup"><span data-stu-id="451ec-145">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="451ec-146">非洲/卡萨布兰卡</span><span class="sxs-lookup"><span data-stu-id="451ec-146">Africa/Casablanca</span></span>

<span data-ttu-id="451ec-147">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="451ec-147">Etc/GMT</span></span>

<span data-ttu-id="451ec-148">欧洲/伦敦</span><span class="sxs-lookup"><span data-stu-id="451ec-148">Europe/London</span></span>

<span data-ttu-id="451ec-149">大西洋/雷克雅未克</span><span class="sxs-lookup"><span data-stu-id="451ec-149">Atlantic/Reykjavik</span></span>

<span data-ttu-id="451ec-150">欧洲/柏林</span><span class="sxs-lookup"><span data-stu-id="451ec-150">Europe/Berlin</span></span>

<span data-ttu-id="451ec-151">欧洲/布达佩斯</span><span class="sxs-lookup"><span data-stu-id="451ec-151">Europe/Budapest</span></span>

<span data-ttu-id="451ec-152">欧洲/巴黎</span><span class="sxs-lookup"><span data-stu-id="451ec-152">Europe/Paris</span></span>

<span data-ttu-id="451ec-153">欧洲/华沙</span><span class="sxs-lookup"><span data-stu-id="451ec-153">Europe/Warsaw</span></span>

<span data-ttu-id="451ec-154">非洲/拉各斯</span><span class="sxs-lookup"><span data-stu-id="451ec-154">Africa/Lagos</span></span>

<span data-ttu-id="451ec-155">非洲/温得和克</span><span class="sxs-lookup"><span data-stu-id="451ec-155">Africa/Windhoek</span></span>

<span data-ttu-id="451ec-156">欧洲/布加勒斯特</span><span class="sxs-lookup"><span data-stu-id="451ec-156">Europe/Bucharest</span></span>

<span data-ttu-id="451ec-157">亚洲/贝鲁特</span><span class="sxs-lookup"><span data-stu-id="451ec-157">Asia/Beirut</span></span>

<span data-ttu-id="451ec-158">非洲/开罗</span><span class="sxs-lookup"><span data-stu-id="451ec-158">Africa/Cairo</span></span>

<span data-ttu-id="451ec-159">亚洲/大马士革</span><span class="sxs-lookup"><span data-stu-id="451ec-159">Asia/Damascus</span></span>

<span data-ttu-id="451ec-160">非洲/约翰内斯堡</span><span class="sxs-lookup"><span data-stu-id="451ec-160">Africa/Johannesburg</span></span>

<span data-ttu-id="451ec-161">欧洲/基辅</span><span class="sxs-lookup"><span data-stu-id="451ec-161">Europe/Kyiv (Kiev)</span></span>

<span data-ttu-id="451ec-162">欧洲/伊斯坦布尔</span><span class="sxs-lookup"><span data-stu-id="451ec-162">Europe/Istanbul</span></span>

<span data-ttu-id="451ec-163">亚洲/耶路撒冷</span><span class="sxs-lookup"><span data-stu-id="451ec-163">Asia/Jerusalem</span></span>

<span data-ttu-id="451ec-164">亚洲/安曼</span><span class="sxs-lookup"><span data-stu-id="451ec-164">Asia/Amman</span></span>

<span data-ttu-id="451ec-165">亚洲/巴格达</span><span class="sxs-lookup"><span data-stu-id="451ec-165">Asia/Baghdad</span></span>

<span data-ttu-id="451ec-166">欧洲/加里宁格勒</span><span class="sxs-lookup"><span data-stu-id="451ec-166">Europe/Kaliningrad</span></span>

<span data-ttu-id="451ec-167">亚洲/利雅得</span><span class="sxs-lookup"><span data-stu-id="451ec-167">Asia/Riyadh</span></span>

<span data-ttu-id="451ec-168">非洲/内罗毕</span><span class="sxs-lookup"><span data-stu-id="451ec-168">Africa/Nairobi</span></span>

<span data-ttu-id="451ec-169">亚洲/德黑兰</span><span class="sxs-lookup"><span data-stu-id="451ec-169">Asia/Tehran</span></span>

<span data-ttu-id="451ec-170">亚洲/迪拜</span><span class="sxs-lookup"><span data-stu-id="451ec-170">Asia/Dubai</span></span>

<span data-ttu-id="451ec-171">亚洲/巴库</span><span class="sxs-lookup"><span data-stu-id="451ec-171">Asia/Baku</span></span>

<span data-ttu-id="451ec-172">欧洲/莫斯科</span><span class="sxs-lookup"><span data-stu-id="451ec-172">Europe/Moscow</span></span>

<span data-ttu-id="451ec-173">印度洋/毛里求斯</span><span class="sxs-lookup"><span data-stu-id="451ec-173">Indian/Mauritius</span></span>

<span data-ttu-id="451ec-174">亚洲/第比利斯</span><span class="sxs-lookup"><span data-stu-id="451ec-174">Asia/Tbilisi</span></span>

<span data-ttu-id="451ec-175">亚洲/埃里温</span><span class="sxs-lookup"><span data-stu-id="451ec-175">Asia/Yerevan</span></span>

<span data-ttu-id="451ec-176">亚洲/喀布尔</span><span class="sxs-lookup"><span data-stu-id="451ec-176">Asia/Kabul</span></span>

<span data-ttu-id="451ec-177">亚洲/卡拉奇</span><span class="sxs-lookup"><span data-stu-id="451ec-177">Asia/Karachi</span></span>

<span data-ttu-id="451ec-178">亚洲/塔什干</span><span class="sxs-lookup"><span data-stu-id="451ec-178">Asia/Toshkent (Tashkent)</span></span>

<span data-ttu-id="451ec-179">亚洲/加尔各答</span><span class="sxs-lookup"><span data-stu-id="451ec-179">Asia/Kolkata</span></span>

<span data-ttu-id="451ec-180">亚洲/科伦坡</span><span class="sxs-lookup"><span data-stu-id="451ec-180">Asia/Colombo</span></span>

<span data-ttu-id="451ec-181">亚洲/加德满都</span><span class="sxs-lookup"><span data-stu-id="451ec-181">Asia/Kathmandu</span></span>

<span data-ttu-id="451ec-182">亚洲/阿斯塔纳（阿拉木图）</span><span class="sxs-lookup"><span data-stu-id="451ec-182">Asia/Astana (Almaty)</span></span>

<span data-ttu-id="451ec-183">亚洲/达卡</span><span class="sxs-lookup"><span data-stu-id="451ec-183">Asia/Dhaka</span></span>

<span data-ttu-id="451ec-184">亚洲/叶卡捷琳堡</span><span class="sxs-lookup"><span data-stu-id="451ec-184">Asia/Yekaterinburg</span></span>

<span data-ttu-id="451ec-185">亚洲/仰光</span><span class="sxs-lookup"><span data-stu-id="451ec-185">Asia/Yangon (Rangoon)</span></span>

<span data-ttu-id="451ec-186">亚洲/曼谷</span><span class="sxs-lookup"><span data-stu-id="451ec-186">Asia/Bangkok</span></span>

<span data-ttu-id="451ec-187">亚洲/新西伯利亚</span><span class="sxs-lookup"><span data-stu-id="451ec-187">Asia/Novosibirsk</span></span>

<span data-ttu-id="451ec-188">亚洲/上海</span><span class="sxs-lookup"><span data-stu-id="451ec-188">Asia/Shanghai</span></span>

<span data-ttu-id="451ec-189">亚洲/克拉斯诺亚尔斯克</span><span class="sxs-lookup"><span data-stu-id="451ec-189">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="451ec-190">亚洲/新加坡</span><span class="sxs-lookup"><span data-stu-id="451ec-190">Asia/Singapore</span></span>

<span data-ttu-id="451ec-191">澳大利亚/珀斯</span><span class="sxs-lookup"><span data-stu-id="451ec-191">Australia/Perth</span></span>

<span data-ttu-id="451ec-192">亚洲/台北</span><span class="sxs-lookup"><span data-stu-id="451ec-192">Asia/Taipei</span></span>

<span data-ttu-id="451ec-193">亚洲/乌兰巴托</span><span class="sxs-lookup"><span data-stu-id="451ec-193">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="451ec-194">亚洲/伊尔库茨克</span><span class="sxs-lookup"><span data-stu-id="451ec-194">Asia/Irkutsk</span></span>

<span data-ttu-id="451ec-195">亚洲/东京</span><span class="sxs-lookup"><span data-stu-id="451ec-195">Asia/Tokyo</span></span>

<span data-ttu-id="451ec-196">亚洲/首尔</span><span class="sxs-lookup"><span data-stu-id="451ec-196">Asia/Seoul</span></span>

<span data-ttu-id="451ec-197">澳洲/阿德莱德</span><span class="sxs-lookup"><span data-stu-id="451ec-197">Australia/Adelaide</span></span>

<span data-ttu-id="451ec-198">澳洲/达尔文</span><span class="sxs-lookup"><span data-stu-id="451ec-198">Australia/Darwin</span></span>

<span data-ttu-id="451ec-199">澳洲/布里斯班</span><span class="sxs-lookup"><span data-stu-id="451ec-199">Australia/Brisbane</span></span>

<span data-ttu-id="451ec-200">澳洲/悉尼</span><span class="sxs-lookup"><span data-stu-id="451ec-200">Australia/Sydney</span></span>

<span data-ttu-id="451ec-201">太平洋/莫尔斯比港</span><span class="sxs-lookup"><span data-stu-id="451ec-201">Pacific/Port_Moresby</span></span>

<span data-ttu-id="451ec-202">澳洲/霍巴特</span><span class="sxs-lookup"><span data-stu-id="451ec-202">Australia/Hobart</span></span>

<span data-ttu-id="451ec-203">亚洲/雅库茨克</span><span class="sxs-lookup"><span data-stu-id="451ec-203">Asia/Yakutsk</span></span>

<span data-ttu-id="451ec-204">太平洋/瓜达尔卡纳尔</span><span class="sxs-lookup"><span data-stu-id="451ec-204">Pacific/Guadalcanal</span></span>

<span data-ttu-id="451ec-205">亚洲/符拉迪沃斯托克</span><span class="sxs-lookup"><span data-stu-id="451ec-205">Asia/Vladivostok</span></span>

<span data-ttu-id="451ec-206">太平洋/奥克兰</span><span class="sxs-lookup"><span data-stu-id="451ec-206">Pacific/Auckland</span></span>

<span data-ttu-id="451ec-207">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="451ec-207">Etc/GMT-12</span></span>

<span data-ttu-id="451ec-208">太平洋/斐济</span><span class="sxs-lookup"><span data-stu-id="451ec-208">Pacific/Fiji</span></span>

<span data-ttu-id="451ec-209">亚洲/马加丹</span><span class="sxs-lookup"><span data-stu-id="451ec-209">Asia/Magadan</span></span>

<span data-ttu-id="451ec-210">太平洋/汤加塔布</span><span class="sxs-lookup"><span data-stu-id="451ec-210">Pacific/Tongatapu</span></span>

<span data-ttu-id="451ec-211">太平洋/阿皮亚</span><span class="sxs-lookup"><span data-stu-id="451ec-211">Pacific/Apia</span></span>

<span data-ttu-id="451ec-212">太平洋/圣诞岛</span><span class="sxs-lookup"><span data-stu-id="451ec-212">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="451ec-213">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="451ec-213">JSON representation</span></span>

<span data-ttu-id="451ec-214">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="451ec-214">Here is a JSON representation of the resource</span></span>

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
