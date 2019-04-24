---
title: alertHistoryState 资源类型
description: 存储对警报所做的更改。
localization_priority: Normal
author: preetikr
ms.prod: security
ms.openlocfilehash: 1a7975d870389be5163a8f230f6a6cc4cd1425c3
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: zh-CN
ms.lasthandoff: 04/24/2019
ms.locfileid: "32461045"
---
# <a name="alerthistorystate-resource-type"></a><span data-ttu-id="b9d05-103">alertHistoryState 资源类型</span><span class="sxs-lookup"><span data-stu-id="b9d05-103">alertHistoryState resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="b9d05-104">存储对警报所做的更改。</span><span class="sxs-lookup"><span data-stu-id="b9d05-104">Stores changes made to alerts.</span></span>

## <a name="properties"></a><span data-ttu-id="b9d05-105">属性</span><span class="sxs-lookup"><span data-stu-id="b9d05-105">Properties</span></span>

| <span data-ttu-id="b9d05-106">属性</span><span class="sxs-lookup"><span data-stu-id="b9d05-106">Property</span></span>     | <span data-ttu-id="b9d05-107">类型</span><span class="sxs-lookup"><span data-stu-id="b9d05-107">Type</span></span>        | <span data-ttu-id="b9d05-108">说明</span><span class="sxs-lookup"><span data-stu-id="b9d05-108">Description</span></span> |
|:-------------|:------------|:------------|
|<span data-ttu-id="b9d05-109">appId</span><span class="sxs-lookup"><span data-stu-id="b9d05-109">appId</span></span>|<span data-ttu-id="b9d05-110">字符串</span><span class="sxs-lookup"><span data-stu-id="b9d05-110">String</span></span>| <span data-ttu-id="b9d05-111">向警报提交更新 (修补程序) 的呼叫应用程序的应用程序 ID。</span><span class="sxs-lookup"><span data-stu-id="b9d05-111">The Application ID of the calling application that submitted an update (PATCH) to the alert.</span></span> <span data-ttu-id="b9d05-112">应从身份验证令牌中提取 appId, 并且调用应用程序不手动输入该 appId。</span><span class="sxs-lookup"><span data-stu-id="b9d05-112">The appId should be extracted from the auth token and not entered manually by the calling application.</span></span> |
|<span data-ttu-id="b9d05-113">assignedTo</span><span class="sxs-lookup"><span data-stu-id="b9d05-113">assignedTo</span></span>|<span data-ttu-id="b9d05-114">String</span><span class="sxs-lookup"><span data-stu-id="b9d05-114">String</span></span>| <span data-ttu-id="b9d05-115">向其分配了警报的用户的 UPN (注意: alert。分配程序仅存储最后一个 value/UPN)。</span><span class="sxs-lookup"><span data-stu-id="b9d05-115">UPN of user the alert was assigned to (note: alert.assignedTo only stores the last value/UPN).</span></span> |
|<span data-ttu-id="b9d05-116">comments</span><span class="sxs-lookup"><span data-stu-id="b9d05-116">comments</span></span>|<span data-ttu-id="b9d05-117">String collection</span><span class="sxs-lookup"><span data-stu-id="b9d05-117">String collection</span></span>|<span data-ttu-id="b9d05-118">登录用户输入的注释。</span><span class="sxs-lookup"><span data-stu-id="b9d05-118">Comment entered by signed-in user.</span></span>|
|<span data-ttu-id="b9d05-119">征求</span><span class="sxs-lookup"><span data-stu-id="b9d05-119">feedback</span></span>|<span data-ttu-id="b9d05-120">字符串</span><span class="sxs-lookup"><span data-stu-id="b9d05-120">String</span></span>| <span data-ttu-id="b9d05-121">此更新中有关通知的分析师反馈。</span><span class="sxs-lookup"><span data-stu-id="b9d05-121">Analyst feedback on the alert in this update.</span></span> <span data-ttu-id="b9d05-122">可取值为：`unknown`、`truePositive`、`falsePositive`、`benignPositive`。</span><span class="sxs-lookup"><span data-stu-id="b9d05-122">Possible values are: `unknown`, `truePositive`, `falsePositive`, `benignPositive`.</span></span>|
|<span data-ttu-id="b9d05-123">status</span><span class="sxs-lookup"><span data-stu-id="b9d05-123">status</span></span>|<span data-ttu-id="b9d05-124">字符串</span><span class="sxs-lookup"><span data-stu-id="b9d05-124">String</span></span>| <span data-ttu-id="b9d05-125">警报状态值 (如果已更新)。</span><span class="sxs-lookup"><span data-stu-id="b9d05-125">Alert status value (if updated).</span></span> <span data-ttu-id="b9d05-126">可取值为：`unknown`、`newAlert`、`inProgress`、`resolved` 或 `dismissed`。</span><span class="sxs-lookup"><span data-stu-id="b9d05-126">Possible values are: `unknown`, `newAlert`, `inProgress`, `resolved`, `dismissed`.</span></span>|
|<span data-ttu-id="b9d05-127">updatedDateTime</span><span class="sxs-lookup"><span data-stu-id="b9d05-127">updatedDateTime</span></span>|<span data-ttu-id="b9d05-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b9d05-128">DateTimeOffset</span></span>| <span data-ttu-id="b9d05-129">通知更新的日期和时间。</span><span class="sxs-lookup"><span data-stu-id="b9d05-129">Date and time of the alert update.</span></span> <span data-ttu-id="b9d05-130">时间戳类型表示使用 ISO 8601 格式的日期和时间信息，并且始终处于 UTC 时间。</span><span class="sxs-lookup"><span data-stu-id="b9d05-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="b9d05-131">例如，2014 年 1 月 1 日午夜 UTC 如下所示：`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="b9d05-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="b9d05-132">user</span><span class="sxs-lookup"><span data-stu-id="b9d05-132">user</span></span>|<span data-ttu-id="b9d05-133">字符串</span><span class="sxs-lookup"><span data-stu-id="b9d05-133">String</span></span>| <span data-ttu-id="b9d05-134">更新了警报的已登录用户 (在用户/委派身份验证模式下) 中的 UPN。</span><span class="sxs-lookup"><span data-stu-id="b9d05-134">UPN of the signed-in user that updated the alert (taken from the bearer token - if in user/delegated auth mode).</span></span> |

## <a name="json-representation"></a><span data-ttu-id="b9d05-135">JSON 表示形式</span><span class="sxs-lookup"><span data-stu-id="b9d05-135">JSON representation</span></span>

<span data-ttu-id="b9d05-136">下面是资源的 JSON 表示形式。</span><span class="sxs-lookup"><span data-stu-id="b9d05-136">The following is a JSON representation of the resource.</span></span>

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