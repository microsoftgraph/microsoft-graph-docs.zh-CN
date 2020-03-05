---
title: onlineMeetingInfo 资源类型
description: 关于与会者如何加入联机会议的详细信息。
localization_priority: Normal
author: ananmishr
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 8ac6c42f28ed1f2adccd54fcd3bd6667f4113b7a
ms.sourcegitcommit: 272996d2772b51105ec25f1cf7482ecda3b74ebe
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/05/2020
ms.locfileid: "42522247"
---
# <a name="onlinemeetinginfo-resource-type"></a><span data-ttu-id="00faa-103">onlineMeetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="00faa-103">onlineMeetingInfo resource type</span></span>

<span data-ttu-id="00faa-104">命名空间： microsoft. graph</span><span class="sxs-lookup"><span data-stu-id="00faa-104">Namespace: microsoft.graph</span></span>

<span data-ttu-id="00faa-105">关于与会者如何加入联机会议的详细信息。</span><span class="sxs-lookup"><span data-stu-id="00faa-105">Details for an attendee to join the meeting online.</span></span>

## <a name="properties"></a><span data-ttu-id="00faa-106">属性</span><span class="sxs-lookup"><span data-stu-id="00faa-106">Properties</span></span>

| <span data-ttu-id="00faa-107">属性</span><span class="sxs-lookup"><span data-stu-id="00faa-107">Property</span></span>     | <span data-ttu-id="00faa-108">类型</span><span class="sxs-lookup"><span data-stu-id="00faa-108">Type</span></span>        | <span data-ttu-id="00faa-109">说明</span><span class="sxs-lookup"><span data-stu-id="00faa-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="00faa-110">conferenceId</span><span class="sxs-lookup"><span data-stu-id="00faa-110">conferenceId</span></span>|<span data-ttu-id="00faa-111">String</span><span class="sxs-lookup"><span data-stu-id="00faa-111">String</span></span>| <span data-ttu-id="00faa-112">会议的 ID。</span><span class="sxs-lookup"><span data-stu-id="00faa-112">The ID of the conference.</span></span>|
|<span data-ttu-id="00faa-113">joinUrl</span><span class="sxs-lookup"><span data-stu-id="00faa-113">joinUrl</span></span>|<span data-ttu-id="00faa-114">String</span><span class="sxs-lookup"><span data-stu-id="00faa-114">String</span></span>| <span data-ttu-id="00faa-115">启动联机会议的外部链接。</span><span class="sxs-lookup"><span data-stu-id="00faa-115">The external link that launches the online meeting.</span></span> <span data-ttu-id="00faa-116">这是客户端将启动到浏览器并将重定向用户加入会议的 URL。</span><span class="sxs-lookup"><span data-stu-id="00faa-116">This is a URL that clients will launch into a browser and will redirect the user to join the meeting.</span></span>|
|<span data-ttu-id="00faa-117">phones</span><span class="sxs-lookup"><span data-stu-id="00faa-117">phones</span></span>|<span data-ttu-id="00faa-118">[phone](phone.md) collection</span><span class="sxs-lookup"><span data-stu-id="00faa-118">[phone](phone.md) collection</span></span>| <span data-ttu-id="00faa-119">与此会议关联的所有电话号码。</span><span class="sxs-lookup"><span data-stu-id="00faa-119">All of the phone numbers associated with this conference.</span></span>|
|<span data-ttu-id="00faa-120">quickDial</span><span class="sxs-lookup"><span data-stu-id="00faa-120">quickDial</span></span>|<span data-ttu-id="00faa-121">String</span><span class="sxs-lookup"><span data-stu-id="00faa-121">String</span></span>| <span data-ttu-id="00faa-122">此调用的预格式化的 quickdial。</span><span class="sxs-lookup"><span data-stu-id="00faa-122">The pre-formatted quickdial for this call.</span></span>|
|<span data-ttu-id="00faa-123">tollFreeNumbers</span><span class="sxs-lookup"><span data-stu-id="00faa-123">tollFreeNumbers</span></span>|<span data-ttu-id="00faa-124">String 集合</span><span class="sxs-lookup"><span data-stu-id="00faa-124">String collection</span></span>| <span data-ttu-id="00faa-125">可用于加入会议的免费电话号码。</span><span class="sxs-lookup"><span data-stu-id="00faa-125">The toll free numbers that can be used to join the conference.</span></span>|
|<span data-ttu-id="00faa-126">tollNumber</span><span class="sxs-lookup"><span data-stu-id="00faa-126">tollNumber</span></span>|<span data-ttu-id="00faa-127">String</span><span class="sxs-lookup"><span data-stu-id="00faa-127">String</span></span>| <span data-ttu-id="00faa-128">可用于加入会议的收费号码。</span><span class="sxs-lookup"><span data-stu-id="00faa-128">The toll number that can be used to join the conference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="00faa-129">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="00faa-129">JSON representation</span></span>

<span data-ttu-id="00faa-130">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="00faa-130">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "@odata.type": "microsoft.graph.onlineMeetingInfo"
}-->

```json
{
  "conferenceId": "String",
  "joinUrl": "String",
  "phones": [{"@odata.type": "microsoft.graph.phone"}],
  "quickDial": "String",
  "tollFreeNumbers": ["String"],
  "tollNumber": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "onlineMeetingInfo resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->s
