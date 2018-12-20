---
title: commsOperation 资源类型
description: 某些长时间运行操作的状态。
author: VinodRavichandran
ms.openlocfilehash: 09d3f81e8f6307850d94cfab43f98426dae47a5f
ms.sourcegitcommit: 0b3a57ac8b99871e56389f9be15e4f96e219f635
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 12/20/2018
ms.locfileid: "27380350"
---
# <a name="commsoperation-resource-type"></a><span data-ttu-id="81cf5-103">commsOperation 资源类型</span><span class="sxs-lookup"><span data-stu-id="81cf5-103">commsOperation resource type</span></span>

> <span data-ttu-id="81cf5-104">**重要说明：** Microsoft Graph 中 /beta 版本下的 API 是预览版，可能会发生变化。</span><span class="sxs-lookup"><span data-stu-id="81cf5-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="81cf5-105">不支持在生产应用程序中使用这些 API。</span><span class="sxs-lookup"><span data-stu-id="81cf5-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="81cf5-106">某些长时间运行操作的状态。</span><span class="sxs-lookup"><span data-stu-id="81cf5-106">The status of certain long-running operations.</span></span>

## <a name="methods"></a><span data-ttu-id="81cf5-107">方法</span><span class="sxs-lookup"><span data-stu-id="81cf5-107">Methods</span></span>
<span data-ttu-id="81cf5-108">无</span><span class="sxs-lookup"><span data-stu-id="81cf5-108">None</span></span>

## <a name="properties"></a><span data-ttu-id="81cf5-109">属性</span><span class="sxs-lookup"><span data-stu-id="81cf5-109">Properties</span></span>

| <span data-ttu-id="81cf5-110">属性</span><span class="sxs-lookup"><span data-stu-id="81cf5-110">Property</span></span>           | <span data-ttu-id="81cf5-111">类型</span><span class="sxs-lookup"><span data-stu-id="81cf5-111">Type</span></span>                        | <span data-ttu-id="81cf5-112">说明</span><span class="sxs-lookup"><span data-stu-id="81cf5-112">Description</span></span>                                                                     |
| :----------------- | :-------------------------- | :-------------------------------------------------------------------------------|
| <span data-ttu-id="81cf5-113">clientContext</span><span class="sxs-lookup"><span data-stu-id="81cf5-113">clientContext</span></span>      | <span data-ttu-id="81cf5-114">字符串</span><span class="sxs-lookup"><span data-stu-id="81cf5-114">String</span></span>                      | <span data-ttu-id="81cf5-115">客户端上下文。</span><span class="sxs-lookup"><span data-stu-id="81cf5-115">The client context.</span></span>                                                             |
| <span data-ttu-id="81cf5-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="81cf5-116">createdDateTime</span></span>    | <span data-ttu-id="81cf5-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81cf5-117">DateTimeOffset</span></span>              | <span data-ttu-id="81cf5-118">操作的开始时间。</span><span class="sxs-lookup"><span data-stu-id="81cf5-118">The start time of the operation.</span></span>                                                |
| <span data-ttu-id="81cf5-119">id</span><span class="sxs-lookup"><span data-stu-id="81cf5-119">id</span></span>                 | <span data-ttu-id="81cf5-120">字符串</span><span class="sxs-lookup"><span data-stu-id="81cf5-120">String</span></span>                      | <span data-ttu-id="81cf5-121">操作 ID。只读。</span><span class="sxs-lookup"><span data-stu-id="81cf5-121">The operation id. Read-only.</span></span> <span data-ttu-id="81cf5-122">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="81cf5-122">Server generated.</span></span>                                  |
| <span data-ttu-id="81cf5-123">lastActionDateTime</span><span class="sxs-lookup"><span data-stu-id="81cf5-123">lastActionDateTime</span></span> | <span data-ttu-id="81cf5-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="81cf5-124">DateTimeOffset</span></span>              | <span data-ttu-id="81cf5-125">操作的上次活动时间。</span><span class="sxs-lookup"><span data-stu-id="81cf5-125">The time of the last action of the operation.</span></span>                                   |
| <span data-ttu-id="81cf5-126">resultInfo</span><span class="sxs-lookup"><span data-stu-id="81cf5-126">resultInfo</span></span>         | [<span data-ttu-id="81cf5-127">resultInfo</span><span class="sxs-lookup"><span data-stu-id="81cf5-127">resultInfo</span></span>](resultinfo.md) | <span data-ttu-id="81cf5-128">结果的信息。</span><span class="sxs-lookup"><span data-stu-id="81cf5-128">The result information.</span></span> <span data-ttu-id="81cf5-129">只读。</span><span class="sxs-lookup"><span data-stu-id="81cf5-129">Read-only.</span></span> <span data-ttu-id="81cf5-130">生成的服务器。</span><span class="sxs-lookup"><span data-stu-id="81cf5-130">Server generated.</span></span>                            |
| <span data-ttu-id="81cf5-131">status</span><span class="sxs-lookup"><span data-stu-id="81cf5-131">status</span></span>             | <span data-ttu-id="81cf5-132">String</span><span class="sxs-lookup"><span data-stu-id="81cf5-132">String</span></span>                      | <span data-ttu-id="81cf5-133">可取值为 `notStarted`、`running`、`completed`、`failed`。</span><span class="sxs-lookup"><span data-stu-id="81cf5-133">Possible values are: `notStarted`, `running`, `completed`, `failed`.</span></span> <span data-ttu-id="81cf5-134">只读。</span><span class="sxs-lookup"><span data-stu-id="81cf5-134">Read-only.</span></span> |

## <a name="relationships"></a><span data-ttu-id="81cf5-135">Relationships</span><span class="sxs-lookup"><span data-stu-id="81cf5-135">Relationships</span></span>
<span data-ttu-id="81cf5-136">无</span><span class="sxs-lookup"><span data-stu-id="81cf5-136">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="81cf5-137">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="81cf5-137">JSON representation</span></span>

<span data-ttu-id="81cf5-138">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="81cf5-138">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "String",
  "createdDateTime": "String (timestamp)",
  "id": "String (identifier)",
  "lastActionDateTime": "String (timestamp)",
  "resultInfo": { "@odata.type": "#microsoft.graph.resultInfo" },
  "status": "notStarted | running | completed | failed"
}
```

## <a name="example"></a><span data-ttu-id="81cf5-139">示例</span><span class="sxs-lookup"><span data-stu-id="81cf5-139">Example</span></span>

<!-- {
  "blockType": "example",
  "@odata.type": "microsoft.graph.commsOperation"
}-->
```json
{
  "clientContext": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "createdDateTime": "2018-09-06T15:58:41Z",
  "id": "ABB33D04-3A2C-4D78-996F-9EEEF55EF119",
  "lastActionDateTime": "2018-09-06T15:58:41Z",
  "resultInfo": {
    "@odata.type": "#microsoft.graph.resultInfo",
    "code": "200"
  },
  "status": "completed"
}
```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "commsOperation resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
