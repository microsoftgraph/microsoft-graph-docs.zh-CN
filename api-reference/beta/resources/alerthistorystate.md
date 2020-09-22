---
title: alertHistoryState 资源类型
description: 存储对警报所做的更改。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: cf8043b4409b29220841e2706649050003b09f34
ms.sourcegitcommit: acdf972e2f25fef2c6855f6f28a63c0762228ffa
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 09/18/2020
ms.locfileid: "48004277"
---
# <a name="alerthistorystate-resource-type"></a><span data-ttu-id="2e743-103">alertHistoryState 资源类型</span><span class="sxs-lookup"><span data-stu-id="2e743-103">alertHistoryState resource type</span></span>

<span data-ttu-id="2e743-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2e743-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2e743-105">存储对警报所做的更改。</span><span class="sxs-lookup"><span data-stu-id="2e743-105">Stores changes made to alerts.</span></span>

## <a name="properties"></a><span data-ttu-id="2e743-106">属性</span><span class="sxs-lookup"><span data-stu-id="2e743-106">Properties</span></span>

| <span data-ttu-id="2e743-107">属性</span><span class="sxs-lookup"><span data-stu-id="2e743-107">Property</span></span>     | <span data-ttu-id="2e743-108">类型</span><span class="sxs-lookup"><span data-stu-id="2e743-108">Type</span></span>        | <span data-ttu-id="2e743-109">说明</span><span class="sxs-lookup"><span data-stu-id="2e743-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2e743-110">appId</span><span class="sxs-lookup"><span data-stu-id="2e743-110">appId</span></span>|<span data-ttu-id="2e743-111">String</span><span class="sxs-lookup"><span data-stu-id="2e743-111">String</span></span>| <span data-ttu-id="2e743-112">向警报提交更新 (PATCH) 的调用应用程序的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="2e743-112">The Application ID of the calling application that submitted an update (PATCH) to the alert.</span></span> <span data-ttu-id="2e743-113">应从身份验证令牌中提取 appId，并且调用应用程序不手动输入该 appId。</span><span class="sxs-lookup"><span data-stu-id="2e743-113">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span> |
|<span data-ttu-id="2e743-114">assignedTo</span><span class="sxs-lookup"><span data-stu-id="2e743-114">assignedTo</span></span>|<span data-ttu-id="2e743-115">String</span><span class="sxs-lookup"><span data-stu-id="2e743-115">String</span></span>| <span data-ttu-id="2e743-116">用户的 UPN 已将警报分配给 (注意： alert。分配仅存储最后一个 value/UPN) 。</span><span class="sxs-lookup"><span data-stu-id="2e743-116">UPN of user the alert was assigned to (note: alert.assignedTo only stores the last value/UPN).</span></span> |
|<span data-ttu-id="2e743-117">comments</span><span class="sxs-lookup"><span data-stu-id="2e743-117">comments</span></span>|<span data-ttu-id="2e743-118">字符串集合</span><span class="sxs-lookup"><span data-stu-id="2e743-118">String collection</span></span>|<span data-ttu-id="2e743-119">登录用户输入的注释。</span><span class="sxs-lookup"><span data-stu-id="2e743-119">Comment entered by signed-in user.</span></span>|
|<span data-ttu-id="2e743-120">反馈</span><span class="sxs-lookup"><span data-stu-id="2e743-120">feedback</span></span>|<span data-ttu-id="2e743-121">String</span><span class="sxs-lookup"><span data-stu-id="2e743-121">String</span></span>| <span data-ttu-id="2e743-122">此更新中有关通知的分析师反馈。</span><span class="sxs-lookup"><span data-stu-id="2e743-122">Analyst feedback on the alert in this update.</span></span> <span data-ttu-id="2e743-123">可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。</span><span class="sxs-lookup"><span data-stu-id="2e743-123">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="2e743-124">状态</span><span class="sxs-lookup"><span data-stu-id="2e743-124">status</span></span>|<span data-ttu-id="2e743-125">String</span><span class="sxs-lookup"><span data-stu-id="2e743-125">String</span></span>| <span data-ttu-id="2e743-126">如果) 更新，则通知状态值 (。</span><span class="sxs-lookup"><span data-stu-id="2e743-126">Alert status value (if updated).</span></span> <span data-ttu-id="2e743-127">可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`、`dismissed`。</span><span class="sxs-lookup"><span data-stu-id="2e743-127">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span></span>|
|<span data-ttu-id="2e743-128">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2e743-128">updatedDateTime</span></span>|<span data-ttu-id="2e743-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2e743-129">DateTimeOffset</span></span>| <span data-ttu-id="2e743-130">通知更新的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2e743-130">Date and time of the alert update.</span></span> <span data-ttu-id="2e743-131">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="2e743-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2e743-132">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2e743-132">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2e743-133">user</span><span class="sxs-lookup"><span data-stu-id="2e743-133">user</span></span>|<span data-ttu-id="2e743-134">String</span><span class="sxs-lookup"><span data-stu-id="2e743-134">String</span></span>| <span data-ttu-id="2e743-135">更新了警报的已登录用户的 UPN (从持有者令牌中获取-如果在用户/委派身份验证模式中) 。</span><span class="sxs-lookup"><span data-stu-id="2e743-135">UPN of the signed-in user that updated the alert (taken from the bearer token - if in user/delegated auth mode).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2e743-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2e743-136">JSON representation</span></span>

<span data-ttu-id="2e743-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2e743-137">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.alertHistoryState",
  "baseType": null
}-->

```json
{
  "appId": "String",
  "assignedTo": "String",
  "comments": ["String"],
  "feedback": "String",
  "status": "String",
  "updatedDateTime": "String (timestamp)",
  "user": "String"
}
```

<!-- uuid: 16cd6b66-4b1a-43a1-adaf-3a886856ed98
2019-02-04 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "alertHistoryState resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->

