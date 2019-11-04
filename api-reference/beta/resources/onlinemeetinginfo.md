---
title: onlineMeetingInfo 资源类型
description: 用于联机加入会议的与会者的详细信息。
localization_priority: Normal
author: VinodRavichandran
ms.prod: microsoft-teams
doc_type: resourcePageType
ms.openlocfilehash: 7ed8543be8b1d22c797d0033dcd0d41ba6308888
ms.sourcegitcommit: 62507617292d5ad8598e83a8a253c986d9bac787
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 11/02/2019
ms.locfileid: "37939388"
---
# <a name="onlinemeetinginfo-resource-type"></a><span data-ttu-id="ebfcb-103">onlineMeetingInfo 资源类型</span><span class="sxs-lookup"><span data-stu-id="ebfcb-103">onlineMeetingInfo resource type</span></span>

<span data-ttu-id="ebfcb-104">用于联机加入会议的与会者的详细信息。</span><span class="sxs-lookup"><span data-stu-id="ebfcb-104">Details for an attendee to join the meeting online.</span></span>

## <a name="properties"></a><span data-ttu-id="ebfcb-105">属性</span><span class="sxs-lookup"><span data-stu-id="ebfcb-105">Properties</span></span>

| <span data-ttu-id="ebfcb-106">属性</span><span class="sxs-lookup"><span data-stu-id="ebfcb-106">Property</span></span>     | <span data-ttu-id="ebfcb-107">类型</span><span class="sxs-lookup"><span data-stu-id="ebfcb-107">Type</span></span>        | <span data-ttu-id="ebfcb-108">描述</span><span class="sxs-lookup"><span data-stu-id="ebfcb-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="ebfcb-109">conferenceId</span><span class="sxs-lookup"><span data-stu-id="ebfcb-109">conferenceId</span></span>|<span data-ttu-id="ebfcb-110">字符串</span><span class="sxs-lookup"><span data-stu-id="ebfcb-110">String</span></span>| <span data-ttu-id="ebfcb-111">会议的 ID。</span><span class="sxs-lookup"><span data-stu-id="ebfcb-111">The ID of the conference.</span></span>|
|<span data-ttu-id="ebfcb-112">joinUrl</span><span class="sxs-lookup"><span data-stu-id="ebfcb-112">joinUrl</span></span>|<span data-ttu-id="ebfcb-113">字符串</span><span class="sxs-lookup"><span data-stu-id="ebfcb-113">String</span></span>| <span data-ttu-id="ebfcb-114">启动联机会议的外部链接。</span><span class="sxs-lookup"><span data-stu-id="ebfcb-114">The external link that launches the online meeting.</span></span> <span data-ttu-id="ebfcb-115">这是客户端将启动到浏览器并将重定向用户加入会议的 URL。</span><span class="sxs-lookup"><span data-stu-id="ebfcb-115">This is a URL that clients will launch into a browser and will redirect the user to join the meeting.</span></span>|
|<span data-ttu-id="ebfcb-116">phones</span><span class="sxs-lookup"><span data-stu-id="ebfcb-116">phones</span></span>|<span data-ttu-id="ebfcb-117">[phone](phone.md) collection</span><span class="sxs-lookup"><span data-stu-id="ebfcb-117">[phone](phone.md) collection</span></span>| <span data-ttu-id="ebfcb-118">与此会议关联的所有电话号码。</span><span class="sxs-lookup"><span data-stu-id="ebfcb-118">All of the phone numbers associated with this conference.</span></span>|
|<span data-ttu-id="ebfcb-119">quickDial</span><span class="sxs-lookup"><span data-stu-id="ebfcb-119">quickDial</span></span>|<span data-ttu-id="ebfcb-120">字符串</span><span class="sxs-lookup"><span data-stu-id="ebfcb-120">String</span></span>| <span data-ttu-id="ebfcb-121">此调用的预格式化的 quickdial。</span><span class="sxs-lookup"><span data-stu-id="ebfcb-121">The pre-formatted quickdial for this call.</span></span>|
|<span data-ttu-id="ebfcb-122">tollFreeNumbers</span><span class="sxs-lookup"><span data-stu-id="ebfcb-122">tollFreeNumbers</span></span>|<span data-ttu-id="ebfcb-123">String collection</span><span class="sxs-lookup"><span data-stu-id="ebfcb-123">String collection</span></span>| <span data-ttu-id="ebfcb-124">可用于加入会议的免费电话号码。</span><span class="sxs-lookup"><span data-stu-id="ebfcb-124">The toll free numbers that can be used to join the conference.</span></span>|
|<span data-ttu-id="ebfcb-125">tollNumber</span><span class="sxs-lookup"><span data-stu-id="ebfcb-125">tollNumber</span></span>|<span data-ttu-id="ebfcb-126">字符串</span><span class="sxs-lookup"><span data-stu-id="ebfcb-126">String</span></span>| <span data-ttu-id="ebfcb-127">可用于加入会议的收费号码。</span><span class="sxs-lookup"><span data-stu-id="ebfcb-127">The toll number that can be used to join the conference.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ebfcb-128">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="ebfcb-128">JSON representation</span></span>

<span data-ttu-id="ebfcb-129">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="ebfcb-129">The following is a JSON representation of the resource.</span></span>

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
