---
title: alertHistoryState 资源类型
description: 存储对警报所做的更改。
localization_priority: Normal
author: preetikr
ms.prod: security
doc_type: resourcePageType
ms.openlocfilehash: 2bc1c1a58f6f7f073b6803adbee07b4b2990a0e1
ms.sourcegitcommit: 14648839f2feac2e5d6c8f876b7ae43e996ea6a0
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 03/11/2021
ms.locfileid: "50722165"
---
# <a name="alerthistorystate-resource-type"></a><span data-ttu-id="2ddb5-103">alertHistoryState 资源类型</span><span class="sxs-lookup"><span data-stu-id="2ddb5-103">alertHistoryState resource type</span></span>

<span data-ttu-id="2ddb5-104">命名空间：microsoft.graph</span><span class="sxs-lookup"><span data-stu-id="2ddb5-104">Namespace: microsoft.graph</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="2ddb5-105">存储对警报所做的更改。</span><span class="sxs-lookup"><span data-stu-id="2ddb5-105">Stores changes made to alerts.</span></span>

## <a name="properties"></a><span data-ttu-id="2ddb5-106">属性</span><span class="sxs-lookup"><span data-stu-id="2ddb5-106">Properties</span></span>

| <span data-ttu-id="2ddb5-107">属性</span><span class="sxs-lookup"><span data-stu-id="2ddb5-107">Property</span></span>     | <span data-ttu-id="2ddb5-108">类型</span><span class="sxs-lookup"><span data-stu-id="2ddb5-108">Type</span></span>        | <span data-ttu-id="2ddb5-109">说明</span><span class="sxs-lookup"><span data-stu-id="2ddb5-109">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="2ddb5-110">appId</span><span class="sxs-lookup"><span data-stu-id="2ddb5-110">appId</span></span>|<span data-ttu-id="2ddb5-111">String</span><span class="sxs-lookup"><span data-stu-id="2ddb5-111">String</span></span>| <span data-ttu-id="2ddb5-112">提交更新的调用应用程序的应用程序 ID (PATCH) 警报。</span><span class="sxs-lookup"><span data-stu-id="2ddb5-112">The Application ID of the calling application that submitted an update (PATCH) to the alert.</span></span> <span data-ttu-id="2ddb5-113">appId 应从身份验证令牌中提取，调用应用程序不应手动输入。</span><span class="sxs-lookup"><span data-stu-id="2ddb5-113">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span> |
|<span data-ttu-id="2ddb5-114">assignedTo</span><span class="sxs-lookup"><span data-stu-id="2ddb5-114">assignedTo</span></span>|<span data-ttu-id="2ddb5-115">String</span><span class="sxs-lookup"><span data-stu-id="2ddb5-115">String</span></span>| <span data-ttu-id="2ddb5-116">警报已分配给用户的 UPN， (注意：alert.assignedTo 仅存储最后一个值/UPN) 。</span><span class="sxs-lookup"><span data-stu-id="2ddb5-116">UPN of user the alert was assigned to (note: alert.assignedTo only stores the last value/UPN).</span></span> |
|<span data-ttu-id="2ddb5-117">comments</span><span class="sxs-lookup"><span data-stu-id="2ddb5-117">comments</span></span>|<span data-ttu-id="2ddb5-118">字符串集合</span><span class="sxs-lookup"><span data-stu-id="2ddb5-118">String collection</span></span>|<span data-ttu-id="2ddb5-119">登录用户输入的注释。</span><span class="sxs-lookup"><span data-stu-id="2ddb5-119">Comment entered by signed-in user.</span></span>|
|<span data-ttu-id="2ddb5-120">反馈</span><span class="sxs-lookup"><span data-stu-id="2ddb5-120">feedback</span></span>|<span data-ttu-id="2ddb5-121">String</span><span class="sxs-lookup"><span data-stu-id="2ddb5-121">String</span></span>| <span data-ttu-id="2ddb5-122">分析员对此更新中警报的反馈。</span><span class="sxs-lookup"><span data-stu-id="2ddb5-122">Analyst feedback on the alert in this update.</span></span> <span data-ttu-id="2ddb5-123">可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。</span><span class="sxs-lookup"><span data-stu-id="2ddb5-123">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="2ddb5-124">状态</span><span class="sxs-lookup"><span data-stu-id="2ddb5-124">status</span></span>|<span data-ttu-id="2ddb5-125">String</span><span class="sxs-lookup"><span data-stu-id="2ddb5-125">String</span></span>| <span data-ttu-id="2ddb5-126">警报状态值 (更新) 。</span><span class="sxs-lookup"><span data-stu-id="2ddb5-126">Alert status value (if updated).</span></span> <span data-ttu-id="2ddb5-127">可取值为：`unknown`、`newAlert`、`inProgress`、`resolved`、`dismissed`。</span><span class="sxs-lookup"><span data-stu-id="2ddb5-127">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span></span>|
|<span data-ttu-id="2ddb5-128">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="2ddb5-128">updatedDateTime</span></span>|<span data-ttu-id="2ddb5-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2ddb5-129">DateTimeOffset</span></span>| <span data-ttu-id="2ddb5-130">警报更新的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="2ddb5-130">Date and time of the alert update.</span></span> <span data-ttu-id="2ddb5-131">时间戳类型表示采用 ISO 8601 格式的日期和时间信息，始终采用 UTC 时区。</span><span class="sxs-lookup"><span data-stu-id="2ddb5-131">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2ddb5-132">例如，2014 年 1 月 1 日午夜 UTC 为 `2014-01-01T00:00:00Z`</span><span class="sxs-lookup"><span data-stu-id="2ddb5-132">For example, midnight UTC on Jan 1, 2014 is `2014-01-01T00:00:00Z`</span></span>|
|<span data-ttu-id="2ddb5-133">user</span><span class="sxs-lookup"><span data-stu-id="2ddb5-133">user</span></span>|<span data-ttu-id="2ddb5-134">String</span><span class="sxs-lookup"><span data-stu-id="2ddb5-134">String</span></span>| <span data-ttu-id="2ddb5-135">更新警报的已登录用户的 UPN， (令牌获取的警报- 如果用户/委派身份验证模式) 。</span><span class="sxs-lookup"><span data-stu-id="2ddb5-135">UPN of the signed-in user that updated the alert (taken from the bearer token - if in user/delegated auth mode).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="2ddb5-136">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="2ddb5-136">JSON representation</span></span>

<span data-ttu-id="2ddb5-137">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="2ddb5-137">The following is a JSON representation of the resource.</span></span>

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

