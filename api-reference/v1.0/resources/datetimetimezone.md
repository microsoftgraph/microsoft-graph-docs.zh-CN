---
title: dateTimeTimeZone 资源类型
description: 介绍某个时间点的日期、时间和时区。
localization_priority: Priority
doc_type: resourcePageType
author: harini84
ms.prod: outlook
ms.openlocfilehash: bfbd81bc08720e0974c34529502009dcff2a28b714327c09b71e3343d6042023
ms.sourcegitcommit: 986c33b848fa22a153f28437738953532b78c051
ms.translationtype: HT
ms.contentlocale: zh-CN
ms.lasthandoff: 08/05/2021
ms.locfileid: "54124526"
---
# <a name="datetimetimezone-resource-type"></a>dateTimeTimeZone 资源类型

命名空间：microsoft.graph

介绍某个时间点的日期、时间和时区。

## <a name="properties"></a>属性
| 属性     | 类型   |说明|
|:---------------|:--------|:----------|
|dateTime|字符串|日期和时间组合表示形式的单个时间点（`{date}T{time}`；例如 `2017-08-29T04:00:00.0000000`）。|
|timeZone|String|表示时区，例如“太平洋标准时间”。 有关更多可能的值，请参见下文。|

通常，**timeZone** 属性 _可以_ 设置为 [Windows 当前支持的任意时区](/windows-hardware/manufacture/desktop/default-time-zones)，以及 [日历 API 支持的其他时区](#additional-time-zones)。

将 **dateTimeTimeZone** 与某一方法（例如 [创建](../api/user-post-events.md)或 [更新](../api/event-update.md)事件）结合使用时，请注意支持的实际时区，这可能是一个较小的子集。

### <a name="additional-time-zones"></a>其他时区

Etc/GMT+12

Etc/GMT+11

太平洋/火奴鲁鲁

美洲/安克雷奇

美洲/圣伊莎贝尔

美洲/洛杉矶

美洲/菲尼克斯

美洲/奇瓦瓦

美洲/丹佛

美洲/危地马拉

美洲/芝加哥

美洲/墨西哥城

美洲/里贾纳

美洲/波哥大

美洲/纽约

美洲/印第安纳/印第安纳波利斯

美洲/加拉加斯

美洲/亚松森

美洲/哈利法克斯

美洲/库亚巴

美洲/拉巴斯

美洲/圣地亚哥

美洲/圣约翰斯

美洲/圣保罗

美洲/阿根廷/布宜诺斯艾利斯

美洲/卡宴

美洲/戈特霍布

美洲/蒙得维的亚

美洲/巴伊亚

Etc/GMT+2

大西洋/亚速尔群岛

大西洋/佛得角

非洲/卡萨布兰卡

Etc/GMT

欧洲/伦敦

大西洋/雷克雅未克

欧洲/柏林

欧洲/布达佩斯

欧洲/巴黎

欧洲/华沙

非洲/拉各斯

非洲/温得和克

欧洲/布加勒斯特

亚洲/贝鲁特

非洲/开罗

亚洲/大马士革

非洲/约翰内斯堡

欧洲/基辅

欧洲/伊斯坦布尔

亚洲/耶路撒冷

亚洲/安曼

亚洲/巴格达

欧洲/加里宁格勒

亚洲/利雅得

非洲/内罗毕

亚洲/德黑兰

亚洲/迪拜

亚洲/巴库

欧洲/莫斯科

印度洋/毛里求斯

亚洲/第比利斯

亚洲/埃里温

亚洲/喀布尔

亚洲/卡拉奇

亚洲/塔什干

亚洲/加尔各答

亚洲/科伦坡

亚洲/加德满都

亚洲/阿斯塔纳（阿拉木图）

亚洲/达卡

亚洲/叶卡捷琳堡

亚洲/仰光

亚洲/曼谷

亚洲/新西伯利亚

亚洲/上海

亚洲/克拉斯诺亚尔斯克

亚洲/新加坡

澳大利亚/珀斯

亚洲/台北

亚洲/乌兰巴托

亚洲/伊尔库茨克

亚洲/东京

亚洲/首尔

澳洲/阿德莱德

澳洲/达尔文

澳洲/布里斯班

澳洲/悉尼

太平洋/莫尔斯比港

澳洲/霍巴特

亚洲/雅库茨克

太平洋/瓜达尔卡纳尔

亚洲/符拉迪沃斯托克

太平洋/奥克兰

Etc/GMT-12

太平洋/斐济

亚洲/马加丹

太平洋/汤加塔布

太平洋/阿皮亚

太平洋/圣诞岛

## <a name="json-representation"></a>JSON 表示形式

下面是资源的 JSON 表示形式。

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

