# <a name="datetimetimezone-resource-type"></a><span data-ttu-id="eea0c-101">dateTimeTimeZone 资源类型</span><span class="sxs-lookup"><span data-stu-id="eea0c-101">dateTimeTimeZone resource type</span></span>

<span data-ttu-id="eea0c-102">介绍某个时间点的日期、时间和时区。</span><span class="sxs-lookup"><span data-stu-id="eea0c-102">Describes the date, time, and time zone of a point in time.</span></span>

## <a name="properties"></a><span data-ttu-id="eea0c-103">属性</span><span class="sxs-lookup"><span data-stu-id="eea0c-103">Properties</span></span>
| <span data-ttu-id="eea0c-104">属性</span><span class="sxs-lookup"><span data-stu-id="eea0c-104">Property</span></span>     | <span data-ttu-id="eea0c-105">类型</span><span class="sxs-lookup"><span data-stu-id="eea0c-105">Type</span></span>   |<span data-ttu-id="eea0c-106">说明</span><span class="sxs-lookup"><span data-stu-id="eea0c-106">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="eea0c-107">DateTime</span><span class="sxs-lookup"><span data-stu-id="eea0c-107">DateTime</span></span>|<span data-ttu-id="eea0c-108">String</span><span class="sxs-lookup"><span data-stu-id="eea0c-108">String</span></span>|<span data-ttu-id="eea0c-109">日期和时间组合表示形式的单个时间点 (`<date>T<time>`)。</span><span class="sxs-lookup"><span data-stu-id="eea0c-109">A single point of time in a combined date and time representation (`<date>T<time>`).</span></span>|
|<span data-ttu-id="eea0c-110">TimeZone</span><span class="sxs-lookup"><span data-stu-id="eea0c-110">TimeZone</span></span>|<span data-ttu-id="eea0c-111">String</span><span class="sxs-lookup"><span data-stu-id="eea0c-111">String</span></span>|<span data-ttu-id="eea0c-112">以下时区名称之一。</span><span class="sxs-lookup"><span data-stu-id="eea0c-112">One of the following time zone names.</span></span>|

<span data-ttu-id="eea0c-113">_TimeZone_ 属性可以设置为 Windows 支持的任意时区，以及以下时区名称。</span><span class="sxs-lookup"><span data-stu-id="eea0c-113">The _TimeZone_ property can be set to any of the time zones supported by Windows, as well as the following time zones names.</span></span>

<span data-ttu-id="eea0c-114">Etc/GMT+12</span><span class="sxs-lookup"><span data-stu-id="eea0c-114">Etc/GMT+12</span></span>

<span data-ttu-id="eea0c-115">Etc/GMT+11</span><span class="sxs-lookup"><span data-stu-id="eea0c-115">Etc/GMT+11</span></span>

<span data-ttu-id="eea0c-116">太平洋/火奴鲁鲁</span><span class="sxs-lookup"><span data-stu-id="eea0c-116">Pacific/Honolulu</span></span>

<span data-ttu-id="eea0c-117">美洲/安克雷奇</span><span class="sxs-lookup"><span data-stu-id="eea0c-117">America/Anchorage</span></span>

<span data-ttu-id="eea0c-118">美洲/圣伊莎贝尔</span><span class="sxs-lookup"><span data-stu-id="eea0c-118">America/Santa_Isabel</span></span>

<span data-ttu-id="eea0c-119">美洲/洛杉矶</span><span class="sxs-lookup"><span data-stu-id="eea0c-119">America/Los_Angeles</span></span>

<span data-ttu-id="eea0c-120">美洲/菲尼克斯</span><span class="sxs-lookup"><span data-stu-id="eea0c-120">America/Phoenix</span></span>

<span data-ttu-id="eea0c-121">美洲/奇瓦瓦</span><span class="sxs-lookup"><span data-stu-id="eea0c-121">America/Chihuahua</span></span>

<span data-ttu-id="eea0c-122">美洲/丹佛</span><span class="sxs-lookup"><span data-stu-id="eea0c-122">America/Denver</span></span>

<span data-ttu-id="eea0c-123">美洲/危地马拉</span><span class="sxs-lookup"><span data-stu-id="eea0c-123">America/Guatemala</span></span>

<span data-ttu-id="eea0c-124">美洲/芝加哥</span><span class="sxs-lookup"><span data-stu-id="eea0c-124">America/Chicago</span></span>

<span data-ttu-id="eea0c-125">美洲/墨西哥城</span><span class="sxs-lookup"><span data-stu-id="eea0c-125">America/Mexico_City</span></span>

<span data-ttu-id="eea0c-126">美洲/里贾纳</span><span class="sxs-lookup"><span data-stu-id="eea0c-126">America/Regina</span></span>

<span data-ttu-id="eea0c-127">美洲/波哥大</span><span class="sxs-lookup"><span data-stu-id="eea0c-127">America/Bogota</span></span>

<span data-ttu-id="eea0c-128">美洲/纽约</span><span class="sxs-lookup"><span data-stu-id="eea0c-128">America/New_York</span></span>

<span data-ttu-id="eea0c-129">美洲/印第安纳/印第安纳波利斯</span><span class="sxs-lookup"><span data-stu-id="eea0c-129">America/Indiana/Indianapolis</span></span>

<span data-ttu-id="eea0c-130">美洲/加拉加斯</span><span class="sxs-lookup"><span data-stu-id="eea0c-130">America/Caracas</span></span>

<span data-ttu-id="eea0c-131">美洲/亚松森</span><span class="sxs-lookup"><span data-stu-id="eea0c-131">America/Asuncion</span></span>

<span data-ttu-id="eea0c-132">美洲/哈利法克斯</span><span class="sxs-lookup"><span data-stu-id="eea0c-132">America/Halifax</span></span>

<span data-ttu-id="eea0c-133">美洲/库亚巴</span><span class="sxs-lookup"><span data-stu-id="eea0c-133">America/Cuiaba</span></span>

<span data-ttu-id="eea0c-134">美洲/拉巴斯</span><span class="sxs-lookup"><span data-stu-id="eea0c-134">America/La_Paz</span></span>

<span data-ttu-id="eea0c-135">美洲/圣地亚哥</span><span class="sxs-lookup"><span data-stu-id="eea0c-135">America/Santiago</span></span>

<span data-ttu-id="eea0c-136">美洲/圣约翰斯</span><span class="sxs-lookup"><span data-stu-id="eea0c-136">America/St_Johns</span></span>

<span data-ttu-id="eea0c-137">美洲/圣保罗</span><span class="sxs-lookup"><span data-stu-id="eea0c-137">America/Sao_Paulo</span></span>

<span data-ttu-id="eea0c-138">美洲/阿根廷/布宜诺斯艾利斯</span><span class="sxs-lookup"><span data-stu-id="eea0c-138">America/Argentina/Buenos_Aires</span></span>

<span data-ttu-id="eea0c-139">美洲/卡宴</span><span class="sxs-lookup"><span data-stu-id="eea0c-139">America/Cayenne</span></span>

<span data-ttu-id="eea0c-140">美洲/戈特霍布</span><span class="sxs-lookup"><span data-stu-id="eea0c-140">America/Godthab</span></span>

<span data-ttu-id="eea0c-141">美洲/蒙得维的亚</span><span class="sxs-lookup"><span data-stu-id="eea0c-141">America/Montevideo</span></span>

<span data-ttu-id="eea0c-142">美洲/巴伊亚</span><span class="sxs-lookup"><span data-stu-id="eea0c-142">America/Bahia</span></span>

<span data-ttu-id="eea0c-143">Etc/GMT+2</span><span class="sxs-lookup"><span data-stu-id="eea0c-143">Etc/GMT+2</span></span>

<span data-ttu-id="eea0c-144">大西洋/亚速尔群岛</span><span class="sxs-lookup"><span data-stu-id="eea0c-144">Atlantic/Azores</span></span>

<span data-ttu-id="eea0c-145">大西洋/佛得角</span><span class="sxs-lookup"><span data-stu-id="eea0c-145">Atlantic/Cape_Verde</span></span>

<span data-ttu-id="eea0c-146">非洲/卡萨布兰卡</span><span class="sxs-lookup"><span data-stu-id="eea0c-146">Africa/Casablanca</span></span>

<span data-ttu-id="eea0c-147">Etc/GMT</span><span class="sxs-lookup"><span data-stu-id="eea0c-147">Etc/GMT</span></span>

<span data-ttu-id="eea0c-148">欧洲/伦敦</span><span class="sxs-lookup"><span data-stu-id="eea0c-148">Europe/London</span></span>

<span data-ttu-id="eea0c-149">大西洋/雷克雅未克</span><span class="sxs-lookup"><span data-stu-id="eea0c-149">Atlantic/Reykjavik</span></span>

<span data-ttu-id="eea0c-150">欧洲/柏林</span><span class="sxs-lookup"><span data-stu-id="eea0c-150">Europe/Berlin</span></span>

<span data-ttu-id="eea0c-151">欧洲/布达佩斯</span><span class="sxs-lookup"><span data-stu-id="eea0c-151">Europe/Budapest</span></span>

<span data-ttu-id="eea0c-152">欧洲/巴黎</span><span class="sxs-lookup"><span data-stu-id="eea0c-152">Europe/Paris</span></span>

<span data-ttu-id="eea0c-153">欧洲/华沙</span><span class="sxs-lookup"><span data-stu-id="eea0c-153">Europe/Warsaw</span></span>

<span data-ttu-id="eea0c-154">非洲/拉各斯</span><span class="sxs-lookup"><span data-stu-id="eea0c-154">Africa/Lagos</span></span>

<span data-ttu-id="eea0c-155">非洲/温得和克</span><span class="sxs-lookup"><span data-stu-id="eea0c-155">Africa/Windhoek</span></span>

<span data-ttu-id="eea0c-156">欧洲/布加勒斯特</span><span class="sxs-lookup"><span data-stu-id="eea0c-156">Europe/Bucharest</span></span>

<span data-ttu-id="eea0c-157">亚洲/贝鲁特</span><span class="sxs-lookup"><span data-stu-id="eea0c-157">Asia/Beirut</span></span>

<span data-ttu-id="eea0c-158">非洲/开罗</span><span class="sxs-lookup"><span data-stu-id="eea0c-158">Africa/Cairo</span></span>

<span data-ttu-id="eea0c-159">亚洲/大马士革</span><span class="sxs-lookup"><span data-stu-id="eea0c-159">Asia/Damascus</span></span>

<span data-ttu-id="eea0c-160">非洲/约翰内斯堡</span><span class="sxs-lookup"><span data-stu-id="eea0c-160">Africa/Johannesburg</span></span>

<span data-ttu-id="eea0c-161">欧洲/基辅</span><span class="sxs-lookup"><span data-stu-id="eea0c-161">Europe/Kiev</span></span>

<span data-ttu-id="eea0c-162">欧洲/伊斯坦布尔</span><span class="sxs-lookup"><span data-stu-id="eea0c-162">Europe/Istanbul</span></span>

<span data-ttu-id="eea0c-163">亚洲/耶路撒冷</span><span class="sxs-lookup"><span data-stu-id="eea0c-163">Asia/Jerusalem</span></span>

<span data-ttu-id="eea0c-164">亚洲/安曼</span><span class="sxs-lookup"><span data-stu-id="eea0c-164">Asia/Amman</span></span>

<span data-ttu-id="eea0c-165">亚洲/巴格达</span><span class="sxs-lookup"><span data-stu-id="eea0c-165">Asia/Baghdad</span></span>

<span data-ttu-id="eea0c-166">欧洲/加里宁格勒</span><span class="sxs-lookup"><span data-stu-id="eea0c-166">Europe/Kaliningrad</span></span>

<span data-ttu-id="eea0c-167">亚洲/利雅得</span><span class="sxs-lookup"><span data-stu-id="eea0c-167">Asia/Riyadh</span></span>

<span data-ttu-id="eea0c-168">非洲/内罗毕</span><span class="sxs-lookup"><span data-stu-id="eea0c-168">Africa/Nairobi</span></span>

<span data-ttu-id="eea0c-169">亚洲/德黑兰</span><span class="sxs-lookup"><span data-stu-id="eea0c-169">Asia/Tehran</span></span>

<span data-ttu-id="eea0c-170">亚洲/迪拜</span><span class="sxs-lookup"><span data-stu-id="eea0c-170">Asia/Dubai</span></span>

<span data-ttu-id="eea0c-171">亚洲/巴库</span><span class="sxs-lookup"><span data-stu-id="eea0c-171">Asia/Baku</span></span>

<span data-ttu-id="eea0c-172">欧洲/莫斯科</span><span class="sxs-lookup"><span data-stu-id="eea0c-172">Europe/Moscow</span></span>

<span data-ttu-id="eea0c-173">印度洋/毛里求斯</span><span class="sxs-lookup"><span data-stu-id="eea0c-173">Indian/Mauritius</span></span>

<span data-ttu-id="eea0c-174">亚洲/第比利斯</span><span class="sxs-lookup"><span data-stu-id="eea0c-174">Asia/Tbilisi</span></span>

<span data-ttu-id="eea0c-175">亚洲/埃里温</span><span class="sxs-lookup"><span data-stu-id="eea0c-175">Asia/Yerevan</span></span>

<span data-ttu-id="eea0c-176">亚洲/喀布尔</span><span class="sxs-lookup"><span data-stu-id="eea0c-176">Asia/Kabul</span></span>

<span data-ttu-id="eea0c-177">亚洲/卡拉奇</span><span class="sxs-lookup"><span data-stu-id="eea0c-177">Asia/Karachi</span></span>

<span data-ttu-id="eea0c-178">亚洲/塔什干</span><span class="sxs-lookup"><span data-stu-id="eea0c-178">Asia/Tashkent</span></span>

<span data-ttu-id="eea0c-179">亚洲/加尔各答</span><span class="sxs-lookup"><span data-stu-id="eea0c-179">Asia/Kolkata</span></span>

<span data-ttu-id="eea0c-180">亚洲/科伦坡</span><span class="sxs-lookup"><span data-stu-id="eea0c-180">Asia/Colombo</span></span>

<span data-ttu-id="eea0c-181">亚洲/加德满都</span><span class="sxs-lookup"><span data-stu-id="eea0c-181">Asia/Kathmandu</span></span>

<span data-ttu-id="eea0c-182">亚洲/阿拉木图</span><span class="sxs-lookup"><span data-stu-id="eea0c-182">Asia/Almaty</span></span>

<span data-ttu-id="eea0c-183">亚洲/达卡</span><span class="sxs-lookup"><span data-stu-id="eea0c-183">Asia/Dhaka</span></span>

<span data-ttu-id="eea0c-184">亚洲/叶卡捷琳堡</span><span class="sxs-lookup"><span data-stu-id="eea0c-184">Asia/Yekaterinburg</span></span>

<span data-ttu-id="eea0c-185">亚洲/仰光</span><span class="sxs-lookup"><span data-stu-id="eea0c-185">Asia/Rangoon</span></span>

<span data-ttu-id="eea0c-186">亚洲/曼谷</span><span class="sxs-lookup"><span data-stu-id="eea0c-186">Asia/Bangkok</span></span>

<span data-ttu-id="eea0c-187">亚洲/新西伯利亚</span><span class="sxs-lookup"><span data-stu-id="eea0c-187">Asia/Novosibirsk</span></span>

<span data-ttu-id="eea0c-188">亚洲/上海</span><span class="sxs-lookup"><span data-stu-id="eea0c-188">Asia/Shanghai</span></span>

<span data-ttu-id="eea0c-189">亚洲/克拉斯诺亚尔斯克</span><span class="sxs-lookup"><span data-stu-id="eea0c-189">Asia/Krasnoyarsk</span></span>

<span data-ttu-id="eea0c-190">亚洲/新加坡</span><span class="sxs-lookup"><span data-stu-id="eea0c-190">Asia/Singapore</span></span>

<span data-ttu-id="eea0c-191">澳大利亚/珀斯</span><span class="sxs-lookup"><span data-stu-id="eea0c-191">Australia/Perth</span></span>

<span data-ttu-id="eea0c-192">亚洲/台北</span><span class="sxs-lookup"><span data-stu-id="eea0c-192">Asia/Taipei</span></span>

<span data-ttu-id="eea0c-193">亚洲/乌兰巴托</span><span class="sxs-lookup"><span data-stu-id="eea0c-193">Asia/Ulaanbaatar</span></span>

<span data-ttu-id="eea0c-194">亚洲/伊尔库茨克</span><span class="sxs-lookup"><span data-stu-id="eea0c-194">Asia/Irkutsk</span></span>

<span data-ttu-id="eea0c-195">亚洲/东京</span><span class="sxs-lookup"><span data-stu-id="eea0c-195">Asia/Tokyo</span></span>

<span data-ttu-id="eea0c-196">亚洲/首尔</span><span class="sxs-lookup"><span data-stu-id="eea0c-196">Asia/Seoul</span></span>

<span data-ttu-id="eea0c-197">澳洲/阿德莱德</span><span class="sxs-lookup"><span data-stu-id="eea0c-197">Australia/Adelaide</span></span>

<span data-ttu-id="eea0c-198">澳洲/达尔文</span><span class="sxs-lookup"><span data-stu-id="eea0c-198">Australia/Darwin</span></span>

<span data-ttu-id="eea0c-199">澳洲/布里斯班</span><span class="sxs-lookup"><span data-stu-id="eea0c-199">Australia/Brisbane</span></span>

<span data-ttu-id="eea0c-200">澳洲/悉尼</span><span class="sxs-lookup"><span data-stu-id="eea0c-200">Australia/Sydney</span></span>

<span data-ttu-id="eea0c-201">太平洋/莫尔斯比港</span><span class="sxs-lookup"><span data-stu-id="eea0c-201">Pacific/Port_Moresby</span></span>

<span data-ttu-id="eea0c-202">澳洲/霍巴特</span><span class="sxs-lookup"><span data-stu-id="eea0c-202">Australia/Hobart</span></span>

<span data-ttu-id="eea0c-203">亚洲/雅库茨克</span><span class="sxs-lookup"><span data-stu-id="eea0c-203">Asia/Yakutsk</span></span>

<span data-ttu-id="eea0c-204">太平洋/瓜达尔卡纳尔</span><span class="sxs-lookup"><span data-stu-id="eea0c-204">Pacific/Guadalcanal</span></span>

<span data-ttu-id="eea0c-205">亚洲/符拉迪沃斯托克</span><span class="sxs-lookup"><span data-stu-id="eea0c-205">Asia/Vladivostok</span></span>

<span data-ttu-id="eea0c-206">太平洋/奥克兰</span><span class="sxs-lookup"><span data-stu-id="eea0c-206">Pacific/Auckland</span></span>

<span data-ttu-id="eea0c-207">Etc/GMT-12</span><span class="sxs-lookup"><span data-stu-id="eea0c-207">Etc/GMT-12</span></span>

<span data-ttu-id="eea0c-208">太平洋/斐济</span><span class="sxs-lookup"><span data-stu-id="eea0c-208">Pacific/Fiji</span></span>

<span data-ttu-id="eea0c-209">亚洲/马加丹</span><span class="sxs-lookup"><span data-stu-id="eea0c-209">Asia/Magadan</span></span>

<span data-ttu-id="eea0c-210">太平洋/汤加塔布</span><span class="sxs-lookup"><span data-stu-id="eea0c-210">Pacific/Tongatapu</span></span>

<span data-ttu-id="eea0c-211">太平洋/阿皮亚</span><span class="sxs-lookup"><span data-stu-id="eea0c-211">Pacific/Apia</span></span>

<span data-ttu-id="eea0c-212">太平洋/圣诞岛</span><span class="sxs-lookup"><span data-stu-id="eea0c-212">Pacific/Kiritimati</span></span>

## <a name="json-representation"></a><span data-ttu-id="eea0c-213">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="eea0c-213">JSON representation</span></span>

<span data-ttu-id="eea0c-214">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="eea0c-214">Here is a JSON representation of the resource</span></span>

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
